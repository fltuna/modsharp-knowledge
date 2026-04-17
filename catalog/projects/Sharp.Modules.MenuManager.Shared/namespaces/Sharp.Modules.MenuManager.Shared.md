# Sharp.Modules.MenuManager.Shared

Project: Sharp.Modules.MenuManager.Shared
Types: 9 (0 generated)

### interface IMenuController : System.IDisposable

- FullName: `Sharp.Modules.MenuManager.Shared.IMenuController`
- Kind: interface
- Modifiers: public
- Source: Sharp.Modules/MenuManager/Shared/IMenuController.cs:25
- Generated: false

#### Properties
- `Sharp.Modules.MenuManager.Shared.Menu Sharp.Modules.MenuManager.Shared.IMenuController.Menu` [L:27]
  - Modifiers: public, abstract, readonly
- `Sharp.Shared.Objects.IGameClient Sharp.Modules.MenuManager.Shared.IMenuController.Client` [L:31]
  - Modifiers: public, abstract, readonly

#### Methods
- `void Sharp.Modules.MenuManager.Shared.IMenuController.Exit()` [L:37]
  - Modifiers: public, abstract
- `void Sharp.Modules.MenuManager.Shared.IMenuController.GoBack()` [L:39]
  - Modifiers: public, abstract
- `void Sharp.Modules.MenuManager.Shared.IMenuController.Next(Sharp.Modules.MenuManager.Shared.Menu menu)` [L:33]
  - Modifiers: public, abstract
- `void Sharp.Modules.MenuManager.Shared.IMenuController.Next(System.Func<Sharp.Shared.Objects.IGameClient, Sharp.Modules.MenuManager.Shared.Menu> menuFactory)` [L:35]
  - Modifiers: public, abstract
- `void Sharp.Modules.MenuManager.Shared.IMenuController.Refresh()` [L:29]
  - Modifiers: public, abstract


### interface IMenuManager

- FullName: `Sharp.Modules.MenuManager.Shared.IMenuManager`
- Kind: interface
- Modifiers: public
- Source: Sharp.Modules/MenuManager/Shared/IMenuManager.cs:24
- Generated: false

#### Fields
- `const string Sharp.Modules.MenuManager.Shared.IMenuManager.Identity = "IMenuManager"` [L:26]
  - Modifiers: public, static, const

#### Methods
- `bool Sharp.Modules.MenuManager.Shared.IMenuManager.IsInCurrentMenu(Sharp.Shared.Objects.IGameClient client, Sharp.Modules.MenuManager.Shared.Menu menuInstance)` [L:53]
  - Modifiers: public, abstract
  - Summary: Returns whether the current top menu is the specified menu instance.
- `bool Sharp.Modules.MenuManager.Shared.IMenuManager.IsInMenu(Sharp.Shared.Objects.IGameClient client)` [L:37]
  - Modifiers: public, abstract
  - Summary: Returns whether the client currently has an active menu session.
- `bool Sharp.Modules.MenuManager.Shared.IMenuManager.IsInMenu(Sharp.Shared.Objects.IGameClient client, Sharp.Modules.MenuManager.Shared.Menu menuInstance)` [L:43]
  - Modifiers: public, abstract
  - Summary: Returns whether the client is currently in the specified menu instance,
- `bool Sharp.Modules.MenuManager.Shared.IMenuManager.IsInMenu(Sharp.Shared.Objects.IGameClient client, ulong sessionId)` [L:48]
  - Modifiers: public, abstract
  - Summary: Returns whether the client is currently in the specified menu session.
- `bool Sharp.Modules.MenuManager.Shared.IMenuManager.TryGetCurrentMenuSessionId(Sharp.Shared.Objects.IGameClient client, out ulong sessionId)` [L:58]
  - Modifiers: public, abstract
  - Summary: Returns the current menu session identifier when the client is in a menu.
- `void Sharp.Modules.MenuManager.Shared.IMenuManager.DisplayMenu(Sharp.Shared.Objects.IGameClient client, Sharp.Modules.MenuManager.Shared.Menu menu)` [L:28]
  - Modifiers: public, abstract
