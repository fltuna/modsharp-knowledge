# Usage

## Update workflow
Catalog updates happen inside a Claude Code session. No shell scripts
or CI automation are provided on purpose.

1. Open a Claude Code session in this repository.
2. Tell Claude "update the catalog" (or something equivalent).
3. Claude Code follows `CLAUDE.md` and runs the commands itself.
4. Review the diff and commit.

## Consuming the catalog from a plugin project

### 1. Add as a submodule
```bash
cd my-plugin
git submodule add <this-repo-url> refs/modsharp-knowledge
git commit -m "Add ModSharp knowledge reference"
```

### 2. Reference it from the plugin's `CLAUDE.md`
The catalog is large. Some files are small and worth loading into
context at session start (`@path` references); others are big and
should only be read on demand.

**Quickest path** — in the plugin repo, tell Claude Code:

> Follow `refs/modsharp-knowledge/init.md`

That runbook asks which preset you want (Full / Minimal / Custom),
then inserts the correct block into your `CLAUDE.md` between
`<!-- BEGIN modsharp-knowledge integration -->` / `<!-- END ... -->`
markers so a later re-run can update it in place.

**Manual path** — if you prefer to paste it yourself, use this snippet:

```markdown
## ModSharp reference material

When working on ModSharp-related code, read on demand (do NOT use
`@` auto-loading — it has broken Claude Code startup with this
integration):

- `refs/modsharp-knowledge/catalog/_index.md` — top-level index, read this first
- `refs/modsharp-knowledge/gotchas.md` — known pitfalls
- `refs/modsharp-knowledge/catalog/projects/Sharp.Shared/_index.md` — main consumer-facing API
- `refs/modsharp-knowledge/catalog/projects/Sharp.Shared/namespaces/` — per-namespace type details
- `refs/modsharp-knowledge/catalog/indexes/` — cross-cutting indexes
- `refs/modsharp-knowledge/patterns/` — verified usage patterns

## Workflow when touching ModSharp APIs
1. Start from `refs/modsharp-knowledge/catalog/_index.md` to find the right project.
2. Read `refs/modsharp-knowledge/catalog/projects/Sharp.Shared/_index.md` to locate the namespace.
3. Read the relevant `namespaces/<Namespace>.md` file for type signatures.
4. Check `refs/modsharp-knowledge/patterns/` for a verified precedent before writing new code.
5. Scan `refs/modsharp-knowledge/gotchas.md` before committing anything non-trivial.

## Keeping the catalog current
If the catalog looks stale, or the user mentions a ModSharp API that
isn't in it, suggest refreshing the submodule before proceeding:

    git submodule update --remote refs/modsharp-knowledge
    git commit -m "Update modsharp-knowledge submodule"

Commit the pointer bump separately so it's easy to audit.

## Notes
- Never load large per-namespace files unnecessarily — `_global.md` alone exceeds 60k lines.
- Do not prefix any of the paths above with `@`.
```

### Which files to reference — cheat sheet

All references are **plain paths, no `@` prefix**. `@`-auto-loading
has broken Claude Code startup in this integration; use on-demand
reads.

| File / directory | Typical size | Notes |
|---|---|---|
| `catalog/_index.md` | small | Top-level index, read first when entering ModSharp context |
| `gotchas.md` | small | Known pitfalls — worth reading before non-trivial changes |
| `catalog/projects/Sharp.Shared/_index.md` | medium | Main consumer-facing API navigation |
| `catalog/projects/Sharp.Shared/namespaces/*.md` | **large** (`_global.md` exceeds 60k lines) | Read a specific namespace file only when needed |
| `catalog/indexes/entry-points.md` | medium | Useful during scaffolding of a new plugin |
| `catalog/indexes/generated-types.md` | medium | Useful when working with protobuf / generated code |
| `patterns/` | small per file | Read individual patterns as relevant |

A plugin consumer only needs the submodule. The generator tool at
`~/tools/ModSharpApiCatalog` is required for **updating** the catalog,
not for **consuming** it.

### 3. Pull catalog updates into the plugin
When the plugin wants a fresher catalog:
```bash
git submodule update --remote refs/modsharp-knowledge
git commit -am "Update catalog reference"
```

## Cloning on a new machine
```bash
git clone --recurse-submodules <plugin-repo-url>
```
Don't forget `--recurse-submodules`. You can make it the default with
`git config --global submodule.recurse true`.

## Note: testing submodule wiring against a local path
Modern git refuses `file://` submodule clones by default. When wiring
this catalog into a throwaway test project on the same filesystem,
allow it for that single command:
```bash
git -c protocol.file.allow=always submodule add /path/to/modsharp-knowledge refs/modsharp-knowledge
```
HTTPS-hosted submodules don't need this.
