# Sharp.Shared.HookParams

Project: Sharp.Shared
Types: 44 (0 generated)

### struct EmptyHookReturn : System.ValueType

- FullName: `Sharp.Shared.HookParams.EmptyHookReturn`
- Kind: struct
- Modifiers: public, readonly
- Source: Sharp.Shared/HookParams/FunctionParams.cs:31
- Generated: false

Inheritance: object → System.ValueType → **EmptyHookReturn**


### interface IClientCanHearHookParams : Sharp.Shared.HookParams.IClientFunctionParams, Sharp.Shared.HookParams.IFunctionParams

- FullName: `Sharp.Shared.HookParams.IClientCanHearHookParams`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/HookParams/ClientCanHearHookParams.cs:24
- Generated: false

#### Properties
- `Sharp.Shared.Objects.IGameClient Sharp.Shared.HookParams.IClientCanHearHookParams.Speaker` [L:27]
  - Modifiers: public, abstract, readonly


### interface IClientConnectHookParams : Sharp.Shared.HookParams.IFunctionParams

- FullName: `Sharp.Shared.HookParams.IClientConnectHookParams`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/HookParams/ClientConnectHookParams.cs:25
- Generated: false

#### Properties
- `Sharp.Shared.Units.SteamID Sharp.Shared.HookParams.IClientConnectHookParams.SteamId` [L:27]
  - Modifiers: public, abstract, readonly
- `string Sharp.Shared.HookParams.IClientConnectHookParams.Name` [L:28]
  - Modifiers: public, abstract, readonly

#### Methods
- `void Sharp.Shared.HookParams.IClientConnectHookParams.SetBlockReason(string reason)` [L:37]
  - Modifiers: public, abstract
  - Summary: Set the reason to reject this client's connection


### interface IClientFunctionParams

- FullName: `Sharp.Shared.HookParams.IClientFunctionParams`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/HookParams/FunctionParams.cs:33
- Generated: false

#### Properties
- `Sharp.Shared.Objects.IGameClient Sharp.Shared.HookParams.IClientFunctionParams.Client` [L:35]
  - Modifiers: public, abstract, readonly


### interface IClientSpeakingHookParams : Sharp.Shared.HookParams.IClientFunctionParams, Sharp.Shared.HookParams.IFunctionParams

- FullName: `Sharp.Shared.HookParams.IClientSpeakingHookParams`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/HookParams/ClientSpeakingHookParams.cs:22
- Generated: false

#### Properties
- `int Sharp.Shared.HookParams.IClientSpeakingHookParams.Size` [L:42]
  - Modifiers: public, abstract, readonly
  - Summary: Size of voice data
- `nint Sharp.Shared.HookParams.IClientSpeakingHookParams.PVoiceData` [L:37]
  - Modifiers: public, abstract, readonly
  - Summary: Voice data
- `uint Sharp.Shared.HookParams.IClientSpeakingHookParams.SectionNumber` [L:32]
  - Modifiers: public, abstract, readonly
  - Summary: Voice section id
- `ulong Sharp.Shared.HookParams.IClientSpeakingHookParams.Xuid` [L:27]
  - Modifiers: public, abstract, readonly
  - Summary: User steamid


### interface IConnectClientHookParams : Sharp.Shared.HookParams.IFunctionParams

- FullName: `Sharp.Shared.HookParams.IConnectClientHookParams`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/HookParams/ConnectClientHookParams.cs:24
- Generated: false

#### Properties
- `Sharp.Shared.Units.SteamID Sharp.Shared.HookParams.IConnectClientHookParams.SteamId` [L:26]
  - Modifiers: public, abstract, readonly
- `string Sharp.Shared.HookParams.IConnectClientHookParams.Ip` [L:28]
  - Modifiers: public, abstract, readonly
- `string Sharp.Shared.HookParams.IConnectClientHookParams.Name` [L:27]
  - Modifiers: public, abstract, readonly


### interface IEmitMusicForwardParams : Sharp.Shared.HookParams.IFunctionParams

- FullName: `Sharp.Shared.HookParams.IEmitMusicForwardParams`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/HookParams/EmitMusicForwardParams.cs:25
- Generated: false

#### Properties
- `Sharp.Shared.Types.SoundOpEventGuid Sharp.Shared.HookParams.IEmitMusicForwardParams.EventGuid` [L:30]
  - Modifiers: public, abstract, readonly
- `Sharp.Shared.Units.EntityIndex Sharp.Shared.HookParams.IEmitMusicForwardParams.EntityIndex` [L:27]
  - Modifiers: public, abstract, readonly
- `Sharp.Shared.Units.NetworkReceiver Sharp.Shared.HookParams.IEmitMusicForwardParams.Receivers` [L:31]
  - Modifiers: public, abstract, readonly
- `float Sharp.Shared.HookParams.IEmitMusicForwardParams.Duration` [L:29]
  - Modifiers: public, abstract, readonly
- `string Sharp.Shared.HookParams.IEmitMusicForwardParams.SoundName` [L:28]
  - Modifiers: public, abstract, readonly


### interface IEmitSoundHookParams : Sharp.Shared.HookParams.IFunctionParams

- FullName: `Sharp.Shared.HookParams.IEmitSoundHookParams`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/HookParams/EmitSoundHookParams.cs:24
- Generated: false