- `void Sharp.Modules.MenuManager.Shared.IMenuManager.DisplayMenu(Sharp.Shared.Objects.IGameClient client, Sharp.Modules.MenuManager.Shared.Menu menu, out ulong sessionId)` [L:30]
  - Modifiers: public, abstract
- `void Sharp.Modules.MenuManager.Shared.IMenuManager.QuitMenu(Sharp.Shared.Objects.IGameClient client)` [L:32]
  - Modifiers: public, abstract


### class Menu

- FullName: `Sharp.Modules.MenuManager.Shared.Menu`
- Kind: class
- Modifiers: public
- Source: Sharp.Modules/MenuManager/Shared/Menu.cs:38
- Generated: false
- Summary: Represents a menu that can be displayed to a game client.

Inheritance: object → **Menu**

#### Fields
- `System.Action<Sharp.Shared.Objects.IGameClient>? Sharp.Modules.MenuManager.Shared.Menu.OnEnter` [L:89]
  - Summary: Invoked when the menu is first displayed or navigated into.
- `System.Action<Sharp.Shared.Objects.IGameClient>? Sharp.Modules.MenuManager.Shared.Menu.OnExit` [L:84]
  - Summary: Invoked when the menu is closed or navigated away from.

#### Properties
- `System.Collections.Generic.IReadOnlyList<Sharp.Modules.MenuManager.Shared.MenuItem> Sharp.Modules.MenuManager.Shared.Menu.Items` [L:45]
  - Modifiers: public, readonly
  - Summary: Gets the list of menu items.
- `bool Sharp.Modules.MenuManager.Shared.Menu.IsPlayerMovementEnabled` [L:71]
  - Summary: Gets whether the player is allowed to move while the menu is open.
- `bool Sharp.Modules.MenuManager.Shared.Menu.ShowIndex` [L:66]
  - Summary: Gets whether item indices (e.g. "1.", "2.") are displayed before item titles.
- `string Sharp.Modules.MenuManager.Shared.Menu.CursorLeft` [L:56]
  - Summary: Gets the left cursor indicator shown on the currently selected item.
- `string Sharp.Modules.MenuManager.Shared.Menu.CursorRight` [L:61]
  - Summary: Gets the right cursor indicator shown on the currently selected item.

#### Methods
- `System.ReadOnlySpan<Sharp.Modules.MenuManager.Shared.MenuItem> Sharp.Modules.MenuManager.Shared.Menu.GetItemSpan()` [L:50]
  - Summary: Gets the item span backed by the internal list, avoiding allocation.
- `static Sharp.Modules.MenuManager.Shared.Menu.Builder Sharp.Modules.MenuManager.Shared.Menu.Create()` [L:345]
  - Modifiers: public, static
  - Summary: Creates a new  for fluent menu construction.
- `string Sharp.Modules.MenuManager.Shared.Menu.BuildTitle(Sharp.Shared.Objects.IGameClient player)` [L:132]
  - Summary: Builds the menu title for the specified player.
- `void Sharp.Modules.MenuManager.Shared.Menu.AddBackItem(System.Func<Sharp.Shared.Objects.IGameClient, string> titleFactory)` [L:292]
  - Summary: Adds an item with a per-client dynamic title that navigates back to the previous menu when selected.
- `void Sharp.Modules.MenuManager.Shared.Menu.AddBackItem([string name = "Back"])` [L:275]
  - Summary: Adds an item that navigates back to the previous menu when selected.
- `void Sharp.Modules.MenuManager.Shared.Menu.AddDisabledItem(System.Func<Sharp.Shared.Objects.IGameClient, string> titleFactory)` [L:220]
  - Summary: Adds a disabled item with a per-client dynamic title. Disabled items are visible but not selectable.
- `void Sharp.Modules.MenuManager.Shared.Menu.AddDisabledItem(string name)` [L:205]
  - Summary: Adds a disabled item with a static title. Disabled items are visible but not selectable.
