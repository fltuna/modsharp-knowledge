# Sharp.Core.Bridges.Natives

Project: Sharp.Core
Types: 13 (0 generated)

### class Client

- FullName: `Sharp.Core.Bridges.Natives.Client`
- Kind: class
- Modifiers: public, static
- Source: Sharp.Core/Bridges/Natives/Client.cs:27
- Generated: false

Inheritance: object → **Client**

#### Methods
- `static float Sharp.Core.Bridges.Natives.Client.GetTimeConnected(Sharp.Shared.Objects.IGameClient ptr)` [L:37]
  - Modifiers: public, static
- `static nint Sharp.Core.Bridges.Natives.Client.GetClientBySlot(Sharp.Shared.Units.PlayerSlot slot)` [L:29]
  - Modifiers: public, static
- `static nint Sharp.Core.Bridges.Natives.Client.GetClientBySteamId(Sharp.Shared.Units.SteamID steamId)` [L:33]
  - Modifiers: public, static
- `static nint Sharp.Core.Bridges.Natives.Client.GetClientByUserId(Sharp.Shared.Units.UserID steamId)` [L:31]
  - Modifiers: public, static
- `static nint Sharp.Core.Bridges.Natives.Client.GetConVarValue(Sharp.Shared.Objects.IGameClient ptr, string name)` [L:53]
  - Modifiers: public, static
- `static string Sharp.Core.Bridges.Natives.Client.GetNetWorkAddress(Sharp.Shared.Objects.IGameClient client)` [L:35]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Client.AddCommandCallback(string command)` [L:45]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Client.AddCommandListener(string command)` [L:47]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Client.ClientCommand(Sharp.Shared.Objects.IGameClient ptr, string command)` [L:55]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Client.ConsolePrint(Sharp.Shared.Objects.IGameClient ptr, string message)` [L:39]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Client.ExecuteStringCommand(Sharp.Shared.Objects.IGameClient ptr, string command)` [L:59]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Client.FakeClientCommand(Sharp.Shared.Objects.IGameClient ptr, string command)` [L:57]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Client.KickClient(Sharp.Shared.Objects.IGameClient ptr, string internalReason, Sharp.Shared.Enums.NetworkDisconnectionReason networkDisconnectionReason)` [L:49]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Client.SayChatMessage(Sharp.Shared.Objects.IGameClient ptr, bool teamOnly, string message)` [L:43]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Client.SetName(Sharp.Shared.Objects.IGameClient ptr, string name)` [L:41]
  - Modifiers: public, static


### class Core

- FullName: `Sharp.Core.Bridges.Natives.Core`
- Kind: class
- Modifiers: public, static
- Source: Sharp.Core/Bridges/Natives/Core.cs:25
- Generated: false

Inheritance: object → **Core**

#### Methods
- `static bool Sharp.Core.Bridges.Natives.Core.SetMemoryAccess(nint address, long size, Sharp.Shared.Enums.MemoryAccess access, Sharp.Shared.Enums.MemoryAccess* originalAccess)` [L:71]
  - Modifiers: public, static
- `static double Sharp.Core.Bridges.Natives.Core.GetEngineTime()` [L:37]
  - Modifiers: public, static
- `static nint Sharp.Core.Bridges.Natives.Core.CreateInlineHook()` [L:53]
  - Modifiers: public, static
- `static nint Sharp.Core.Bridges.Natives.Core.CreateMidFuncHook()` [L:55]
  - Modifiers: public, static
- `static nint Sharp.Core.Bridges.Natives.Core.FindPattern(string module, string pattern)` [L:61]
  - Modifiers: public, static
- `static nint Sharp.Core.Bridges.Natives.Core.FindStringTable(string name)` [L:51]
  - Modifiers: public, static
- `static nint Sharp.Core.Bridges.Natives.Core.FindValveInterface(string module, string name)` [L:69]
  - Modifiers: public, static
- `static nint Sharp.Core.Bridges.Natives.Core.GetCoreBridge()` [L:29]
  - Modifiers: public, static
- `static nint Sharp.Core.Bridges.Natives.Core.GetGameData()` [L:49]
  - Modifiers: public, static
- `static nint Sharp.Core.Bridges.Natives.Core.GetGameDirectory()` [L:31]
  - Modifiers: public, static
- `static nint Sharp.Core.Bridges.Natives.Core.GetGameRules()` [L:39]
  - Modifiers: public, static
- `static nint Sharp.Core.Bridges.Natives.Core.GetGlobals()` [L:33]
  - Modifiers: public, static
- `static nint Sharp.Core.Bridges.Natives.Core.GetIServer()` [L:35]
  - Modifiers: public, static
- `static nint Sharp.Core.Bridges.Natives.Core.GetLibraryModule(string module)` [L:67]
  - Modifiers: public, static
- `static nint Sharp.Core.Bridges.Natives.Core.GetVTableByClass(string module, string className)` [L:63]
  - Modifiers: public, static
- `static nint Sharp.Core.Bridges.Natives.Core.InstallVirtualHook(nint vTable, int index, nint hook)` [L:65]
  - Modifiers: public, static
- `static string Sharp.Core.Bridges.Natives.Core.GetCommandLine()` [L:27]
  - Modifiers: public, static
- `static uint Sharp.Core.Bridges.Natives.Core.MakeStringToken(string str)` [L:75]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Core.FatalError(string message)` [L:41]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Core.LogColorText(byte r, byte g, byte b, string message)` [L:47]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Core.LogMessage(string message)` [L:45]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Core.LogWarning(string message)` [L:43]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Core.RejectConnection(nint pNetAdr, Sharp.Shared.Enums.NetworkDisconnectionReason reason)` [L:73]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Core.RemoveInlineHook(nint ptr)` [L:57]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Core.RemoveMidFuncHook(nint ptr)` [L:59]
  - Modifiers: public, static