#### Properties
- `Sharp.Shared.Units.EntityIndex Sharp.Shared.HookParams.IEmitSoundHookParams.EntityIndex` [L:26]
  - Modifiers: public, abstract, readonly
- `Sharp.Shared.Units.NetworkReceiver Sharp.Shared.HookParams.IEmitSoundHookParams.Receivers` [L:29]
  - Modifiers: public, abstract, readonly
- `bool Sharp.Shared.HookParams.IEmitSoundHookParams.Changed` [L:30]
  - Modifiers: public, abstract, readonly
- `float Sharp.Shared.HookParams.IEmitSoundHookParams.Volume` [L:28]
  - Modifiers: public, abstract, readonly
- `string Sharp.Shared.HookParams.IEmitSoundHookParams.SoundName` [L:27]
  - Modifiers: public, abstract, readonly

#### Methods
- `bool Sharp.Shared.HookParams.IEmitSoundHookParams.HasReceiver(Sharp.Shared.Units.PlayerSlot slot)` [L:38]
  - Modifiers: public, abstract
- `int Sharp.Shared.HookParams.IEmitSoundHookParams.GetReceiverCount()` [L:36]
  - Modifiers: public, abstract
- `void Sharp.Shared.HookParams.IEmitSoundHookParams.AddReceiver(Sharp.Shared.Units.PlayerSlot slot)` [L:40]
  - Modifiers: public, abstract
- `void Sharp.Shared.HookParams.IEmitSoundHookParams.RemoveReceiver(Sharp.Shared.Units.PlayerSlot slot)` [L:42]
  - Modifiers: public, abstract
- `void Sharp.Shared.HookParams.IEmitSoundHookParams.SetSoundName(string soundName)` [L:32]
  - Modifiers: public, abstract
- `void Sharp.Shared.HookParams.IEmitSoundHookParams.SetVolume(float volume)` [L:34]
  - Modifiers: public, abstract
- `void Sharp.Shared.HookParams.IEmitSoundHookParams.UpdateReceiver(Sharp.Shared.Units.NetworkReceiver newReceivers)` [L:44]
  - Modifiers: public, abstract


### interface IEntityDispatchTraceAttackHookParams : Sharp.Shared.HookParams.IFunctionParams, Sharp.Shared.HookParams.ITakeDamageInfoParams, Sharp.Shared.HookParams.ITakeDamageResultParams

- FullName: `Sharp.Shared.HookParams.IEntityDispatchTraceAttackHookParams`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/HookParams/EntityDispatchTraceAttackHookParams.cs:24
- Generated: false

#### Properties
- `Sharp.Shared.GameEntities.IBaseEntity Sharp.Shared.HookParams.IEntityDispatchTraceAttackHookParams.Entity` [L:26]
  - Modifiers: public, abstract, readonly


### interface IFireBulletsInfoParams

- FullName: `Sharp.Shared.HookParams.IFireBulletsInfoParams`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/HookParams/FunctionParams.cs:128
- Generated: false

#### Properties
- `Sharp.Shared.Types.FireBulletInfo* Sharp.Shared.HookParams.IFireBulletsInfoParams.Info` [L:130]
  - Modifiers: public, abstract, readonly
- `Sharp.Shared.Types.Vector Sharp.Shared.HookParams.IFireBulletsInfoParams.ShootAngles` [L:133]
  - Modifiers: public, abstract
- `Sharp.Shared.Types.Vector Sharp.Shared.HookParams.IFireBulletsInfoParams.ShootPosition` [L:132]
  - Modifiers: public, abstract
- `float Sharp.Shared.HookParams.IFireBulletsInfoParams.Penetration` [L:136]
  - Modifiers: public, abstract
- `float Sharp.Shared.HookParams.IFireBulletsInfoParams.Range` [L:134]
  - Modifiers: public, abstract
- `float Sharp.Shared.HookParams.IFireBulletsInfoParams.RangeModifier` [L:135]
  - Modifiers: public, abstract
- `float Sharp.Shared.HookParams.IFireBulletsInfoParams.SpreadX` [L:140]
  - Modifiers: public, abstract
- `float Sharp.Shared.HookParams.IFireBulletsInfoParams.SpreadY` [L:141]
  - Modifiers: public, abstract
- `int Sharp.Shared.HookParams.IFireBulletsInfoParams.CurrentBullet` [L:139]
  - Modifiers: public, abstract
- `int Sharp.Shared.HookParams.IFireBulletsInfoParams.Damage` [L:138]
  - Modifiers: public, abstract
- `int Sharp.Shared.HookParams.IFireBulletsInfoParams.PenetrationCount` [L:137]
  - Modifiers: public, abstract


### interface IFunctionParams : Sharp.Shared.CStrike.IContextObject

- FullName: `Sharp.Shared.HookParams.IFunctionParams`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/HookParams/FunctionParams.cs:29
- Generated: false


### interface IGiveGloveItemForwardParams : Sharp.Shared.HookParams.IFunctionParams, Sharp.Shared.HookParams.IPlayerPawnFunctionParams

- FullName: `Sharp.Shared.HookParams.IGiveGloveItemForwardParams`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/HookParams/GiveGloveItemForwardParams.cs:22
- Generated: false


### interface IGiveNamedItemHookParams : Sharp.Shared.HookParams.IFunctionParams, Sharp.Shared.HookParams.IPlayerPawnFunctionParams

