# init.md — Setup runbook for plugin consumers

**Audience:** you are Claude Code running inside a **plugin project**
that has added `modsharp-knowledge` as a submodule at `refs/modsharp-knowledge`.
The user pointed you at this file. Your job: wire the catalog into the
plugin's own `CLAUDE.md`, interactively.

If you are running inside the `modsharp-knowledge` repo itself, this is
the wrong file — stop and tell the user.

## Step 1: verify environment
1. Confirm that `refs/modsharp-knowledge/catalog/_index.md` exists
   relative to the plugin repo root. If not, tell the user the submodule
   isn't checked out and stop.
2. Locate the plugin's `CLAUDE.md`:
   - If `CLAUDE.md` exists at the plugin root, use it.
   - If not, **ask the user before creating one** — creating `CLAUDE.md`
     affects every future Claude Code session in the repo.

## Step 2: ask the user which preset to apply
Use the `AskUserQuestion` tool (or an equivalent interactive prompt).
Present these options and default to **Full** if the user doesn't care:

| Option | What it does |
|---|---|
| **Full** (recommended) | Always-on `@`-refs + workflow checklist + browse list + notes |
| **Minimal** | Only the always-on `@`-refs (`_index.md`, `gotchas.md`) |
| **Custom** | Walk through each block and ask per item |
| **Cancel** | Do nothing |

## Step 3: check for an existing integration
Search the plugin `CLAUDE.md` for the marker:

```
<!-- BEGIN modsharp-knowledge integration -->
```

- If present: ask the user whether to **replace** the existing block or **skip**.
- If absent: continue.

## Step 4: compose the snippet
Assemble the block the user chose. Always wrap it with the BEGIN / END
markers so a later re-run of this runbook can locate and replace it.

### Full preset

```markdown
<!-- BEGIN modsharp-knowledge integration -->
## ModSharp reference material

When you work on anything ModSharp-related, read these on demand
(do NOT use `@` auto-loading — some catalog files are huge and
`@`-prefixed paths in Markdown have caused Claude Code to fail to
start in this repo's integration history):

- `refs/modsharp-knowledge/catalog/_index.md` — top-level index, read this first
- `refs/modsharp-knowledge/gotchas.md` — known pitfalls, skim before committing tricky code
- `refs/modsharp-knowledge/catalog/projects/Sharp.Shared/_index.md` — main consumer-facing API
- `refs/modsharp-knowledge/catalog/projects/Sharp.Shared/namespaces/` — per-namespace type details
- `refs/modsharp-knowledge/catalog/indexes/` — cross-cutting indexes (by-attribute, by-interface, entry-points, generated-types)
- `refs/modsharp-knowledge/patterns/` — verified usage patterns

## Workflow when touching ModSharp APIs
1. Start from `refs/modsharp-knowledge/catalog/_index.md` to find the right project.
2. Read `refs/modsharp-knowledge/catalog/projects/Sharp.Shared/_index.md` to locate the namespace.
3. Read the relevant `namespaces/<Namespace>.md` file for type signatures.
4. Check `refs/modsharp-knowledge/patterns/` for a verified precedent.
5. Scan `refs/modsharp-knowledge/gotchas.md` before committing tricky code.

## Keeping the catalog current
- Before starting substantial ModSharp work, sanity-check the catalog age.
  If it looks stale, or if the user mentions an API that isn't in the
  catalog, suggest refreshing the submodule before proceeding:
  ```bash
  git submodule update --remote refs/modsharp-knowledge
  git commit -m "Update modsharp-knowledge submodule"
  ```
- Always commit the submodule pointer bump as its own commit so the
  refresh is easy to audit and revert.
- Do not silently refresh without telling the user — the new catalog
  may change what APIs are visible.

## Notes
- Never auto-load `catalog/projects/*/namespaces/*.md` with `@` — some files exceed 60k lines and will blow the context window.
<!-- END modsharp-knowledge integration -->
```

### Minimal preset

```markdown
<!-- BEGIN modsharp-knowledge integration -->
## ModSharp reference material

When working on ModSharp-related code, read on demand:

- `refs/modsharp-knowledge/catalog/_index.md` — top-level index
- `refs/modsharp-knowledge/gotchas.md` — known pitfalls

Do not use `@` auto-loading for these paths — it has historically
broken Claude Code startup in this repo's integration. Never
auto-load per-namespace files — some exceed 60k lines.

If the catalog looks stale, suggest
`git submodule update --remote refs/modsharp-knowledge` before proceeding.
<!-- END modsharp-knowledge integration -->
```

### Custom preset
Offer these blocks individually and assemble only the ones the user chooses:

- **Reference list** — plain paths to `_index.md`, `gotchas.md`, and the browsable directories
- **Workflow checklist** — the 5-step workflow
- **Keep-current reminder** — guidance for suggesting `git submodule update --remote` when the catalog is stale
- **Notes** — the "never auto-load large files" / "do not use `@` prefix" warning

Never include raw `@refs/...` auto-import lines — they have broken
Claude Code startup and the recommendation is to reference files by
plain path only.

Whichever blocks the user picks, wrap the final output with the same
BEGIN / END markers.

## Step 5: write the change
- If `CLAUDE.md` exists:
  - If the marker already existed and the user chose **replace**, substitute
    the block between the markers (inclusive).
  - Otherwise, append a blank line and the new block at the end of the file.
- If `CLAUDE.md` does not exist and the user approved creating one:
  - Create the file containing only the chosen block.

## Step 6: summarize and stop
Report back:
- Which file you touched.
- Which preset you applied.
- The lines you added or replaced.

**Do not commit** — leave that to the user so they can review the diff
first.

## Language policy
The snippets above are in English. Even if the user is speaking another
language with you, keep the inserted block in English for consistency
with the rest of the catalog.