### class Cvar

- FullName: `Sharp.Core.Bridges.Natives.Cvar`
- Kind: class
- Modifiers: public, static
- Source: Sharp.Core/Bridges/Natives/Cvar.cs:26
- Generated: false

Inheritance: object → **Cvar**

#### Methods
- `static bool Sharp.Core.Bridges.Natives.Cvar.InstallChangeHook(nint cvar)` [L:28]
  - Modifiers: public, static
- `static bool Sharp.Core.Bridges.Natives.Cvar.ReleaseCommand(string name)` [L:52]
  - Modifiers: public, static
- `static bool Sharp.Core.Bridges.Natives.Cvar.RemoveChangeHook(nint ptr)` [L:30]
  - Modifiers: public, static
- `static bool Sharp.Core.Bridges.Natives.Cvar.SetMaxBound(nint cvar, Sharp.Shared.Types.ConVarVariantValue* value)` [L:46]
  - Modifiers: public, static
- `static bool Sharp.Core.Bridges.Natives.Cvar.SetMinBound(nint cvar, Sharp.Shared.Types.ConVarVariantValue* value)` [L:44]
  - Modifiers: public, static
- `static long Sharp.Core.Bridges.Natives.Cvar.CreateCommand(string name, string helpString, Sharp.Shared.Enums.ConVarFlags flags)` [L:48]
  - Modifiers: public, static
- `static nint Sharp.Core.Bridges.Natives.Cvar.CreateConVar(string name, Sharp.Shared.Types.ConVarVariantValue* defaultValue, string helpString, Sharp.Shared.Enums.ConVarType type, Sharp.Shared.Enums.ConVarFlags flags, Sharp.Shared.Types.ConVarVariantValue?* min, Sharp.Shared.Types.ConVarVariantValue?* max)` [L:34]
  - Modifiers: public, static
- `static nint Sharp.Core.Bridges.Natives.Cvar.FindConVar(string name, bool useIterator)` [L:32]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Cvar.ReplicateToClient(nint cvar, string value, nint client)` [L:54]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Cvar.SetValue(nint cvar, Sharp.Shared.Types.ConVarVariantValue* value)` [L:42]
  - Modifiers: public, static


### class Econ

- FullName: `Sharp.Core.Bridges.Natives.Econ`
- Kind: class
- Modifiers: public, static
- Source: Sharp.Core/Bridges/Natives/Econ.cs:22
- Generated: false

Inheritance: object → **Econ**

#### Methods
- `static bool Sharp.Core.Bridges.Natives.Econ.UpdateItemAttributes(nint entity, uint accountId, string nameTag, int paint, int pattern, float wear, int nSticker1, float flSticker1, int nSticker2, float flSticker2, int nSticker3, float flSticker3, int nSticker4, float flSticker4)` [L:28]
  - Modifiers: public, static
- `static nint Sharp.Core.Bridges.Natives.Econ.GetItemDefinitions()` [L:24]
  - Modifiers: public, static
- `static nint Sharp.Core.Bridges.Natives.Econ.GetPaintKits()` [L:26]
  - Modifiers: public, static


### class Engine

- FullName: `Sharp.Core.Bridges.Natives.Engine`
- Kind: class
- Modifiers: public, static
- Source: Sharp.Core/Bridges/Natives/Engine.cs:22
- Generated: false

Inheritance: object → **Engine**