- FullName: `Sharp.Shared.HookParams.IGiveNamedItemHookParams`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/HookParams/GiveNamedItemHookParams.cs:22
- Generated: false

#### Properties
- `bool Sharp.Shared.HookParams.IGiveNamedItemHookParams.IgnoreCEconItemView` [L:33]
  - Modifiers: public, abstract, readonly
  - Summary: Gets a value indicating whether to ignore the CEconItemView.
- `string Sharp.Shared.HookParams.IGiveNamedItemHookParams.Classname` [L:27]
  - Modifiers: public, abstract, readonly
  - Summary: Gets the class name of the item (e.g. "weapon_ak47").

#### Methods
- `void Sharp.Shared.HookParams.IGiveNamedItemHookParams.SetOverride(string classname, [bool ignoreCEconItemView = false])` [L:40]
  - Modifiers: public, abstract
  - Summary: Overrides the parameters used to give the item.


### interface IHandleCommandJoinTeamHookParams : Sharp.Shared.HookParams.IFunctionParams, Sharp.Shared.HookParams.IPlayerFunctionParams

- FullName: `Sharp.Shared.HookParams.IHandleCommandJoinTeamHookParams`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/HookParams/HandleCommandJoinTeamHookParams.cs:22
- Generated: false

#### Properties
- `bool Sharp.Shared.HookParams.IHandleCommandJoinTeamHookParams.Queue` [L:30]
  - Modifiers: public, abstract, readonly
- `int Sharp.Shared.HookParams.IHandleCommandJoinTeamHookParams.CoachTeam` [L:31]
  - Modifiers: public, abstract, readonly
- `int Sharp.Shared.HookParams.IHandleCommandJoinTeamHookParams.Team` [L:28]
  - Modifiers: public, abstract, readonly
  - Summary: Gets the index of the team the player is attempting to join.

#### Methods
- `void Sharp.Shared.HookParams.IHandleCommandJoinTeamHookParams.OverrideCoachTeam(int coachTeam)` [L:37]
  - Modifiers: public, abstract
- `void Sharp.Shared.HookParams.IHandleCommandJoinTeamHookParams.OverrideQueue(bool queue)` [L:35]
  - Modifiers: public, abstract
- `void Sharp.Shared.HookParams.IHandleCommandJoinTeamHookParams.OverrideTeam(int team)` [L:33]
  - Modifiers: public, abstract


### interface IMapVoteCreatedForwardParams : Sharp.Shared.HookParams.IFunctionParams

- FullName: `Sharp.Shared.HookParams.IMapVoteCreatedForwardParams`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/HookParams/MapVoteCreatedForwardParams.cs:24
- Generated: false

#### Properties
- `Sharp.Shared.Objects.IGameRules Sharp.Shared.HookParams.IMapVoteCreatedForwardParams.GameRules` [L:26]
  - Modifiers: public, abstract, readonly


### interface IPlayerCanAcquireHookParams : Sharp.Shared.HookParams.IFunctionParams, Sharp.Shared.HookParams.IPlayerPawnFunctionParams

- FullName: `Sharp.Shared.HookParams.IPlayerCanAcquireHookParams`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/HookParams/PlayerCanAcquireHookParams.cs:24
- Generated: false

#### Properties
- `Sharp.Shared.Enums.EAcquireMethod Sharp.Shared.HookParams.IPlayerCanAcquireHookParams.Method` [L:27]
  - Modifiers: public, abstract, readonly
- `Sharp.Shared.Enums.EAcquireResult Sharp.Shared.HookParams.IPlayerCanAcquireHookParams.DefaultResult` [L:28]
  - Modifiers: public, abstract, readonly
- `ushort Sharp.Shared.HookParams.IPlayerCanAcquireHookParams.ItemDefinitionIndex` [L:26]
  - Modifiers: public, abstract, readonly


### interface IPlayerDispatchTraceAttackHookParams : Sharp.Shared.HookParams.IFunctionParams, Sharp.Shared.HookParams.IPlayerPawnFunctionParams, Sharp.Shared.HookParams.ITakeDamageInfoParams, Sharp.Shared.HookParams.ITakeDamageResultParams

- FullName: `Sharp.Shared.HookParams.IPlayerDispatchTraceAttackHookParams`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/HookParams/PlayerDispatchTraceAttackHookParams.cs:22
- Generated: false


### interface IPlayerDropWeaponForwardParams : Sharp.Shared.HookParams.IFunctionParams, Sharp.Shared.HookParams.IPlayerWeaponWithServiceFunctionParams

- FullName: `Sharp.Shared.HookParams.IPlayerDropWeaponForwardParams`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/HookParams/PlayerDropWeaponForwardParams.cs:22
- Generated: false


### interface IPlayerEquipWeaponForwardParams : Sharp.Shared.HookParams.IFunctionParams, Sharp.Shared.HookParams.IPlayerWeaponWithServiceFunctionParams

- FullName: `Sharp.Shared.HookParams.IPlayerEquipWeaponForwardParams`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/HookParams/PlayerEquipWeaponForwardParams.cs:24
- Generated: false

#### Obsolete Members
- `long Sharp.Shared.HookParams.IPlayerEquipWeaponForwardParams.EquipmentValue` [L:27] — DO NOT USE THIS, IT IS GARBAGE VALUE FROM LAST RAX REGISTER. WILL BE REMOVED IN THE FUTURE