- `void Sharp.Modules.MenuManager.Shared.Menu.AddExitItem(System.Func<Sharp.Shared.Objects.IGameClient, string> titleFactory)` [L:321]
  - Summary: Adds an item with a per-client dynamic title that closes the menu when selected.
- `void Sharp.Modules.MenuManager.Shared.Menu.AddExitItem([string name = "Exit"])` [L:305]
  - Summary: Adds an item that closes the menu when selected.
- `void Sharp.Modules.MenuManager.Shared.Menu.AddItem(Sharp.Modules.MenuManager.Shared.MenuItemGenerator generator)` [L:178]
  - Summary: Adds a menu item using a raw  for full control over the item context.
- `void Sharp.Modules.MenuManager.Shared.Menu.AddItem(Sharp.Modules.MenuManager.Shared.MenuItemGenerator generator, System.Action<Sharp.Modules.MenuManager.Shared.IMenuController>? action)` [L:187]
  - Summary: Adds a menu item using a raw  with a fallback action.
- `void Sharp.Modules.MenuManager.Shared.Menu.AddItem(System.Func<Sharp.Shared.Objects.IGameClient, string> titleFactory, [System.Action<Sharp.Modules.MenuManager.Shared.IMenuController>? action = null])` [L:166]
  - Summary: Adds a menu item with a per-client dynamic title.
- `void Sharp.Modules.MenuManager.Shared.Menu.AddItem(string name, [System.Action<Sharp.Modules.MenuManager.Shared.IMenuController>? action = null])` [L:149]
  - Summary: Adds a menu item with a static title.
- `void Sharp.Modules.MenuManager.Shared.Menu.AddItems(System.Collections.Generic.IEnumerable<Sharp.Modules.MenuManager.Shared.MenuItem> items)` [L:139]
  - Summary: Adds multiple pre-constructed menu items.
- `void Sharp.Modules.MenuManager.Shared.Menu.AddSpacer()` [L:197]
  - Summary: Adds a spacer item that renders as an empty line. Spacers are not selectable.
- `void Sharp.Modules.MenuManager.Shared.Menu.AddSubMenu(System.Func<Sharp.Shared.Objects.IGameClient, string> titleFactory, Sharp.Modules.MenuManager.Shared.Menu subMenu)` [L:254]
  - Summary: Adds an item with a per-client dynamic title that navigates to a sub-menu when selected.
- `void Sharp.Modules.MenuManager.Shared.Menu.AddSubMenu(System.Func<Sharp.Shared.Objects.IGameClient, string> titleFactory, System.Func<Sharp.Shared.Objects.IGameClient, Sharp.Modules.MenuManager.Shared.Menu> menuFactory)` [L:266]
  - Summary: Adds an item with a per-client dynamic title that navigates to a dynamically created sub-menu when selected.
- `void Sharp.Modules.MenuManager.Shared.Menu.AddSubMenu(string name, Sharp.Modules.MenuManager.Shared.Menu subMenu)` [L:233]
  - Summary: Adds an item that navigates to a sub-menu when selected.
- `void Sharp.Modules.MenuManager.Shared.Menu.AddSubMenu(string name, System.Func<Sharp.Shared.Objects.IGameClient, Sharp.Modules.MenuManager.Shared.Menu> menuFactory)` [L:242]
  - Summary: Adds an item that navigates to a dynamically created sub-menu when selected.
- `void Sharp.Modules.MenuManager.Shared.Menu.DisablePlayerMovement()` [L:338]
  - Summary: Disables player movement while this menu is open.
- `void Sharp.Modules.MenuManager.Shared.Menu.EnablePlayerMovement()` [L:332]
  - Summary: Enables player movement while this menu is open.
- `void Sharp.Modules.MenuManager.Shared.Menu.SetCursor(string left, string right)` [L:106]
  - Summary: Sets the cursor indicators displayed around the currently selected item.
- `void Sharp.Modules.MenuManager.Shared.Menu.SetPlayerMovement(bool enabled)` [L:76]
  - Summary: Sets whether the player is allowed to move while the menu is open.
- `void Sharp.Modules.MenuManager.Shared.Menu.SetShowIndex(bool show)` [L:116]
  - Summary: Sets whether item indices are displayed.