#### Methods
- `static bool Sharp.Core.Bridges.Natives.Engine.IsMapValid(string map)` [L:26]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Engine.ChangeLevel(string map)` [L:24]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Engine.PrecacheResource(nint pContext, string pszModel)` [L:30]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Engine.ServerCommand(string command)` [L:28]
  - Modifiers: public, static


### class Entity

- FullName: `Sharp.Core.Bridges.Natives.Entity`
- Kind: class
- Modifiers: public, static
- Source: Sharp.Core/Bridges/Natives/Entity.cs:27
- Generated: false

Inheritance: object → **Entity**

#### Methods
- `static Sharp.Shared.Types.Vector* Sharp.Core.Bridges.Natives.Entity.GetAbsAngles(nint entity)` [L:140]
  - Modifiers: public, static
- `static Sharp.Shared.Types.Vector* Sharp.Core.Bridges.Natives.Entity.GetAbsOrigin(nint entity)` [L:144]
  - Modifiers: public, static
- `static Sharp.Shared.Types.Vector* Sharp.Core.Bridges.Natives.Entity.GetAbsVelocity(nint entity)` [L:152]
  - Modifiers: public, static
- `static Sharp.Shared.Types.Vector* Sharp.Core.Bridges.Natives.Entity.GetCenter(nint entity)` [L:134]
  - Modifiers: public, static
- `static Sharp.Shared.Types.Vector* Sharp.Core.Bridges.Natives.Entity.GetEyeAngles(nint entity)` [L:136]
  - Modifiers: public, static
- `static Sharp.Shared.Types.Vector* Sharp.Core.Bridges.Natives.Entity.GetEyePosition(nint entity)` [L:138]
  - Modifiers: public, static
- `static Sharp.Shared.Types.Vector* Sharp.Core.Bridges.Natives.Entity.GetLocalVelocity(nint entity)` [L:148]
  - Modifiers: public, static
- `static bool Sharp.Core.Bridges.Natives.Entity.AcceptInput(nint entity, string input, nint activator, nint caller, string? value, int outputId)` [L:69]
  - Modifiers: public, static
- `static bool Sharp.Core.Bridges.Natives.Entity.AcceptInputFloat(nint entity, string input, nint activator, nint caller, float value, int outputId)` [L:83]
  - Modifiers: public, static
- `static bool Sharp.Core.Bridges.Natives.Entity.AcceptInputInt(nint entity, string input, nint activator, nint caller, int value, int outputId)` [L:76]
  - Modifiers: public, static
- `static bool Sharp.Core.Bridges.Natives.Entity.IsPlayerController(nint entity)` [L:180]
  - Modifiers: public, static
- `static bool Sharp.Core.Bridges.Natives.Entity.IsPlayerPawn(nint entity)` [L:182]
  - Modifiers: public, static
- `static bool Sharp.Core.Bridges.Natives.Entity.IsValid(uint eHandle)` [L:29]
  - Modifiers: public, static
- `static bool Sharp.Core.Bridges.Natives.Entity.IsWeapon(nint entity)` [L:178]
  - Modifiers: public, static
- `static int Sharp.Core.Bridges.Natives.Entity.LookupAttachment(nint entity, string attachment)` [L:160]
  - Modifiers: public, static
- `static int Sharp.Core.Bridges.Natives.Entity.LookupBone(nint entity, string bone)` [L:164]
  - Modifiers: public, static
- `static long Sharp.Core.Bridges.Natives.Entity.DispatchTraceAttack(nint entity, Sharp.Shared.Types.TakeDamageInfo* info, bool bypassHook)` [L:114]
  - Modifiers: public, static
- `static long Sharp.Core.Bridges.Natives.Entity.EmitSound(nint entity, string sound, float?* volume, Sharp.Shared.Types.RecipientFilter* filter)` [L:43]
  - Modifiers: public, static
- `static nint Sharp.Core.Bridges.Natives.Entity.AllocPooledString(string content)` [L:63]
  - Modifiers: public, static
- `static nint Sharp.Core.Bridges.Natives.Entity.CreateByName(string classname)` [L:61]
  - Modifiers: public, static
- `static nint Sharp.Core.Bridges.Natives.Entity.FindByClassname(nint start, string classname)` [L:51]
  - Modifiers: public, static
- `static nint Sharp.Core.Bridges.Natives.Entity.FindByEHandle(uint eHandle)` [L:47]
  - Modifiers: public, static
- `static nint Sharp.Core.Bridges.Natives.Entity.FindByIndex(int index)` [L:49]
  - Modifiers: public, static
- `static nint Sharp.Core.Bridges.Natives.Entity.FindByName(nint start, string name)` [L:53]
  - Modifiers: public, static
- `static nint Sharp.Core.Bridges.Natives.Entity.FindInSphere(nint start, Sharp.Shared.Types.Vector* center, float radius)` [L:55]
  - Modifiers: public, static
- `static nint Sharp.Core.Bridges.Natives.Entity.GetGlobalCStrikeTeam(Sharp.Shared.Enums.CStrikeTeam team)` [L:184]
  - Modifiers: public, static
- `static nint Sharp.Core.Bridges.Natives.Entity.SpawnEntitySync(string classname, Sharp.Core.Types.EntityKeyValuesVariant* lumps, int count)` [L:57]
  - Modifiers: public, static
- `static nint Sharp.Core.Bridges.Natives.Entity.WeaponFromEntity(nint entity)` [L:176]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Entity.AddIOEvent(nint entity, float delay, string input, nint activator, nint caller, string? value, int outputId)` [L:90]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Entity.AddIOEventFloat(nint entity, float delay, string input, nint activator, nint caller, float value, int outputId)` [L:106]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Entity.AddIOEventInt(nint entity, float delay, string input, nint activator, nint caller, int value, int outputId)` [L:98]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Entity.ApplyAbsVelocityImpulse(nint entity, Sharp.Shared.Types.Vector* vVelocity)` [L:132]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Entity.ChangeTeam(nint entity, Sharp.Shared.Enums.CStrikeTeam team)` [L:33]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Entity.CollisionRulesChanged(nint entity)` [L:41]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Entity.DispatchSpawn(nint entity, Sharp.Core.Types.EntityKeyValuesVariant* lumps, int count)` [L:186]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Entity.GetAttachment(nint entity, int attachment, out Sharp.Shared.Types.Vector vOrigin, out Sharp.Shared.Types.Vector vAngles)` [L:162]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Entity.GetBoneTransform(nint entity, int bone, out Sharp.Shared.Types.Matrix3x4 matrix)` [L:166]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Entity.HookInput(string classname, string input)` [L:67]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Entity.HookOutput(string classname, string output)` [L:65]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Entity.Kill(nint entity)` [L:31]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Entity.NetworkStateChanged(nint entity, ushort offset)` [L:35]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Entity.SetAbsAngles(nint entity, Sharp.Shared.Types.Vector* vAngles)` [L:142]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Entity.SetAbsOrigin(nint entity, Sharp.Shared.Types.Vector* vOrigin)` [L:146]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Entity.SetAbsVelocity(nint entity, Sharp.Shared.Types.Vector* vVelocity)` [L:154]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Entity.SetBodyGroupByName(nint entity, string name, int value)` [L:156]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Entity.SetCollisionBounds(nint entity, Sharp.Shared.Types.Vector* mins, Sharp.Shared.Types.Vector* maxs)` [L:170]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Entity.SetGravityScale(nint entity, float scale)` [L:130]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Entity.SetGroundEntity(nint entity, nint ground, nint unknown)` [L:122]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Entity.SetLocalVelocity(nint entity, Sharp.Shared.Types.Vector* vVelocity)` [L:150]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Entity.SetMaterialGroupMask(nint entity, ulong mask)` [L:158]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Entity.SetModel(nint entity, string model)` [L:118]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Entity.SetModelScale(nint entity, float scale)` [L:168]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Entity.SetMoveType(nint entity, Sharp.Shared.Enums.MoveType moveType)` [L:128]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Entity.SetName(nint entity, string name)` [L:116]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Entity.SetOwner(nint entity, nint owner)` [L:120]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Entity.SetSolid(nint entity, Sharp.Shared.Enums.SolidType solid)` [L:124]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Entity.SetStateChanged(nint entity, ushort offset)` [L:37]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Entity.SetStructStateChanged(nint entity, ushort offset)` [L:39]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Entity.StopSound(nint entity, string sound)` [L:45]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Entity.Teleport(nint entity, Sharp.Shared.Types.Vector?* vPosition, Sharp.Shared.Types.Vector?* vAngles, Sharp.Shared.Types.Vector?* vVelocity)` [L:126]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Entity.WeaponDeploy(nint weapon)` [L:174]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Entity.WeaponHolster(nint weapon)` [L:172]
  - Modifiers: public, static


### class Event

- FullName: `Sharp.Core.Bridges.Natives.Event`
- Kind: class
- Modifiers: public, static
- Source: Sharp.Core/Bridges/Natives/Event.cs:26
- Generated: false

Inheritance: object → **Event**

#### Methods
- `static bool Sharp.Core.Bridges.Natives.Event.FindListener(Sharp.Shared.Units.PlayerSlot slot, string name)` [L:42]
  - Modifiers: public, static
- `static float Sharp.Core.Bridges.Natives.Event.GetFloat(nint @event, string key, float defaultValue)` [L:56]
  - Modifiers: public, static
- `static int Sharp.Core.Bridges.Natives.Event.GetInt(nint @event, string key, int defaultValue)` [L:48]
  - Modifiers: public, static
- `static nint Sharp.Core.Bridges.Natives.Event.CloneEvent(nint @event)` [L:40]
  - Modifiers: public, static
- `static nint Sharp.Core.Bridges.Natives.Event.CreateEvent(string name, bool force)` [L:30]
  - Modifiers: public, static
- `static nint Sharp.Core.Bridges.Natives.Event.GetPlayerController(nint @event, string key)` [L:52]
  - Modifiers: public, static
- `static nint Sharp.Core.Bridges.Natives.Event.GetPlayerPawn(nint @event, string key)` [L:54]
  - Modifiers: public, static
- `static sbyte* Sharp.Core.Bridges.Natives.Event.GetName(nint @event)` [L:44]
  - Modifiers: public, static
- `static sbyte* Sharp.Core.Bridges.Natives.Event.GetString(nint @event, string key, string defaultValue)` [L:46]
  - Modifiers: public, static
- `static ulong Sharp.Core.Bridges.Natives.Event.GetUInt64(nint @event, string key, ulong defaultValue)` [L:50]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Event.FireEvent(nint @event, bool serverOnly)` [L:32]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Event.FireToClient(nint @event, int slot)` [L:34]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Event.FireToClients(nint @event)` [L:36]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Event.FreeEvent(nint @event)` [L:38]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Event.HookEvent(string name)` [L:28]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Event.SetFloat(nint @event, string key, float value)` [L:62]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Event.SetInt(nint @event, string key, int value)` [L:60]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Event.SetPlayerPawn(nint @event, string key, Sharp.Shared.GameEntities.IBaseEntity pawn)` [L:66]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Event.SetPlayerSlot(nint @event, string key, int slot)` [L:68]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Event.SetString(nint @event, string key, string value)` [L:58]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Event.SetUInt64(nint @event, string key, float value)` [L:64]
  - Modifiers: public, static


