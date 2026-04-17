# Sharp.Shared.Listeners

Project: Sharp.Shared
Types: 5 (0 generated)

### interface IClientListener

- FullName: `Sharp.Shared.Listeners.IClientListener`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/Listeners/ClientListener.cs:25
- Generated: false

#### Fields
- `const int Sharp.Shared.Listeners.IClientListener.ApiVersion = 1` [L:27]
  - Modifiers: public, static, const

#### Properties
- `int Sharp.Shared.Listeners.IClientListener.ListenerPriority` [L:37]
  - Modifiers: public, abstract, readonly
  - Summary: Priority
- `int Sharp.Shared.Listeners.IClientListener.ListenerVersion` [L:32]
  - Modifiers: public, abstract, readonly
  - Summary: Listenver version

#### Methods
- `Sharp.Shared.Enums.ECommandAction Sharp.Shared.Listeners.IClientListener.OnClientSayCommand(Sharp.Shared.Objects.IGameClient client, bool teamOnly, bool isCommand, string commandName, string message)` [L:83]
  - Modifiers: public, virtual
- `bool Sharp.Shared.Listeners.IClientListener.OnClientPreAdminCheck(Sharp.Shared.Objects.IGameClient client)` [L:43]
  - Modifiers: public, virtual
  - Summary: Is allowed to check for Admin
- `void Sharp.Shared.Listeners.IClientListener.OnAdminCacheReload()` [L:86]
  - Modifiers: public, virtual
- `void Sharp.Shared.Listeners.IClientListener.OnClientConnected(Sharp.Shared.Objects.IGameClient client)` [L:46]
  - Modifiers: public, virtual
- `void Sharp.Shared.Listeners.IClientListener.OnClientDisconnected(Sharp.Shared.Objects.IGameClient client, Sharp.Shared.Enums.NetworkDisconnectionReason reason)` [L:62]
  - Modifiers: public, virtual
- `void Sharp.Shared.Listeners.IClientListener.OnClientDisconnecting(Sharp.Shared.Objects.IGameClient client, Sharp.Shared.Enums.NetworkDisconnectionReason reason)` [L:58]
  - Modifiers: public, virtual
- `void Sharp.Shared.Listeners.IClientListener.OnClientPostAdminCheck(Sharp.Shared.Objects.IGameClient client)` [L:54]
  - Modifiers: public, virtual
- `void Sharp.Shared.Listeners.IClientListener.OnClientPutInServer(Sharp.Shared.Objects.IGameClient client)` [L:50]
  - Modifiers: public, virtual
- `void Sharp.Shared.Listeners.IClientListener.OnClientSettingChanged(Sharp.Shared.Objects.IGameClient client)` [L:79]
  - Modifiers: public, virtual
  - Summary: Called when a client changes a ConVar in  that has the


### interface IEntityListener

- FullName: `Sharp.Shared.Listeners.IEntityListener`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/Listeners/EntityListener.cs:26
- Generated: false

#### Fields
- `const int Sharp.Shared.Listeners.IEntityListener.ApiVersion = 1` [L:28]
  - Modifiers: public, static, const

#### Properties
- `int Sharp.Shared.Listeners.IEntityListener.ListenerPriority` [L:38]
  - Modifiers: public, abstract, readonly
  - Summary: Priority
- `int Sharp.Shared.Listeners.IEntityListener.ListenerVersion` [L:33]
  - Modifiers: public, abstract, readonly
  - Summary: Listenver version

#### Methods
- `Sharp.Shared.Enums.EHookAction Sharp.Shared.Listeners.IEntityListener.OnEntityAcceptInput(Sharp.Shared.GameEntities.IBaseEntity entity, string input, in Sharp.Shared.Types.EntityVariant value, Sharp.Shared.GameEntities.IBaseEntity? activator, Sharp.Shared.GameEntities.IBaseEntity? caller)` [L:59]
  - Modifiers: public, virtual
- `Sharp.Shared.Enums.EHookAction Sharp.Shared.Listeners.IEntityListener.OnEntityFireOutput(Sharp.Shared.GameEntities.IBaseEntity entity, string output, Sharp.Shared.GameEntities.IBaseEntity? activator, float delay)` [L:56]
  - Modifiers: public, virtual
- `void Sharp.Shared.Listeners.IEntityListener.OnEntityCreated(Sharp.Shared.GameEntities.IBaseEntity entity)` [L:40]
  - Modifiers: public, virtual
- `void Sharp.Shared.Listeners.IEntityListener.OnEntityDeleted(Sharp.Shared.GameEntities.IBaseEntity entity)` [L:44]
  - Modifiers: public, virtual
- `void Sharp.Shared.Listeners.IEntityListener.OnEntityFollowed(Sharp.Shared.GameEntities.IBaseEntity entity, Sharp.Shared.GameEntities.IBaseEntity? owner)` [L:52]
  - Modifiers: public, virtual
- `void Sharp.Shared.Listeners.IEntityListener.OnEntitySpawned(Sharp.Shared.GameEntities.IBaseEntity entity)` [L:48]
  - Modifiers: public, virtual


### interface IEventListener

- FullName: `Sharp.Shared.Listeners.IEventListener`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/Listeners/EventListener.cs:24
- Generated: false

#### Fields
- `const int Sharp.Shared.Listeners.IEventListener.ApiVersion = 1` [L:26]
  - Modifiers: public, static, const

