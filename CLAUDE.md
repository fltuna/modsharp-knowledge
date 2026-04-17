# modsharp-catalog - Claude Code向け手順書

このリポジトリは ModSharp (CS2/Source2 C# modding framework) の
APIカタログ格納所。カタログ生成・更新は Claude Code がこの手順書に従って
自動実行する。

## 前提
- .NET 10 SDK がインストール済み
- カタログ生成ツール `ModSharpApiCatalog` が利用可能
  - デフォルト: `~/tools/ModSharpApiCatalog`
  - 環境変数 `MODSHARP_CATALOG_TOOL` で上書き可能
  - ツールが見つからない場合はユーザーに確認して停止する

## ユーザーから「カタログを更新して」等の指示があった場合の手順

### 手順1: 更新の有無を確認
```bash
cd external/modsharp
git fetch origin
LOCAL=$(git rev-parse HEAD)
REMOTE=$(git rev-parse origin/master)
```
- `LOCAL == REMOTE` なら更新なし。ユーザーに報告して終了。
- 差分がある場合は `git log --oneline $LOCAL..$REMOTE | head -20` で
  変更内容をユーザーに見せる。

### 手順2: submodule更新
repo ルートに戻って:
```bash
cd <repo root>
git submodule update --remote external/modsharp
```

### 手順3: ModSharp ビルド (Source Generator出力取得のため必須)
```bash
cd external/modsharp
dotnet restore
dotnet build --no-restore --configuration Release
```
- ビルド失敗時はエラー内容をユーザーに報告し、判断を仰ぐ
- ビルドせずにカタログ生成すると Source Generator 生成型が欠落する

### 手順4: カタログ生成
```bash
cd <repo root>
TOOL_PATH="${MODSHARP_CATALOG_TOOL:-$HOME/tools/ModSharpApiCatalog}"
SOLUTION=$(find external/modsharp -maxdepth 2 -name "*.sln" | head -1)
dotnet run --project "$TOOL_PATH" --configuration Release -- \
    --solution "$SOLUTION" \
    --output catalog
```

### 手順5: 変更確認
```bash
git status
git diff --stat catalog/
```
ユーザーに変更概要を報告する。

### 手順6: コミット (ユーザー確認後)
```bash
NEW_COMMIT=$(cd external/modsharp && git rev-parse --short HEAD)
git add -A
git commit -m "Update catalog to ModSharp $NEW_COMMIT"
```
push するかはユーザー判断に委ねる。

## 新マシン初回セットアップ
`--recurse-submodules` なしで clone された場合:
```bash
git submodule update --init --recursive
```

## トラブルシューティング

### MSBuildWorkspace のロード失敗
カタログ生成ツール側で `Microsoft.Build.Locator.RegisterDefaults()` が
呼ばれているか確認。ツール側の修正が必要な場合はユーザーに報告。

### Source Generator生成型がカタログに含まれない
- 手順3のビルドが成功しているか確認
- `catalog/indexes/generated-types.md` が空でないか確認
- 空の場合、ツール側の実装を確認する必要がある

### カタログ生成ツールが見つからない
- 環境変数 `MODSHARP_CATALOG_TOOL` を確認
- デフォルトパス `~/tools/ModSharpApiCatalog` の存在を確認
- 見つからない場合はユーザーに正しいパスを確認する

## 注意事項
- Source Generator出力(`*.g.cs`)はカタログに含める(除外しない)
- `catalog/.meta/generated-at` は変動値のため gitignore 済み
- ModSharpビルドが失敗するとカタログが不完全になる
- `patterns/` と `gotchas.md` は手動メンテ領域。AI による自動更新はしない

## このリポジトリで編集してよいもの / 編集してはいけないもの

### 編集してよい
- `catalog/` 配下 (生成ツールによる再生成のみ。手動編集はしない)
- `patterns/` 配下 (ユーザーが明示的に指示した場合のみ)
- `gotchas.md` (ユーザーが明示的に指示した場合のみ)
- `README.md`, `docs/usage.md`, この `CLAUDE.md`

### 編集してはいけない
- `external/modsharp/` 配下 (submodule の中身)
- `.gitmodules`