### class Game

- FullName: `Sharp.Core.Bridges.Natives.Game`
- Kind: class
- Modifiers: public, static
- Source: Sharp.Core/Bridges/Natives/Game.cs:28
- Generated: false

Inheritance: object → **Game**

#### Methods
- `static Sharp.Shared.Enums.ResourceStatus Sharp.Core.Bridges.Natives.Game.GetResourceStatus(string fileName)` [L:120]
  - Modifiers: public, static
- `static Sharp.Shared.Types.Runtime.NativeSpan<byte> Sharp.Core.Bridges.Natives.Game.FindResourceDataBlockInfo(string fileName, string pathId)` [L:118]
  - Modifiers: public, static
- `static bool Sharp.Core.Bridges.Natives.Game.AddWorkshopMap(ulong sharedFileId, string name, string path)` [L:134]
  - Modifiers: public, static
- `static bool Sharp.Core.Bridges.Natives.Game.RemoveWorkshopMap(ulong sharedFileId)` [L:138]
  - Modifiers: public, static
- `static bool Sharp.Core.Bridges.Natives.Game.WorkshopMapExists(ulong sharedFileId)` [L:136]
  - Modifiers: public, static
- `static int Sharp.Core.Bridges.Natives.Game.DispatchParticleEffectAttachment(string particle, Sharp.Shared.Enums.ParticleAttachmentType attachType, nint entity, byte attachmentIndex, bool resetEntity, Sharp.Shared.Types.RecipientFilter* filter)` [L:109]
  - Modifiers: public, static
- `static int Sharp.Core.Bridges.Natives.Game.DispatchParticleEffectEntityPosition(string particle, nint entity, Sharp.Shared.Types.Vector* origin, Sharp.Shared.Types.Vector* angles, bool resetEntity, Sharp.Shared.Types.RecipientFilter* filter)` [L:102]
  - Modifiers: public, static
