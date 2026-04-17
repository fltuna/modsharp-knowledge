# Sharp.Modules.MenuManager.Core

Project: Sharp.Modules.MenuManager
Types: 2 (0 generated)

### record struct BuiltMenuItem : System.ValueType, System.IEquatable<Sharp.Modules.MenuManager.Core.BuiltMenuItem>

- FullName: `Sharp.Modules.MenuManager.Core.BuiltMenuItem`
- Kind: record struct
- Modifiers: public, readonly
- Source: Sharp.Modules/MenuManager/src/MenuHandler.cs:28
- Generated: false

Inheritance: object → System.ValueType → **BuiltMenuItem**

#### Constructors
- `Sharp.Modules.MenuManager.Core.BuiltMenuItem.BuiltMenuItem(string Title, Sharp.Modules.MenuManager.Shared.MenuItemState State, float Width, [System.Action<Sharp.Modules.MenuManager.Shared.IMenuController>? Action = null], [string? Color = null], [Sharp.Modules.MenuManager.Shared.MenuItemActionKind ActionKind = Sharp.Modules.MenuManager.Shared.MenuItemActionKind.None], [string? HintText = null])` [L:28]

#### Properties
- `Sharp.Modules.MenuManager.Shared.MenuItemActionKind Sharp.Modules.MenuManager.Core.BuiltMenuItem.ActionKind` [L:34]
- `Sharp.Modules.MenuManager.Shared.MenuItemState Sharp.Modules.MenuManager.Core.BuiltMenuItem.State` [L:30]
- `System.Action<Sharp.Modules.MenuManager.Shared.IMenuController>? Sharp.Modules.MenuManager.Core.BuiltMenuItem.Action` [L:32]
- `float Sharp.Modules.MenuManager.Core.BuiltMenuItem.Width` [L:31]
- `string Sharp.Modules.MenuManager.Core.BuiltMenuItem.Title` [L:29]
- `string? Sharp.Modules.MenuManager.Core.BuiltMenuItem.Color` [L:33]
- `string? Sharp.Modules.MenuManager.Core.BuiltMenuItem.HintText` [L:35]


### record struct PreviousMenu : System.ValueType, System.IEquatable<Sharp.Modules.MenuManager.Core.PreviousMenu>

- FullName: `Sharp.Modules.MenuManager.Core.PreviousMenu`
- Kind: record struct
- Modifiers: public, readonly
- Source: Sharp.Modules/MenuManager/src/MenuHandler.cs:26
- Generated: false

Inheritance: object → System.ValueType → **PreviousMenu**

#### Constructors
- `Sharp.Modules.MenuManager.Core.PreviousMenu.PreviousMenu(System.Func<Sharp.Shared.Objects.IGameClient, Sharp.Modules.MenuManager.Shared.Menu> MenuFactory, Sharp.Modules.MenuManager.Shared.Menu Menu, int Page, int Cursor)` [L:26]

#### Properties
- `Sharp.Modules.MenuManager.Shared.Menu Sharp.Modules.MenuManager.Core.PreviousMenu.Menu` [L:26]
- `System.Func<Sharp.Shared.Objects.IGameClient, Sharp.Modules.MenuManager.Shared.Menu> Sharp.Modules.MenuManager.Core.PreviousMenu.MenuFactory` [L:26]
- `int Sharp.Modules.MenuManager.Core.PreviousMenu.Cursor` [L:26]
- `int Sharp.Modules.MenuManager.Core.PreviousMenu.Page` [L:26]