- `void Sharp.Modules.MenuManager.Shared.Menu.SetTitle(System.Func<Sharp.Shared.Objects.IGameClient, string> factory)` [L:124]
  - Summary: Sets a per-client title factory that resolves the menu title at display time.
- `void Sharp.Modules.MenuManager.Shared.Menu.SetTitle(string name)` [L:96]
  - Summary: Sets a static menu title.


### class Builder

- FullName: `Sharp.Modules.MenuManager.Shared.Menu.Builder`
- Kind: class
- Modifiers: public
- Source: Sharp.Modules/MenuManager/Shared/Menu.cs:351
- Generated: false
- Summary: Fluent builder for constructing  instances.

Inheritance: object → **Builder**

#### Methods
- `Sharp.Modules.MenuManager.Shared.Menu Sharp.Modules.MenuManager.Shared.Menu.Builder.Build()` [L:359]
  - Summary: Finalizes and returns the constructed menu.
- `Sharp.Modules.MenuManager.Shared.Menu.Builder Sharp.Modules.MenuManager.Shared.Menu.Builder.BackItem(System.Func<Sharp.Shared.Objects.IGameClient, string> titleFactory)` [L:467]
- `Sharp.Modules.MenuManager.Shared.Menu.Builder Sharp.Modules.MenuManager.Shared.Menu.Builder.BackItem([string name = "Back"])` [L:459]
- `Sharp.Modules.MenuManager.Shared.Menu.Builder Sharp.Modules.MenuManager.Shared.Menu.Builder.Cursor(string left, string right)` [L:507]
- `Sharp.Modules.MenuManager.Shared.Menu.Builder Sharp.Modules.MenuManager.Shared.Menu.Builder.DisablePlayerMovement()` [L:533]
- `Sharp.Modules.MenuManager.Shared.Menu.Builder Sharp.Modules.MenuManager.Shared.Menu.Builder.DisabledItem(System.Func<Sharp.Shared.Objects.IGameClient, string> titleFactory)` [L:419]
- `Sharp.Modules.MenuManager.Shared.Menu.Builder Sharp.Modules.MenuManager.Shared.Menu.Builder.DisabledItem(string name)` [L:411]
- `Sharp.Modules.MenuManager.Shared.Menu.Builder Sharp.Modules.MenuManager.Shared.Menu.Builder.EnablePlayerMovement()` [L:525]
- `Sharp.Modules.MenuManager.Shared.Menu.Builder Sharp.Modules.MenuManager.Shared.Menu.Builder.ExitItem(System.Func<Sharp.Shared.Objects.IGameClient, string> titleFactory)` [L:483]
- `Sharp.Modules.MenuManager.Shared.Menu.Builder Sharp.Modules.MenuManager.Shared.Menu.Builder.ExitItem([string name = "Exit"])` [L:475]
- `Sharp.Modules.MenuManager.Shared.Menu.Builder Sharp.Modules.MenuManager.Shared.Menu.Builder.HideIndex()` [L:517]
  - Summary: Hides item indices from the menu display.
- `Sharp.Modules.MenuManager.Shared.Menu.Builder Sharp.Modules.MenuManager.Shared.Menu.Builder.Item(Sharp.Modules.MenuManager.Shared.MenuItemGenerator generator)` [L:387]
- `Sharp.Modules.MenuManager.Shared.Menu.Builder Sharp.Modules.MenuManager.Shared.Menu.Builder.Item(Sharp.Modules.MenuManager.Shared.MenuItemGenerator generator, System.Action<Sharp.Modules.MenuManager.Shared.IMenuController>? action)` [L:395]
- `Sharp.Modules.MenuManager.Shared.Menu.Builder Sharp.Modules.MenuManager.Shared.Menu.Builder.Item(System.Func<Sharp.Shared.Objects.IGameClient, string> titleFactory, [System.Action<Sharp.Modules.MenuManager.Shared.IMenuController>? action = null])` [L:379]
- `Sharp.Modules.MenuManager.Shared.Menu.Builder Sharp.Modules.MenuManager.Shared.Menu.Builder.Item(string name, [System.Action<Sharp.Modules.MenuManager.Shared.IMenuController>? action = null])` [L:371]
- `Sharp.Modules.MenuManager.Shared.Menu.Builder Sharp.Modules.MenuManager.Shared.Menu.Builder.Items(System.Collections.Generic.IEnumerable<Sharp.Modules.MenuManager.Shared.MenuItem> items)` [L:363]
- `Sharp.Modules.MenuManager.Shared.Menu.Builder Sharp.Modules.MenuManager.Shared.Menu.Builder.OnEnter(System.Action<Sharp.Shared.Objects.IGameClient> fn)` [L:555]
  - Summary: Sets a callback invoked when the menu is first displayed or navigated into.