- `static int Sharp.Core.Bridges.Natives.Game.DispatchParticleEffectPosition(string particle, Sharp.Shared.Types.Vector* origin, Sharp.Shared.Types.Vector* angles, Sharp.Shared.Types.RecipientFilter* filter)` [L:97]
  - Modifiers: public, static
- `static nint Sharp.Core.Bridges.Natives.Game.FindWeaponVDataByName(string name)` [L:128]
  - Modifiers: public, static
- `static nint Sharp.Core.Bridges.Natives.Game.GetAddonName()` [L:122]
  - Modifiers: public, static
- `static nint Sharp.Core.Bridges.Natives.Game.GetGameSystemFactory()` [L:126]
  - Modifiers: public, static
- `static nint Sharp.Core.Bridges.Natives.Game.GetMapGroupMapList(string mapGroup)` [L:116]
  - Modifiers: public, static
- `static nint Sharp.Core.Bridges.Natives.Game.GetMapName()` [L:124]
  - Modifiers: public, static
- `static nint Sharp.Core.Bridges.Natives.Game.ListWorkshopMaps()` [L:140]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Game.DualAddonOverrideCheck(ulong steamId, double time)` [L:132]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Game.DualAddonPurgeCheck()` [L:130]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Game.PrintChannelAll(Sharp.Shared.Enums.HudPrintChannel channel, string message)` [L:30]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Game.PrintChannelFilter(Sharp.Shared.Enums.HudPrintChannel channel, string message, Sharp.Shared.Types.RecipientFilter* filter)` [L:34]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Game.PrintChannelTeam(Sharp.Shared.Enums.HudPrintChannel channel, Sharp.Shared.Enums.CStrikeTeam team, string message)` [L:32]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Game.RadioMessageAll(Sharp.Shared.Units.PlayerSlot slot, string name, string? param1, string? param2, string? param3, string? param4)` [L:44]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Game.RadioMessageTeam(Sharp.Shared.Enums.CStrikeTeam team, Sharp.Shared.Units.PlayerSlot slot, string name, string? param1, string? param2, string? param3, string? param4)` [L:36]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Game.TerminateRound(float delay, Sharp.Shared.Enums.RoundEndReason reason, bool bypassHook, Sharp.Shared.Types.TeamRewardInfo* rewardInfo, int infoSize)` [L:51]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Game.TraceLine(Sharp.Shared.Types.Vector* start, Sharp.Shared.Types.Vector* end, Sharp.Shared.Enums.InteractionLayers mask, Sharp.Shared.Enums.CollisionGroupType group, Sharp.Shared.Enums.TraceQueryFlag flags, Sharp.Shared.Enums.InteractionLayers excludeLayers, nint ignoreEntity1, nint ignoreEntity2, bool ignorePlayers, Sharp.Shared.Types.TraceResultStruct* result)` [L:57]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Game.TraceLineFilter(Sharp.Shared.Types.Vector* start, Sharp.Shared.Types.Vector* end, Sharp.Shared.Enums.InteractionLayers mask, Sharp.Shared.Enums.CollisionGroupType group, Sharp.Shared.Enums.TraceQueryFlag flags, Sharp.Shared.Enums.InteractionLayers excludeLayers, Sharp.Shared.Types.TraceResultStruct* result)` [L:68]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Game.TraceShape(Sharp.Shared.Types.TraceShapeRay* ray, Sharp.Shared.Types.Vector* start, Sharp.Shared.Types.Vector* end, Sharp.Shared.Enums.InteractionLayers mask, Sharp.Shared.Enums.CollisionGroupType group, Sharp.Shared.Enums.TraceQueryFlag flags, Sharp.Shared.Enums.InteractionLayers excludeLayers, nint ignoreEntity1, nint ignoreEntity2, bool ignorePlayers, Sharp.Shared.Types.TraceResultStruct* result)` [L:76]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Game.TraceShapeFilter(Sharp.Shared.Types.TraceShapeRay* ray, Sharp.Shared.Types.Vector* start, Sharp.Shared.Types.Vector* end, Sharp.Shared.Enums.InteractionLayers mask, Sharp.Shared.Enums.CollisionGroupType group, Sharp.Shared.Enums.TraceQueryFlag flags, Sharp.Shared.Enums.InteractionLayers excludeLayers, Sharp.Shared.Types.TraceResultStruct* result)` [L:88]
  - Modifiers: public, static


### class Net

- FullName: `Sharp.Core.Bridges.Natives.Net`
- Kind: class
- Modifiers: public, static
- Source: Sharp.Core/Bridges/Natives/Net.cs:25
- Generated: false

Inheritance: object → **Net**

#### Methods
- `static bool Sharp.Core.Bridges.Natives.Net.CopyFromOtherMessage(nint msg, byte* data, int size)` [L:111]
  - Modifiers: public, static
- `static bool Sharp.Core.Bridges.Natives.Net.NetMessageHasField(nint msg, string field)` [L:41]
  - Modifiers: public, static
- `static bool Sharp.Core.Bridges.Natives.Net.ReadNetMessageBool(nint msg, string field, out bool value, int repeatedIndex)` [L:53]
  - Modifiers: public, static
- `static bool Sharp.Core.Bridges.Natives.Net.ReadNetMessageBytes(nint msg, string field, out nint data, out int size, int repeatedIndex)` [L:63]
  - Modifiers: public, static
- `static bool Sharp.Core.Bridges.Natives.Net.ReadNetMessageDouble(nint msg, string field, out double value, int repeatedIndex)` [L:59]
  - Modifiers: public, static