#### Properties
- `int Sharp.Shared.Listeners.IEventListener.ListenerPriority` [L:36]
  - Modifiers: public, abstract, readonly
  - Summary: Priority
- `int Sharp.Shared.Listeners.IEventListener.ListenerVersion` [L:31]
  - Modifiers: public, abstract, readonly
  - Summary: Listenver version

#### Methods
- `bool Sharp.Shared.Listeners.IEventListener.HookFireEvent(Sharp.Shared.Objects.IGameEvent @event, ref bool serverOnly)` [L:42]
  - Modifiers: public, virtual
  - Summary: Hook and modify event, if you only need to listen, do not implement this function
- `void Sharp.Shared.Listeners.IEventListener.FireGameEvent(Sharp.Shared.Objects.IGameEvent @event)` [L:49]
  - Modifiers: public, abstract
  - Summary: Event listener, do not modify event here


### interface IGameListener

- FullName: `Sharp.Shared.Listeners.IGameListener`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/Listeners/GameListener.cs:24
- Generated: false

#### Fields
- `const int Sharp.Shared.Listeners.IGameListener.ApiVersion = 1` [L:26]
  - Modifiers: public, static, const

#### Properties
- `int Sharp.Shared.Listeners.IGameListener.ListenerPriority` [L:36]
  - Modifiers: public, abstract, readonly
  - Summary: Priority
- `int Sharp.Shared.Listeners.IGameListener.ListenerVersion` [L:31]
  - Modifiers: public, abstract, readonly
  - Summary: Listenver version

#### Methods
- `Sharp.Shared.Enums.ECommandAction Sharp.Shared.Listeners.IGameListener.ConsoleSay(string message)` [L:89]
  - Modifiers: public, virtual
- `void Sharp.Shared.Listeners.IGameListener.OnGameActivate()` [L:62]
  - Modifiers: public, virtual
- `void Sharp.Shared.Listeners.IGameListener.OnGameDeactivate()` [L:66]
  - Modifiers: public, virtual
- `void Sharp.Shared.Listeners.IGameListener.OnGameInit()` [L:54]
  - Modifiers: public, virtual
- `void Sharp.Shared.Listeners.IGameListener.OnGamePostInit()` [L:58]
  - Modifiers: public, virtual
- `void Sharp.Shared.Listeners.IGameListener.OnGamePreShutdown()` [L:70]
  - Modifiers: public, virtual
- `void Sharp.Shared.Listeners.IGameListener.OnGameShutdown()` [L:77]
  - Modifiers: public, virtual
  - Summary: is not usable here!
- `void Sharp.Shared.Listeners.IGameListener.OnResourcePrecache()` [L:50]
  - Modifiers: public, virtual
- `void Sharp.Shared.Listeners.IGameListener.OnRoundRestart()` [L:81]
  - Modifiers: public, virtual
- `void Sharp.Shared.Listeners.IGameListener.OnRoundRestarted()` [L:85]
  - Modifiers: public, virtual
- `void Sharp.Shared.Listeners.IGameListener.OnServerActivate()` [L:46]
  - Modifiers: public, virtual
- `void Sharp.Shared.Listeners.IGameListener.OnServerInit()` [L:38]
  - Modifiers: public, virtual
- `void Sharp.Shared.Listeners.IGameListener.OnServerSpawn()` [L:42]
  - Modifiers: public, virtual


### interface ISteamListener

- FullName: `Sharp.Shared.Listeners.ISteamListener`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/Listeners/SteamListener.cs:25
- Generated: false

#### Fields
- `const int Sharp.Shared.Listeners.ISteamListener.ApiVersion = 2` [L:27]
  - Modifiers: public, static, const

#### Properties
- `int Sharp.Shared.Listeners.ISteamListener.ListenerPriority` [L:37]
  - Modifiers: public, abstract, readonly
  - Summary: Priority
- `int Sharp.Shared.Listeners.ISteamListener.ListenerVersion` [L:32]
  - Modifiers: public, abstract, readonly
  - Summary: Listenver version

#### Methods
- `void Sharp.Shared.Listeners.ISteamListener.OnDownloadItemResult(ulong sharedFileId, Sharp.Shared.Enums.SteamApiResult result)` [L:70]
  - Modifiers: public, virtual
  - Summary: UGC download
- `void Sharp.Shared.Listeners.ISteamListener.OnGroupStatusResult(Sharp.Shared.Units.SteamID steamId, Sharp.Shared.Units.SteamID groupId, bool isMember, bool isOfficer)` [L:42]
  - Modifiers: public, virtual
  - Summary: Triggered after calling RequestUserGroupStatus
- `void Sharp.Shared.Listeners.ISteamListener.OnItemInstalled(ulong publishedFileId)` [L:78]
  - Modifiers: public, virtual
  - Summary: UGC installation
- `void Sharp.Shared.Listeners.ISteamListener.OnSteamServersConnectFailure(Sharp.Shared.Enums.SteamApiResult reason, bool stillRetrying)` [L:63]
  - Modifiers: public, virtual
  - Summary: Server failed to connect to Steam
- `void Sharp.Shared.Listeners.ISteamListener.OnSteamServersConnected()` [L:49]
  - Modifiers: public, virtual
  - Summary: Server connected to Steam
- `void Sharp.Shared.Listeners.ISteamListener.OnSteamServersDisconnected(Sharp.Shared.Enums.SteamApiResult reason)` [L:56]
  - Modifiers: public, virtual
  - Summary: Server disconnected from Steam