### interface IPlayerFunctionParams : Sharp.Shared.HookParams.IClientFunctionParams

- FullName: `Sharp.Shared.HookParams.IPlayerFunctionParams`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/HookParams/FunctionParams.cs:38
- Generated: false

#### Properties
- `Sharp.Shared.GameEntities.IPlayerController Sharp.Shared.HookParams.IPlayerFunctionParams.Controller` [L:40]
  - Modifiers: public, abstract, readonly


### interface IPlayerGetMaxSpeedHookParams : Sharp.Shared.HookParams.IFunctionParams, Sharp.Shared.HookParams.IPlayerPawnFunctionParams

- FullName: `Sharp.Shared.HookParams.IPlayerGetMaxSpeedHookParams`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/HookParams/PlayerGetMaxSpeedHookParams.cs:24
- Generated: false

#### Properties
- `float Sharp.Shared.HookParams.IPlayerGetMaxSpeedHookParams.OriginalSpeed` [L:39]
  - Modifiers: public, abstract, readonly
  - Summary: Gets the original max run speed calculated by the game.


### interface IPlayerKilledForwardParams : Sharp.Shared.HookParams.IFunctionParams, Sharp.Shared.HookParams.IPlayerPawnFunctionParams, Sharp.Shared.HookParams.ITakeDamageInfoParams

- FullName: `Sharp.Shared.HookParams.IPlayerKilledForwardParams`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/HookParams/PlayerKilledForwardParams.cs:24
- Generated: false

#### Properties
- `Sharp.Shared.Types.TakeDamageResult* Sharp.Shared.HookParams.IPlayerKilledForwardParams.Result` [L:26]
  - Modifiers: public, abstract, readonly
- `int Sharp.Shared.HookParams.IPlayerKilledForwardParams.DamageTaken` [L:32]
  - Modifiers: public, abstract
- `int Sharp.Shared.HookParams.IPlayerKilledForwardParams.HealthBefore` [L:30]
  - Modifiers: public, abstract
- `int Sharp.Shared.HookParams.IPlayerKilledForwardParams.HealthLost` [L:28]
  - Modifiers: public, abstract
- `int Sharp.Shared.HookParams.IPlayerKilledForwardParams.TotalledDamageTaken` [L:36]
  - Modifiers: public, abstract
- `int Sharp.Shared.HookParams.IPlayerKilledForwardParams.TotalledHealthLost` [L:34]
  - Modifiers: public, abstract


### interface IPlayerMovementFunctionParams : Sharp.Shared.HookParams.IPlayerPawnFunctionParams

- FullName: `Sharp.Shared.HookParams.IPlayerMovementFunctionParams`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/HookParams/FunctionParams.cs:58
- Generated: false

#### Properties
- `Sharp.Shared.GameObjects.IPlayerMovementService Sharp.Shared.HookParams.IPlayerMovementFunctionParams.Service` [L:60]
  - Modifiers: public, abstract, readonly


### interface IPlayerMovementWithDataFunctionParams : Sharp.Shared.HookParams.IPlayerMovementFunctionParams

- FullName: `Sharp.Shared.HookParams.IPlayerMovementWithDataFunctionParams`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/HookParams/FunctionParams.cs:63
- Generated: false

#### Properties
- `Sharp.Shared.Types.MoveData* Sharp.Shared.HookParams.IPlayerMovementWithDataFunctionParams.Info` [L:65]
  - Modifiers: public, abstract, readonly
- `Sharp.Shared.Types.Vector Sharp.Shared.HookParams.IPlayerMovementWithDataFunctionParams.AbsOrigin` [L:70]
  - Modifiers: public, abstract
- `Sharp.Shared.Types.Vector Sharp.Shared.HookParams.IPlayerMovementWithDataFunctionParams.Angles` [L:69]
  - Modifiers: public, abstract
- `Sharp.Shared.Types.Vector Sharp.Shared.HookParams.IPlayerMovementWithDataFunctionParams.OutWishVel` [L:73]
  - Modifiers: public, abstract
- `Sharp.Shared.Types.Vector Sharp.Shared.HookParams.IPlayerMovementWithDataFunctionParams.Velocity` [L:68]
  - Modifiers: public, abstract
- `Sharp.Shared.Types.Vector Sharp.Shared.HookParams.IPlayerMovementWithDataFunctionParams.ViewAngles` [L:67]
  - Modifiers: public, abstract
- `bool Sharp.Shared.HookParams.IPlayerMovementWithDataFunctionParams.InAir` [L:74]
  - Modifiers: public, abstract
- `float Sharp.Shared.HookParams.IPlayerMovementWithDataFunctionParams.ClientMaxSpeed` [L:72]
  - Modifiers: public, abstract
- `float Sharp.Shared.HookParams.IPlayerMovementWithDataFunctionParams.MaxSpeed` [L:71]
  - Modifiers: public, abstract


### interface IPlayerPawnFunctionParams : Sharp.Shared.HookParams.IPlayerFunctionParams

- FullName: `Sharp.Shared.HookParams.IPlayerPawnFunctionParams`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/HookParams/FunctionParams.cs:43
- Generated: false

#### Properties
- `Sharp.Shared.GameEntities.IPlayerPawn Sharp.Shared.HookParams.IPlayerPawnFunctionParams.Pawn` [L:45]
  - Modifiers: public, abstract, readonly