- `static bool Sharp.Core.Bridges.Natives.Net.ReadNetMessageEnum(nint msg, string field, out int value, int repeatedIndex)` [L:55]
  - Modifiers: public, static
- `static bool Sharp.Core.Bridges.Natives.Net.ReadNetMessageFloat(nint msg, string field, out float value, int repeatedIndex)` [L:57]
  - Modifiers: public, static
- `static bool Sharp.Core.Bridges.Natives.Net.ReadNetMessageInt32(nint msg, string field, out int value, int repeatedIndex)` [L:45]
  - Modifiers: public, static
- `static bool Sharp.Core.Bridges.Natives.Net.ReadNetMessageInt64(nint msg, string field, out long value, int repeatedIndex)` [L:49]
  - Modifiers: public, static
- `static bool Sharp.Core.Bridges.Natives.Net.ReadNetMessageUInt32(nint msg, string field, out uint value, int repeatedIndex)` [L:47]
  - Modifiers: public, static
- `static bool Sharp.Core.Bridges.Natives.Net.ReadNetMessageUInt64(nint msg, string field, out ulong value, int repeatedIndex)` [L:51]
  - Modifiers: public, static
- `static bool Sharp.Core.Bridges.Natives.Net.RemoveNetMessageRepeated(nint msg, string field, int repeatedIndex)` [L:109]
  - Modifiers: public, static
- `static bool Sharp.Core.Bridges.Natives.Net.SendNetMessage(Sharp.Shared.Types.RecipientFilter* filter, nint handle, byte* pData, int size)` [L:27]
  - Modifiers: public, static
- `static bool Sharp.Core.Bridges.Natives.Net.SetNetMessageBool(nint msg, string field, bool value, int repeatedIndex)` [L:73]
  - Modifiers: public, static
- `static bool Sharp.Core.Bridges.Natives.Net.SetNetMessageBytes(nint msg, string field, byte* data, int size, int repeatedIndex)` [L:83]
  - Modifiers: public, static
- `static bool Sharp.Core.Bridges.Natives.Net.SetNetMessageDouble(nint msg, string field, double value, int repeatedIndex)` [L:79]
  - Modifiers: public, static
- `static bool Sharp.Core.Bridges.Natives.Net.SetNetMessageEnum(nint msg, string field, int value, int repeatedIndex)` [L:75]
  - Modifiers: public, static
- `static bool Sharp.Core.Bridges.Natives.Net.SetNetMessageFloat(nint msg, string field, float value, int repeatedIndex)` [L:77]
  - Modifiers: public, static
- `static bool Sharp.Core.Bridges.Natives.Net.SetNetMessageInt32(nint msg, string field, int value, int repeatedIndex)` [L:65]
  - Modifiers: public, static
- `static bool Sharp.Core.Bridges.Natives.Net.SetNetMessageInt64(nint msg, string field, long value, int repeatedIndex)` [L:69]
  - Modifiers: public, static
- `static bool Sharp.Core.Bridges.Natives.Net.SetNetMessageString(nint msg, string field, string value, int repeatedIndex)` [L:81]
  - Modifiers: public, static
- `static bool Sharp.Core.Bridges.Natives.Net.SetNetMessageUInt32(nint msg, string field, uint value, int repeatedIndex)` [L:67]
  - Modifiers: public, static
- `static bool Sharp.Core.Bridges.Natives.Net.SetNetMessageUInt64(nint msg, string field, ulong value, int repeatedIndex)` [L:71]
  - Modifiers: public, static
- `static int Sharp.Core.Bridges.Natives.Net.AddNetMessageBool(nint msg, string field, bool value)` [L:93]
  - Modifiers: public, static
- `static int Sharp.Core.Bridges.Natives.Net.AddNetMessageBytes(nint msg, string field, byte* data, int size)` [L:103]
  - Modifiers: public, static
- `static int Sharp.Core.Bridges.Natives.Net.AddNetMessageDouble(nint msg, string field, double value)` [L:99]
  - Modifiers: public, static
- `static int Sharp.Core.Bridges.Natives.Net.AddNetMessageEnum(nint msg, string field, int value)` [L:95]
  - Modifiers: public, static
- `static int Sharp.Core.Bridges.Natives.Net.AddNetMessageFloat(nint msg, string field, float value)` [L:97]
  - Modifiers: public, static
- `static int Sharp.Core.Bridges.Natives.Net.AddNetMessageInt32(nint msg, string field, int value)` [L:85]
  - Modifiers: public, static
- `static int Sharp.Core.Bridges.Natives.Net.AddNetMessageInt64(nint msg, string field, long value)` [L:89]
  - Modifiers: public, static
- `static int Sharp.Core.Bridges.Natives.Net.AddNetMessageString(nint msg, string field, string value)` [L:101]
  - Modifiers: public, static
- `static int Sharp.Core.Bridges.Natives.Net.AddNetMessageUInt32(nint msg, string field, uint value)` [L:87]
  - Modifiers: public, static
- `static int Sharp.Core.Bridges.Natives.Net.AddNetMessageUInt64(nint msg, string field, ulong value)` [L:91]
  - Modifiers: public, static
- `static int Sharp.Core.Bridges.Natives.Net.NetMessageGetRepeatedCount(nint msg, string field)` [L:43]
  - Modifiers: public, static
- `static nint Sharp.Core.Bridges.Natives.Net.AddNetMessageRepeated(nint msg, string field)` [L:107]
  - Modifiers: public, static
- `static nint Sharp.Core.Bridges.Natives.Net.GetNetMessageHandle(string name)` [L:29]
  - Modifiers: public, static
- `static nint Sharp.Core.Bridges.Natives.Net.GetNetMessageName(nint msg)` [L:37]
  - Modifiers: public, static