- `Sharp.Modules.MenuManager.Shared.Menu.Builder Sharp.Modules.MenuManager.Shared.Menu.Builder.OnExit(System.Action<Sharp.Shared.Objects.IGameClient> fn)` [L:544]
  - Summary: Sets a callback invoked when the menu is closed or navigated away from.
- `Sharp.Modules.MenuManager.Shared.Menu.Builder Sharp.Modules.MenuManager.Shared.Menu.Builder.Spacer()` [L:403]
- `Sharp.Modules.MenuManager.Shared.Menu.Builder Sharp.Modules.MenuManager.Shared.Menu.Builder.SubMenu(System.Func<Sharp.Shared.Objects.IGameClient, string> titleFactory, Sharp.Modules.MenuManager.Shared.Menu subMenu)` [L:443]
- `Sharp.Modules.MenuManager.Shared.Menu.Builder Sharp.Modules.MenuManager.Shared.Menu.Builder.SubMenu(System.Func<Sharp.Shared.Objects.IGameClient, string> titleFactory, System.Func<Sharp.Shared.Objects.IGameClient, Sharp.Modules.MenuManager.Shared.Menu> menuFactory)` [L:451]
- `Sharp.Modules.MenuManager.Shared.Menu.Builder Sharp.Modules.MenuManager.Shared.Menu.Builder.SubMenu(string name, Sharp.Modules.MenuManager.Shared.Menu subMenu)` [L:427]
- `Sharp.Modules.MenuManager.Shared.Menu.Builder Sharp.Modules.MenuManager.Shared.Menu.Builder.SubMenu(string name, System.Func<Sharp.Shared.Objects.IGameClient, Sharp.Modules.MenuManager.Shared.Menu> menuFactory)` [L:435]
- `Sharp.Modules.MenuManager.Shared.Menu.Builder Sharp.Modules.MenuManager.Shared.Menu.Builder.Title(System.Func<Sharp.Shared.Objects.IGameClient, string> factory)` [L:499]
- `Sharp.Modules.MenuManager.Shared.Menu.Builder Sharp.Modules.MenuManager.Shared.Menu.Builder.Title(string name)` [L:491]


### record struct MenuItem : System.ValueType, System.IEquatable<Sharp.Modules.MenuManager.Shared.MenuItem>

- FullName: `Sharp.Modules.MenuManager.Shared.MenuItem`
- Kind: record struct
- Modifiers: public, readonly
- Source: Sharp.Modules/MenuManager/Shared/Menu.cs:571
- Generated: false
- Summary: Represents a single menu item backed by an optional .

Inheritance: object → System.ValueType → **MenuItem**

#### Constructors
- `Sharp.Modules.MenuManager.Shared.MenuItem.MenuItem([Sharp.Modules.MenuManager.Shared.MenuItemGenerator? Generator = null])` [L:571]
  - Summary: Represents a single menu item backed by an optional .

#### Properties
- `Sharp.Modules.MenuManager.Shared.MenuItemGenerator? Sharp.Modules.MenuManager.Shared.MenuItem.Generator` [L:571]
  - Summary: The generator delegate invoked per-client to populate the item context.


### enum MenuItemActionKind : System.Enum