### interface IPlayerProcessMoveForwardParams : Sharp.Shared.HookParams.IFunctionParams, Sharp.Shared.HookParams.IPlayerMovementWithDataFunctionParams

- FullName: `Sharp.Shared.HookParams.IPlayerProcessMoveForwardParams`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/HookParams/PlayerProcessMoveForwardParams.cs:22
- Generated: false


### interface IPlayerRunCommandHookParams : Sharp.Shared.HookParams.IFunctionParams, Sharp.Shared.HookParams.IPlayerFunctionParams

- FullName: `Sharp.Shared.HookParams.IPlayerRunCommandHookParams`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/HookParams/PlayerRunCommandHookParams.cs:27
- Generated: false

#### Properties
- `Sharp.Shared.Enums.UserCommandButtons Sharp.Shared.HookParams.IPlayerRunCommandHookParams.ChangedButtons` [L:45]
  - Modifiers: public, abstract
- `Sharp.Shared.Enums.UserCommandButtons Sharp.Shared.HookParams.IPlayerRunCommandHookParams.KeyButtons` [L:44]
  - Modifiers: public, abstract
- `Sharp.Shared.Enums.UserCommandButtons Sharp.Shared.HookParams.IPlayerRunCommandHookParams.ScrollButtons` [L:46]
  - Modifiers: public, abstract
- `Sharp.Shared.GameEntities.IBasePlayerPawn Sharp.Shared.HookParams.IPlayerRunCommandHookParams.Pawn` [L:29]
  - Modifiers: public, abstract, readonly
- `Sharp.Shared.GameObjects.IMovementService Sharp.Shared.HookParams.IPlayerRunCommandHookParams.Service` [L:30]
  - Modifiers: public, abstract, readonly
- `Sharp.Shared.Types.CppProtobuf.CBaseUserCmdPb* Sharp.Shared.HookParams.IPlayerRunCommandHookParams.BaseUserCmd` [L:42]
  - Modifiers: public, abstract, readonly
  - Summary: Get BaseUserCmd Please use ref when getting member struct
- `Sharp.Shared.Types.CppProtobuf.CCSGOUserCmdPb* Sharp.Shared.HookParams.IPlayerRunCommandHookParams.CSGOUserCmd` [L:36]
  - Modifiers: public, abstract, readonly
  - Summary: Get CSGOUserCmd Please use ref when getting member struct
- `int Sharp.Shared.HookParams.IPlayerRunCommandHookParams.InputHistorySize` [L:48]
  - Modifiers: public, abstract, readonly
- `int Sharp.Shared.HookParams.IPlayerRunCommandHookParams.SubtickMoveSize` [L:56]
  - Modifiers: public, abstract, readonly

#### Methods
- `Sharp.Shared.Types.CppProtobuf.CCSGOInputHistoryEntryPb* Sharp.Shared.HookParams.IPlayerRunCommandHookParams.GetInputHistoryEntry(int index)` [L:54]
  - Modifiers: public, abstract
  - Summary: Get InputHistory
- `Sharp.Shared.Types.CppProtobuf.CSubtickMoveStepPb* Sharp.Shared.HookParams.IPlayerRunCommandHookParams.GetSubtickMove(int index)` [L:62]
  - Modifiers: public, abstract
  - Summary: Get SubtickMove


### interface IPlayerSpawnForwardParams : Sharp.Shared.HookParams.IFunctionParams, Sharp.Shared.HookParams.IPlayerPawnFunctionParams

- FullName: `Sharp.Shared.HookParams.IPlayerSpawnForwardParams`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/HookParams/PlayerSpawnForwardParams.cs:22
- Generated: false


### interface IPlayerSwitchWeaponForwardParams : Sharp.Shared.HookParams.IFunctionParams, Sharp.Shared.HookParams.IPlayerPawnFunctionParams

- FullName: `Sharp.Shared.HookParams.IPlayerSwitchWeaponForwardParams`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/HookParams/PlayerSwitchWeaponForwardParams.cs:25
- Generated: false

#### Properties
- `Sharp.Shared.GameEntities.IBaseWeapon? Sharp.Shared.HookParams.IPlayerSwitchWeaponForwardParams.Weapon` [L:33]
  - Modifiers: public, abstract, readonly
  - Summary: The weapon being switched to, can be empty handsReturns null when switching to empty hands
- `Sharp.Shared.GameObjects.IWeaponService Sharp.Shared.HookParams.IPlayerSwitchWeaponForwardParams.Service` [L:27]
  - Modifiers: public, abstract, readonly


### interface IPlayerThinkForwardParams : Sharp.Shared.HookParams.IFunctionParams, Sharp.Shared.HookParams.IPlayerPawnFunctionParams

- FullName: `Sharp.Shared.HookParams.IPlayerThinkForwardParams`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/HookParams/PlayerThinkForwardParams.cs:22
- Generated: false


### interface IPlayerWalkMoveForwardParams : Sharp.Shared.HookParams.IFunctionParams, Sharp.Shared.HookParams.IPlayerMovementWithDataFunctionParams

- FullName: `Sharp.Shared.HookParams.IPlayerWalkMoveForwardParams`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/HookParams/PlayerWalkMoveForwardParams.cs:22
- Generated: false