- `static nint Sharp.Core.Bridges.Natives.Net.ReadNetMessageMessage(nint msg, string field, int repeatedIndex)` [L:105]
  - Modifiers: public, static
- `static nint Sharp.Core.Bridges.Natives.Net.ReadNetMessageString(nint msg, string field, int repeatedIndex)` [L:61]
  - Modifiers: public, static
- `static ulong Sharp.Core.Bridges.Natives.Net.GetNetMessageSize(nint size)` [L:39]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Net.HookNetMessage(Sharp.Shared.Enums.ProtobufNetMessageType msgId)` [L:31]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Net.SerializeNetMessage(nint data, int size, byte* output)` [L:35]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Net.UnhookNetMessage(Sharp.Shared.Enums.ProtobufNetMessageType msgId)` [L:33]
  - Modifiers: public, static


### class Player

- FullName: `Sharp.Core.Bridges.Natives.Player`
- Kind: class
- Modifiers: public, static
- Source: Sharp.Core/Bridges/Natives/Player.cs:26
- Generated: false

Inheritance: object → **Player**

#### Methods
- `static Sharp.Shared.Types.SoundOpEventGuid Sharp.Core.Bridges.Natives.Player.ControllerEmitSoundClient(nint ptr, string sound, float?* volume)` [L:50]
  - Modifiers: public, static
- `static Sharp.Shared.Types.SoundOpEventGuid Sharp.Core.Bridges.Natives.Player.PawnEmitSoundClient(nint ptr, string sound, float?* volume)` [L:101]
  - Modifiers: public, static
- `static bool Sharp.Core.Bridges.Natives.Player.PawnDetachWeapon(nint ptr, nint entityPtr)` [L:95]
  - Modifiers: public, static
- `static bool Sharp.Core.Bridges.Natives.Player.PawnIsPlayer(nint ptr)` [L:103]
  - Modifiers: public, static
- `static bool Sharp.Core.Bridges.Natives.Player.PawnSelectItem(nint ptr, nint entityPtr)` [L:93]
  - Modifiers: public, static
- `static float Sharp.Core.Bridges.Natives.Player.ControllerGetLaggedMovement(nint ptr)` [L:61]
  - Modifiers: public, static
- `static nint Sharp.Core.Bridges.Natives.Player.ControllerFindBySlot(long slot)` [L:44]
  - Modifiers: public, static
- `static nint Sharp.Core.Bridges.Natives.Player.ControllerFromEntity(nint ptr)` [L:30]
  - Modifiers: public, static
- `static nint Sharp.Core.Bridges.Natives.Player.ControllerGetItemInLoadoutFromInventory(nint ptr, Sharp.Shared.Enums.CStrikeTeam team, int slot)` [L:48]
  - Modifiers: public, static
- `static nint Sharp.Core.Bridges.Natives.Player.ControllerGetPawn(nint ptr)` [L:28]
  - Modifiers: public, static
- `static nint Sharp.Core.Bridges.Natives.Player.PawnFindBySlot(long slot)` [L:81]
  - Modifiers: public, static
- `static nint Sharp.Core.Bridges.Natives.Player.PawnFromEntity(nint ptr)` [L:67]
  - Modifiers: public, static
- `static nint Sharp.Core.Bridges.Natives.Player.PawnGetActiveWeapon(nint ptr)` [L:83]
  - Modifiers: public, static
- `static nint Sharp.Core.Bridges.Natives.Player.PawnGetController(nint ptr)` [L:65]
  - Modifiers: public, static
- `static nint Sharp.Core.Bridges.Natives.Player.PawnGetWeaponBySlot(nint ptr, Sharp.Shared.Enums.GearSlot slot, long unknown)` [L:85]
  - Modifiers: public, static
- `static nint Sharp.Core.Bridges.Natives.Player.PawnGiveNamedItem(nint ptr, string name)` [L:79]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Player.ControllerCheckPawn(nint ptr)` [L:52]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Player.ControllerPrint(nint ptr, Sharp.Shared.Enums.HudPrintChannel channel, string message, string? param1, string? param2, string? param3, string? param4)` [L:32]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Player.ControllerRoundRespawn(nint ptr)` [L:40]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Player.ControllerSetClanTag(nint ptr, string tag)` [L:46]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Player.ControllerSetLaggedMovement(nint ptr, float val)` [L:63]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Player.ControllerSetPawn(nint ptr, nint pawnPtr, bool unknown1, bool unknown2, bool unknown3, bool unknown4)` [L:54]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Player.ControllerSwitchTeam(nint ptr, Sharp.Shared.Enums.CStrikeTeam team)` [L:42]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Player.PawnDropWeapon(nint ptr, nint entityPtr)` [L:91]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Player.PawnGiveGloves(nint ptr, int itemDefIndex, int prefab, float wear, int seed)` [L:99]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Player.PawnPrint(nint ptr, Sharp.Shared.Enums.HudPrintChannel channel, string message, string? param1, string? param2, string? param3, string? param4)` [L:69]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Player.PawnRemoveAllItems(nint ptr, bool removeSuit)` [L:89]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Player.PawnRemovePlayerItem(nint ptr, nint entityPtr)` [L:87]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Player.PawnSlay(nint ptr, bool explode)` [L:77]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Player.PawnSwitchWeapon(nint ptr, nint entityPtr)` [L:97]
  - Modifiers: public, static


### class Schema

- FullName: `Sharp.Core.Bridges.Natives.Schema`
- Kind: class
- Modifiers: public, static
- Source: Sharp.Core/Bridges/Natives/Schema.cs:22
- Generated: false

Inheritance: object → **Schema**

#### Methods
- `static nint Sharp.Core.Bridges.Natives.Schema.GetSchemas()` [L:24]
  - Modifiers: public, static


### class Sound

- FullName: `Sharp.Core.Bridges.Natives.Sound`
- Kind: class
- Modifiers: public, static
- Source: Sharp.Core/Bridges/Natives/Sound.cs:24
- Generated: false

Inheritance: object → **Sound**

#### Methods
- `static bool Sharp.Core.Bridges.Natives.Sound.IsSoundEventValid(string soundEvent)` [L:44]
  - Modifiers: public, static
- `static bool Sharp.Core.Bridges.Natives.Sound.SetSoundEventParamFloat(long guid, string param, float value, Sharp.Shared.Types.RecipientFilter* filter)` [L:34]
  - Modifiers: public, static
- `static bool Sharp.Core.Bridges.Natives.Sound.SetSoundEventParamInt32(long guid, string param, int value, Sharp.Shared.Types.RecipientFilter* filter)` [L:38]
  - Modifiers: public, static
- `static bool Sharp.Core.Bridges.Natives.Sound.SetSoundEventParamUInt32(long guid, string param, uint value, Sharp.Shared.Types.RecipientFilter* filter)` [L:40]
  - Modifiers: public, static
- `static bool Sharp.Core.Bridges.Natives.Sound.SetSoundEventParamUInt64(long guid, string param, ulong value, Sharp.Shared.Types.RecipientFilter* filter)` [L:42]
  - Modifiers: public, static
- `static bool Sharp.Core.Bridges.Natives.Sound.SetSoundEventParamVector(long guid, string param, Sharp.Shared.Types.Vector* value, Sharp.Shared.Types.RecipientFilter* filter)` [L:36]
  - Modifiers: public, static
- `static float Sharp.Core.Bridges.Natives.Sound.GetSoundDuration(string sound)` [L:26]
  - Modifiers: public, static
- `static long Sharp.Core.Bridges.Natives.Sound.StartSoundEvent(nint entity, string sound, float?* volume, Sharp.Shared.Types.RecipientFilter* filter)` [L:28]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Sound.StopSoundEvent(Sharp.Shared.Types.SoundOpEventGuid* guid)` [L:30]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Sound.StopSoundEventFilter(Sharp.Shared.Types.SoundOpEventGuid* guid, Sharp.Shared.Types.RecipientFilter* filter)` [L:32]
  - Modifiers: public, static


### class Transmit

- FullName: `Sharp.Core.Bridges.Natives.Transmit`
- Kind: class
- Modifiers: public, static
- Source: Sharp.Core/Bridges/Natives/Transmit.cs:25
- Generated: false

Inheritance: object → **Transmit**

#### Methods
- `static Sharp.Shared.Enums.TransmitFireBulletState Sharp.Core.Bridges.Natives.Transmit.GetWeaponFireBulletState(nint weapon)` [L:51]
  - Modifiers: public, static
- `static bool Sharp.Core.Bridges.Natives.Transmit.AddEntityHooks(nint entity, bool defaultTransmit)` [L:27]
  - Modifiers: public, static
- `static bool Sharp.Core.Bridges.Natives.Transmit.GetEntityBlock(Sharp.Shared.Units.EntityIndex entity)` [L:37]
  - Modifiers: public, static
- `static bool Sharp.Core.Bridges.Natives.Transmit.GetEntityState(Sharp.Shared.Units.EntityIndex entity, Sharp.Shared.Units.EntityIndex client, int channel)` [L:33]
  - Modifiers: public, static
- `static bool Sharp.Core.Bridges.Natives.Transmit.GetTempEntState(Sharp.Shared.Enums.BlockTempEntType type, Sharp.Shared.Units.PlayerSlot slot)` [L:45]
  - Modifiers: public, static
- `static bool Sharp.Core.Bridges.Natives.Transmit.IsEntityHooked(nint entity)` [L:31]
  - Modifiers: public, static
- `static bool Sharp.Core.Bridges.Natives.Transmit.RemoveEntHooks(nint entity)` [L:29]
  - Modifiers: public, static
- `static bool Sharp.Core.Bridges.Natives.Transmit.SetEntityBlock(Sharp.Shared.Units.EntityIndex entity, bool state)` [L:39]
  - Modifiers: public, static
- `static bool Sharp.Core.Bridges.Natives.Transmit.SetEntityOwner(Sharp.Shared.Units.EntityIndex entity, Sharp.Shared.Units.EntityIndex owner)` [L:43]
  - Modifiers: public, static
- `static bool Sharp.Core.Bridges.Natives.Transmit.SetEntityState(Sharp.Shared.Units.EntityIndex entity, Sharp.Shared.Units.EntityIndex client, bool stats, int channel)` [L:35]
  - Modifiers: public, static
- `static bool Sharp.Core.Bridges.Natives.Transmit.SetTempEntState(Sharp.Shared.Enums.BlockTempEntType type, Sharp.Shared.Units.PlayerSlot slot, bool state)` [L:47]
  - Modifiers: public, static
- `static int Sharp.Core.Bridges.Natives.Transmit.GetEntityOwner(Sharp.Shared.Units.EntityIndex entity)` [L:41]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Transmit.ClearReceiverState(Sharp.Shared.Units.EntityIndex receiver)` [L:49]
  - Modifiers: public, static
- `static void Sharp.Core.Bridges.Natives.Transmit.SetWeaponFireBulletState(nint weapon, Sharp.Shared.Enums.TransmitFireBulletState state)` [L:53]
  - Modifiers: public, static


