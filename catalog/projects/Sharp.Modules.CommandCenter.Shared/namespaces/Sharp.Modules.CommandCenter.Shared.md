# Sharp.Modules.CommandCenter.Shared

Project: Sharp.Modules.CommandCenter.Shared
Types: 2 (0 generated)

### interface ICommandCenter

- FullName: `Sharp.Modules.CommandCenter.Shared.ICommandCenter`
- Kind: interface
- Modifiers: public
- Source: Sharp.Modules/CommandCenter/Shared/ICommandCenter.cs:22
- Generated: false

#### Fields
- `const string Sharp.Modules.CommandCenter.Shared.ICommandCenter.Identity = "ICommandCenter"` [L:24]
  - Modifiers: public, static, const

#### Methods
- `Sharp.Modules.CommandCenter.Shared.ICommandRegistry Sharp.Modules.CommandCenter.Shared.ICommandCenter.GetRegistry(string moduleIdentity)` [L:30]
  - Modifiers: public, abstract
  - Summary: Gets the command registry for the specified module identity.


### interface ICommandRegistry

- FullName: `Sharp.Modules.CommandCenter.Shared.ICommandRegistry`
- Kind: interface
- Modifiers: public
- Source: Sharp.Modules/CommandCenter/Shared/ICommandRegistry.cs:27
- Generated: false

#### Methods
- `void Sharp.Modules.CommandCenter.Shared.ICommandRegistry.AddCommandListener(string commandName, Sharp.Shared.Managers.IClientManager.DelegateClientCommand callback)` [L:89]
  - Modifiers: public, abstract
  - Summary: Adds a listener for a specific command.
- `void Sharp.Modules.CommandCenter.Shared.ICommandRegistry.RegisterClientCommand(string command, System.Action<Sharp.Shared.Objects.IGameClient, Sharp.Shared.Types.StringCommand> call)` [L:42]
  - Modifiers: public, abstract
  - Summary: Registers a client command.
- `void Sharp.Modules.CommandCenter.Shared.ICommandRegistry.RegisterConsoleCommand(string command, System.Action<Sharp.Shared.Objects.IGameClient?, Sharp.Shared.Types.StringCommand> callback, [bool addPrefix = true])` [L:81]
  - Modifiers: public, abstract
  - Summary: Registers a console command.
- `void Sharp.Modules.CommandCenter.Shared.ICommandRegistry.RegisterGenericCommand(string command, System.Action<Sharp.Shared.Objects.IGameClient?, Sharp.Shared.Types.StringCommand> call, [string description = ""])` [L:72]
  - Modifiers: public, abstract
  - Summary: Registers a "generic" command usable in in-game chat, client console, and server console.
- `void Sharp.Modules.CommandCenter.Shared.ICommandRegistry.RegisterServerCommand(string command, System.Action call, [string description = ""], [bool addPrefix = true])` [L:62]
  - Modifiers: public, abstract
  - Summary: Registers a server command.
- `void Sharp.Modules.CommandCenter.Shared.ICommandRegistry.RegisterServerCommand(string command, System.Action<Sharp.Shared.Types.StringCommand> call, [string description = ""], [bool addPrefix = true])` [L:52]
  - Modifiers: public, abstract
  - Summary: Registers a server command.