#### Properties
- `int Sharp.Shared.HookParams.IPlayerWalkMoveForwardParams.Speed` [L:24]
  - Modifiers: public, abstract, readonly

#### Methods
- `void Sharp.Shared.HookParams.IPlayerWalkMoveForwardParams.SetSpeed(int speed)` [L:26]
  - Modifiers: public, abstract


### interface IPlayerWeaponCanEquipHookParams : Sharp.Shared.HookParams.IFunctionParams, Sharp.Shared.HookParams.IPlayerWeaponFunctionParams

- FullName: `Sharp.Shared.HookParams.IPlayerWeaponCanEquipHookParams`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/HookParams/PlayerWeaponCanEquipHookParams.cs:22
- Generated: false


### interface IPlayerWeaponCanSwitchHookParams : Sharp.Shared.HookParams.IFunctionParams, Sharp.Shared.HookParams.IPlayerWeaponFunctionParams

- FullName: `Sharp.Shared.HookParams.IPlayerWeaponCanSwitchHookParams`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/HookParams/PlayerWeaponCanSwitchHookParams.cs:22
- Generated: false


### interface IPlayerWeaponCanUseHookParams : Sharp.Shared.HookParams.IFunctionParams, Sharp.Shared.HookParams.IPlayerWeaponFunctionParams

- FullName: `Sharp.Shared.HookParams.IPlayerWeaponCanUseHookParams`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/HookParams/PlayerWeaponCanUseHookParams.cs:22
- Generated: false


### interface IPlayerWeaponFunctionParams : Sharp.Shared.HookParams.IPlayerPawnFunctionParams

- FullName: `Sharp.Shared.HookParams.IPlayerWeaponFunctionParams`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/HookParams/FunctionParams.cs:48
- Generated: false

#### Properties
- `Sharp.Shared.GameEntities.IBaseWeapon Sharp.Shared.HookParams.IPlayerWeaponFunctionParams.Weapon` [L:50]
  - Modifiers: public, abstract, readonly


### interface IPlayerWeaponWithServiceFunctionParams : Sharp.Shared.HookParams.IPlayerWeaponFunctionParams

- FullName: `Sharp.Shared.HookParams.IPlayerWeaponWithServiceFunctionParams`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/HookParams/FunctionParams.cs:53
- Generated: false

#### Properties
- `Sharp.Shared.GameObjects.IWeaponService Sharp.Shared.HookParams.IPlayerWeaponWithServiceFunctionParams.Service` [L:55]
  - Modifiers: public, abstract, readonly


### interface IPointServerCommandHookParams : Sharp.Shared.HookParams.IFunctionParams

- FullName: `Sharp.Shared.HookParams.IPointServerCommandHookParams`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/HookParams/PointServerCommandHookParams.cs:24
- Generated: false

#### Properties
- `Sharp.Shared.GameEntities.IBaseEntity Sharp.Shared.HookParams.IPointServerCommandHookParams.Entity` [L:26]
  - Modifiers: public, abstract, readonly
- `string Sharp.Shared.HookParams.IPointServerCommandHookParams.Command` [L:27]
  - Modifiers: public, abstract, readonly


### interface IPostEventAbstractHookParams : Sharp.Shared.HookParams.IFunctionParams

- FullName: `Sharp.Shared.HookParams.IPostEventAbstractHookParams`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/HookParams/PostEventAbstractHookParams.cs:26
- Generated: false

#### Properties
- `Sharp.Shared.Enums.ProtobufNetMessageType Sharp.Shared.HookParams.IPostEventAbstractHookParams.MsgId` [L:28]
  - Modifiers: public, abstract, readonly
- `Sharp.Shared.Objects.INetMessage Sharp.Shared.HookParams.IPostEventAbstractHookParams.Data` [L:29]
  - Modifiers: public, abstract, readonly
- `Sharp.Shared.Units.NetworkReceiver Sharp.Shared.HookParams.IPostEventAbstractHookParams.Receivers` [L:30]
  - Modifiers: public, abstract, readonly


### interface IPrintStatusHookParams : Sharp.Shared.HookParams.IFunctionParams

- FullName: `Sharp.Shared.HookParams.IPrintStatusHookParams`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/HookParams/PrintStatusHookParams.cs:24
- Generated: false

#### Properties
- `Sharp.Shared.Objects.IGameClient? Sharp.Shared.HookParams.IPrintStatusHookParams.Client` [L:29]
  - Modifiers: public, abstract, readonly
  - Summary: The client that triggers PrintStatus. if it is null that means it is triggered by console


### interface ISoundEventHookParams : Sharp.Shared.HookParams.IFunctionParams

- FullName: `Sharp.Shared.HookParams.ISoundEventHookParams`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/HookParams/SoundEventHookParams.cs:24
- Generated: false

#### Properties
- `Sharp.Shared.Units.EntityIndex Sharp.Shared.HookParams.ISoundEventHookParams.EntityIndex` [L:26]
  - Modifiers: public, abstract, readonly
- `Sharp.Shared.Units.NetworkReceiver Sharp.Shared.HookParams.ISoundEventHookParams.Receivers` [L:29]
  - Modifiers: public, abstract, readonly
- `bool Sharp.Shared.HookParams.ISoundEventHookParams.Changed` [L:30]
  - Modifiers: public, abstract, readonly
