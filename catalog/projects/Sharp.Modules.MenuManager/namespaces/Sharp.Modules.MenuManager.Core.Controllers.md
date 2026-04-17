# Sharp.Modules.MenuManager.Core.Controllers

Project: Sharp.Modules.MenuManager
Types: 1 (0 generated)

### interface IInternalMenuController : Sharp.Modules.MenuManager.Shared.IMenuController

- FullName: `Sharp.Modules.MenuManager.Core.Controllers.IInternalMenuController`
- Kind: interface
- Modifiers: public
- Source: Sharp.Modules/MenuManager/src/Controllers/IInternalMenuController.cs:24
- Generated: false

#### Properties
- `ulong Sharp.Modules.MenuManager.Core.Controllers.IInternalMenuController.SessionId` [L:26]
  - Modifiers: public, abstract, readonly

#### Methods
- `bool Sharp.Modules.MenuManager.Core.Controllers.IInternalMenuController.IsInCurrentMenu(Sharp.Modules.MenuManager.Shared.Menu menuInstance)` [L:40]
  - Modifiers: public, abstract
- `bool Sharp.Modules.MenuManager.Core.Controllers.IInternalMenuController.IsInMenu(Sharp.Modules.MenuManager.Shared.Menu menuInstance)` [L:38]
  - Modifiers: public, abstract
- `bool Sharp.Modules.MenuManager.Core.Controllers.IInternalMenuController.MoveDownCursor()` [L:30]
  - Modifiers: public, abstract
- `bool Sharp.Modules.MenuManager.Core.Controllers.IInternalMenuController.MoveUpCursor()` [L:28]
  - Modifiers: public, abstract
- `void Sharp.Modules.MenuManager.Core.Controllers.IInternalMenuController.Confirm()` [L:32]
  - Modifiers: public, abstract
- `void Sharp.Modules.MenuManager.Core.Controllers.IInternalMenuController.GoToNextPage()` [L:36]
  - Modifiers: public, abstract
- `void Sharp.Modules.MenuManager.Core.Controllers.IInternalMenuController.GoToPreviousPage()` [L:34]
  - Modifiers: public, abstract