- FullName: `Sharp.Modules.MenuManager.Shared.MenuItemActionKind`
- Kind: enum
- Modifiers: public
- Source: Sharp.Modules/MenuManager/Shared/Menu.cs:630
- Generated: false
- Summary: Semantic item action kind used by the menu renderer.

Inheritance: object → System.ValueType → System.Enum → **MenuItemActionKind**

#### Enum Members
- `Sharp.Modules.MenuManager.Shared.MenuItemActionKind.Back = 1` [L:633]
  - Modifiers: public, static, const
- `Sharp.Modules.MenuManager.Shared.MenuItemActionKind.Exit = 2` [L:634]
  - Modifiers: public, static, const
- `Sharp.Modules.MenuManager.Shared.MenuItemActionKind.None = 0` [L:632]
  - Modifiers: public, static, const


### record struct MenuItemContext : System.ValueType, System.IEquatable<Sharp.Modules.MenuManager.Shared.MenuItemContext>

- FullName: `Sharp.Modules.MenuManager.Shared.MenuItemContext`
- Kind: record struct
- Modifiers: public
- Source: Sharp.Modules/MenuManager/Shared/Menu.cs:586
- Generated: false
- Summary: Mutable context populated by a  during menu building.

Inheritance: object → System.ValueType → **MenuItemContext**

#### Fields
- `Sharp.Modules.MenuManager.Shared.MenuItemActionKind Sharp.Modules.MenuManager.Shared.MenuItemContext.ActionKind` [L:617]
  - Summary: Semantic action kind used by built-in navigation helpers.
- `Sharp.Modules.MenuManager.Shared.MenuItemState Sharp.Modules.MenuManager.Shared.MenuItemContext.State` [L:599]
  - Summary: The item state. Defaults to .
- `System.Action<Sharp.Modules.MenuManager.Shared.IMenuController>? Sharp.Modules.MenuManager.Shared.MenuItemContext.Action` [L:611]
  - Summary: The action invoked when the player selects this item.
- `string? Sharp.Modules.MenuManager.Shared.MenuItemContext.Color` [L:604]
  - Summary: Optional HTML color override for the item title (e.g. "#FFCCCB"). Does not apply to disabled items.
- `string? Sharp.Modules.MenuManager.Shared.MenuItemContext.HintText` [L:624]
  - Summary: Optional custom hint text displayed at the bottom of the menu when this item is selected.
- `string? Sharp.Modules.MenuManager.Shared.MenuItemContext.Title` [L:593]
  - Summary: The display title. If null or whitespace after generation, the item is skipped.


### delegate MenuItemGenerator : System.MulticastDelegate

- FullName: `Sharp.Modules.MenuManager.Shared.MenuItemGenerator`
- Kind: delegate
- Modifiers: public, sealed
- Source: Sharp.Modules/MenuManager/Shared/Menu.cs:581
- Generated: false
- Summary: Delegate invoked per-client to populate a .
- Invoke: `virtual void Sharp.Modules.MenuManager.Shared.MenuItemGenerator.Invoke(Sharp.Shared.Objects.IGameClient client, ref Sharp.Modules.MenuManager.Shared.MenuItemContext context)`

Inheritance: object → System.Delegate → System.MulticastDelegate → **MenuItemGenerator**


### enum MenuItemState : System.Enum

- FullName: `Sharp.Modules.MenuManager.Shared.MenuItemState`
- Kind: enum
- Modifiers: public
- Source: Sharp.Modules/MenuManager/Shared/MenuItemState.cs:22
- Generated: false

Inheritance: object → System.ValueType → System.Enum → **MenuItemState**

#### Enum Members
- `Sharp.Modules.MenuManager.Shared.MenuItemState.Default = 0` [L:24]
  - Modifiers: public, static, const
- `Sharp.Modules.MenuManager.Shared.MenuItemState.Disabled = 1` [L:25]
  - Modifiers: public, static, const
- `Sharp.Modules.MenuManager.Shared.MenuItemState.Ignore = 3` [L:27]
  - Modifiers: public, static, const
- `Sharp.Modules.MenuManager.Shared.MenuItemState.Spacer = 2` [L:26]
  - Modifiers: public, static, const