- `float Sharp.Shared.HookParams.ISoundEventHookParams.SoundDuration` [L:28]
  - Modifiers: public, abstract, readonly
- `string Sharp.Shared.HookParams.ISoundEventHookParams.SoundName` [L:27]
  - Modifiers: public, abstract, readonly

#### Methods
- `bool Sharp.Shared.HookParams.ISoundEventHookParams.HasReceiver(Sharp.Shared.Units.PlayerSlot slot)` [L:34]
  - Modifiers: public, abstract
- `int Sharp.Shared.HookParams.ISoundEventHookParams.GetReceiverCount()` [L:32]
  - Modifiers: public, abstract
- `void Sharp.Shared.HookParams.ISoundEventHookParams.AddReceiver(Sharp.Shared.Units.PlayerSlot slot)` [L:36]
  - Modifiers: public, abstract
- `void Sharp.Shared.HookParams.ISoundEventHookParams.RemoveReceiver(Sharp.Shared.Units.PlayerSlot slot)` [L:38]
  - Modifiers: public, abstract
- `void Sharp.Shared.HookParams.ISoundEventHookParams.UpdateReceiver(Sharp.Shared.Units.NetworkReceiver newReceivers)` [L:40]
  - Modifiers: public, abstract


### interface ITakeDamageInfoParams

- FullName: `Sharp.Shared.HookParams.ITakeDamageInfoParams`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/HookParams/FunctionParams.cs:77
- Generated: false

#### Properties
- `Sharp.Shared.Enums.DamageFlagBits Sharp.Shared.HookParams.ITakeDamageInfoParams.DamageType` [L:96]
  - Modifiers: public, abstract
- `Sharp.Shared.Enums.HitGroupType Sharp.Shared.HookParams.ITakeDamageInfoParams.HitGroup` [L:83]
  - Modifiers: public, abstract, readonly
- `Sharp.Shared.Enums.TakeDamageFlags Sharp.Shared.HookParams.ITakeDamageInfoParams.TakeDamageFlags` [L:102]
  - Modifiers: public, abstract
- `Sharp.Shared.Types.CEntityHandle<Sharp.Shared.GameEntities.IBaseEntity> Sharp.Shared.HookParams.ITakeDamageInfoParams.AbilityHandle` [L:94]
  - Modifiers: public, abstract
- `Sharp.Shared.Types.CEntityHandle<Sharp.Shared.GameEntities.IBaseEntity> Sharp.Shared.HookParams.ITakeDamageInfoParams.AttackerHandle` [L:93]
  - Modifiers: public, abstract
- `Sharp.Shared.Types.CEntityHandle<Sharp.Shared.GameEntities.IBaseEntity> Sharp.Shared.HookParams.ITakeDamageInfoParams.InflictorHandle` [L:92]
  - Modifiers: public, abstract
- `Sharp.Shared.Types.CEntityHandle<Sharp.Shared.GameEntities.IPlayerPawn> Sharp.Shared.HookParams.ITakeDamageInfoParams.AttackerPawnHandle` [L:110]
  - Modifiers: public, abstract
- `Sharp.Shared.Types.GameTrace* Sharp.Shared.HookParams.ITakeDamageInfoParams.Trace` [L:85]
  - Modifiers: public, abstract, readonly
- `Sharp.Shared.Types.TakeDamageInfo* Sharp.Shared.HookParams.ITakeDamageInfoParams.Info` [L:79]
  - Modifiers: public, abstract, readonly
- `Sharp.Shared.Types.Vector Sharp.Shared.HookParams.ITakeDamageInfoParams.DamageDirection` [L:91]
  - Modifiers: public, abstract
- `Sharp.Shared.Types.Vector Sharp.Shared.HookParams.ITakeDamageInfoParams.DamageForce` [L:88]
  - Modifiers: public, abstract
- `Sharp.Shared.Types.Vector Sharp.Shared.HookParams.ITakeDamageInfoParams.DamagePosition` [L:89]
  - Modifiers: public, abstract
- `Sharp.Shared.Types.Vector Sharp.Shared.HookParams.ITakeDamageInfoParams.ReportedPosition` [L:90]
  - Modifiers: public, abstract
- `Sharp.Shared.Types.Vector Sharp.Shared.HookParams.ITakeDamageInfoParams.TraceEndPosition` [L:82]
  - Modifiers: public, abstract, readonly
- `bool Sharp.Shared.HookParams.ITakeDamageInfoParams.InTakeDamageFlow` [L:104]
  - Modifiers: public, abstract
- `bool Sharp.Shared.HookParams.ITakeDamageInfoParams.IsPawn` [L:107]
  - Modifiers: public, abstract
- `bool Sharp.Shared.HookParams.ITakeDamageInfoParams.IsWorld` [L:108]
  - Modifiers: public, abstract
- `bool Sharp.Shared.HookParams.ITakeDamageInfoParams.ShouldBleed` [L:100]
  - Modifiers: public, abstract
- `bool Sharp.Shared.HookParams.ITakeDamageInfoParams.ShouldSpark` [L:101]
  - Modifiers: public, abstract
- `byte Sharp.Shared.HookParams.ITakeDamageInfoParams.AmmoType` [L:98]
  - Modifiers: public, abstract
- `float Sharp.Shared.HookParams.ITakeDamageInfoParams.Damage` [L:95]
  - Modifiers: public, abstract
- `float Sharp.Shared.HookParams.ITakeDamageInfoParams.OriginalDamage` [L:99]
  - Modifiers: public, abstract
- `int Sharp.Shared.HookParams.ITakeDamageInfoParams.AttackerPlayerSlot` [L:109]
  - Modifiers: public, abstract
- `int Sharp.Shared.HookParams.ITakeDamageInfoParams.DamageCustom` [L:97]
  - Modifiers: public, abstract
- `int Sharp.Shared.HookParams.ITakeDamageInfoParams.HitBoxId` [L:84]
  - Modifiers: public, abstract, readonly
- `int Sharp.Shared.HookParams.ITakeDamageInfoParams.NumObjectsPenetrated` [L:103]
  - Modifiers: public, abstract
- `int Sharp.Shared.HookParams.ITakeDamageInfoParams.Team` [L:112]
  - Modifiers: public, abstract
- `int Sharp.Shared.HookParams.ITakeDamageInfoParams.TeamChecked` [L:111]
  - Modifiers: public, abstract


### interface ITakeDamageResultParams

- FullName: `Sharp.Shared.HookParams.ITakeDamageResultParams`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/HookParams/FunctionParams.cs:115
- Generated: false

#### Properties
- `Sharp.Shared.Types.TakeDamageResult* Sharp.Shared.HookParams.ITakeDamageResultParams.Result` [L:117]
  - Modifiers: public, abstract, readonly
- `bool Sharp.Shared.HookParams.ITakeDamageResultParams.WasDamageSuppressed` [L:125]
  - Modifiers: public, abstract
- `float Sharp.Shared.HookParams.ITakeDamageResultParams.PreModifiedDamage` [L:122]
  - Modifiers: public, abstract
- `int Sharp.Shared.HookParams.ITakeDamageResultParams.DamageDealt` [L:121]
  - Modifiers: public, abstract
- `int Sharp.Shared.HookParams.ITakeDamageResultParams.HealthBefore` [L:120]
  - Modifiers: public, abstract
- `int Sharp.Shared.HookParams.ITakeDamageResultParams.HealthLost` [L:119]
  - Modifiers: public, abstract
- `int Sharp.Shared.HookParams.ITakeDamageResultParams.TotalledDamageDealt` [L:124]
  - Modifiers: public, abstract
- `int Sharp.Shared.HookParams.ITakeDamageResultParams.TotalledHealthLost` [L:123]
  - Modifiers: public, abstract


### interface ITerminateRoundHookParams : Sharp.Shared.HookParams.IFunctionParams

- FullName: `Sharp.Shared.HookParams.ITerminateRoundHookParams`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/HookParams/TerminateRoundHookParams.cs:27
- Generated: false

#### Properties
- `Sharp.Shared.Enums.RoundEndReason Sharp.Shared.HookParams.ITerminateRoundHookParams.Reason` [L:31]
  - Modifiers: public, abstract, readonly
- `Sharp.Shared.Objects.IGameRules Sharp.Shared.HookParams.ITerminateRoundHookParams.GameRules` [L:29]
  - Modifiers: public, abstract, readonly
- `System.ReadOnlySpan<Sharp.Shared.Types.TeamRewardInfo> Sharp.Shared.HookParams.ITerminateRoundHookParams.TeamRewardInfo` [L:32]
  - Modifiers: public, abstract, readonly
- `float Sharp.Shared.HookParams.ITerminateRoundHookParams.Delay` [L:30]
  - Modifiers: public, abstract, readonly

#### Methods
- `void Sharp.Shared.HookParams.ITerminateRoundHookParams.OverrideDelay(float delay)` [L:34]
  - Modifiers: public, abstract
- `void Sharp.Shared.HookParams.ITerminateRoundHookParams.OverrideReason(Sharp.Shared.Enums.RoundEndReason reason)` [L:36]
  - Modifiers: public, abstract
- `void Sharp.Shared.HookParams.ITerminateRoundHookParams.OverrideTeamRewards(Sharp.Shared.Types.TeamRewardInfo[] teamRewards)` [L:38]
  - Modifiers: public, abstract


### interface ITextMsgHookParams : Sharp.Shared.HookParams.IFunctionParams

- FullName: `Sharp.Shared.HookParams.ITextMsgHookParams`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/HookParams/TextMsgHookParams.cs:25
- Generated: false

#### Properties
- `Sharp.Shared.Enums.HudPrintChannel Sharp.Shared.HookParams.ITextMsgHookParams.Channel` [L:31]
  - Modifiers: public, abstract, readonly
  - Summary: The specific HUD channel where this message will be displayed
- `Sharp.Shared.Units.NetworkReceiver Sharp.Shared.HookParams.ITextMsgHookParams.Receivers` [L:45]
  - Modifiers: public, abstract, readonly
  - Summary: The target audience for this message (e.g., specific client, broadcast, or team).
- `string Sharp.Shared.HookParams.ITextMsgHookParams.Name` [L:40]
  - Modifiers: public, abstract, readonly
  - Summary: The content of the message.

#### Methods
- `bool Sharp.Shared.HookParams.ITextMsgHookParams.HasClient(Sharp.Shared.Units.PlayerSlot slot)` [L:52]
  - Modifiers: public, abstract
  - Summary: Utility method to check if a specific player slot is among the recipients of this message.


