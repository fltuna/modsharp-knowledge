# Sharp.Shared.GameEvents

Project: Sharp.Shared
Types: 17 (0 generated)

### interface IEventBombAbortDefuse : Sharp.Shared.Objects.IGameEvent

- FullName: `Sharp.Shared.GameEvents.IEventBombAbortDefuse`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameEvents/IEventBombAbortDefuse.cs:26
- Generated: false

#### Properties
- `Sharp.Shared.GameEntities.IPlayerController? Sharp.Shared.GameEvents.IEventBombAbortDefuse.Controller` [L:28]
  - Modifiers: public, abstract
- `Sharp.Shared.GameEntities.IPlayerPawn? Sharp.Shared.GameEvents.IEventBombAbortDefuse.Pawn` [L:29]
  - Modifiers: public, abstract
- `Sharp.Shared.Units.UserID Sharp.Shared.GameEvents.IEventBombAbortDefuse.UserId` [L:30]
  - Modifiers: public, abstract


### interface IEventBombAbortPlant : Sharp.Shared.Objects.IGameEvent

- FullName: `Sharp.Shared.GameEvents.IEventBombAbortPlant`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameEvents/IEventBombAbortPlant.cs:26
- Generated: false

#### Properties
- `Sharp.Shared.GameEntities.IPlayerController? Sharp.Shared.GameEvents.IEventBombAbortPlant.Controller` [L:28]
  - Modifiers: public, abstract
- `Sharp.Shared.GameEntities.IPlayerPawn? Sharp.Shared.GameEvents.IEventBombAbortPlant.Pawn` [L:29]
  - Modifiers: public, abstract
- `Sharp.Shared.Units.UserID Sharp.Shared.GameEvents.IEventBombAbortPlant.UserId` [L:30]
  - Modifiers: public, abstract
- `short Sharp.Shared.GameEvents.IEventBombAbortPlant.Site` [L:32]
  - Modifiers: public, abstract


### interface IEventBombBeginDefuse : Sharp.Shared.Objects.IGameEvent

- FullName: `Sharp.Shared.GameEvents.IEventBombBeginDefuse`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameEvents/IEventBombBeginDefuse.cs:26
- Generated: false

#### Properties
- `Sharp.Shared.GameEntities.IPlayerController? Sharp.Shared.GameEvents.IEventBombBeginDefuse.Controller` [L:28]
  - Modifiers: public, abstract
- `Sharp.Shared.GameEntities.IPlayerPawn? Sharp.Shared.GameEvents.IEventBombBeginDefuse.Pawn` [L:29]
  - Modifiers: public, abstract
- `Sharp.Shared.Units.UserID Sharp.Shared.GameEvents.IEventBombBeginDefuse.UserId` [L:30]
  - Modifiers: public, abstract
- `bool Sharp.Shared.GameEvents.IEventBombBeginDefuse.HasKit` [L:32]
  - Modifiers: public, abstract


### interface IEventBombBeginPlant : Sharp.Shared.Objects.IGameEvent

- FullName: `Sharp.Shared.GameEvents.IEventBombBeginPlant`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameEvents/IEventBombBeginPlant.cs:26
- Generated: false

#### Properties
- `Sharp.Shared.GameEntities.IPlayerController? Sharp.Shared.GameEvents.IEventBombBeginPlant.Controller` [L:28]
  - Modifiers: public, abstract
- `Sharp.Shared.GameEntities.IPlayerPawn? Sharp.Shared.GameEvents.IEventBombBeginPlant.Pawn` [L:29]
  - Modifiers: public, abstract
- `Sharp.Shared.Units.UserID Sharp.Shared.GameEvents.IEventBombBeginPlant.UserId` [L:30]
  - Modifiers: public, abstract
- `short Sharp.Shared.GameEvents.IEventBombBeginPlant.Site` [L:32]
  - Modifiers: public, abstract


### interface IEventBombDefused : Sharp.Shared.Objects.IGameEvent

- FullName: `Sharp.Shared.GameEvents.IEventBombDefused`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameEvents/IEventBombDefused.cs:26
- Generated: false

#### Properties
- `Sharp.Shared.GameEntities.IPlayerController? Sharp.Shared.GameEvents.IEventBombDefused.Controller` [L:28]
  - Modifiers: public, abstract
- `Sharp.Shared.GameEntities.IPlayerPawn? Sharp.Shared.GameEvents.IEventBombDefused.Pawn` [L:29]
  - Modifiers: public, abstract
- `Sharp.Shared.Units.UserID Sharp.Shared.GameEvents.IEventBombDefused.UserId` [L:30]
  - Modifiers: public, abstract
- `short Sharp.Shared.GameEvents.IEventBombDefused.Site` [L:32]
  - Modifiers: public, abstract


### interface IEventBombPlanted : Sharp.Shared.Objects.IGameEvent

- FullName: `Sharp.Shared.GameEvents.IEventBombPlanted`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameEvents/IEventBombPlanted.cs:26
- Generated: false

#### Properties
- `Sharp.Shared.GameEntities.IPlayerController? Sharp.Shared.GameEvents.IEventBombPlanted.Controller` [L:28]
  - Modifiers: public, abstract
- `Sharp.Shared.GameEntities.IPlayerPawn? Sharp.Shared.GameEvents.IEventBombPlanted.Pawn` [L:29]
  - Modifiers: public, abstract
- `Sharp.Shared.Units.UserID Sharp.Shared.GameEvents.IEventBombPlanted.UserId` [L:30]
  - Modifiers: public, abstract
- `short Sharp.Shared.GameEvents.IEventBombPlanted.Site` [L:32]
  - Modifiers: public, abstract


### interface IEventGrenadeThrown : Sharp.Shared.Objects.IGameEvent

- FullName: `Sharp.Shared.GameEvents.IEventGrenadeThrown`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameEvents/IEventGrenadeThrown.cs:26
- Generated: false

#### Properties
- `Sharp.Shared.GameEntities.IPlayerController? Sharp.Shared.GameEvents.IEventGrenadeThrown.Controller` [L:28]
  - Modifiers: public, abstract
- `Sharp.Shared.GameEntities.IPlayerPawn? Sharp.Shared.GameEvents.IEventGrenadeThrown.Pawn` [L:29]
  - Modifiers: public, abstract
- `Sharp.Shared.Units.UserID Sharp.Shared.GameEvents.IEventGrenadeThrown.UserId` [L:30]
  - Modifiers: public, abstract
- `string Sharp.Shared.GameEvents.IEventGrenadeThrown.Grenade` [L:32]
  - Modifiers: public, abstract


### interface IEventItemPurchased : Sharp.Shared.Objects.IGameEvent

- FullName: `Sharp.Shared.GameEvents.IEventItemPurchased`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameEvents/IEventItemPurchased.cs:27
- Generated: false

#### Properties
- `Sharp.Shared.Enums.CStrikeTeam Sharp.Shared.GameEvents.IEventItemPurchased.Team` [L:32]
  - Modifiers: public, abstract
- `Sharp.Shared.GameEntities.IPlayerController? Sharp.Shared.GameEvents.IEventItemPurchased.Controller` [L:29]
  - Modifiers: public, abstract
- `Sharp.Shared.Units.UserID Sharp.Shared.GameEvents.IEventItemPurchased.UserId` [L:30]
  - Modifiers: public, abstract
- `short Sharp.Shared.GameEvents.IEventItemPurchased.Loadout` [L:33]
  - Modifiers: public, abstract
- `string Sharp.Shared.GameEvents.IEventItemPurchased.Weapon` [L:34]
  - Modifiers: public, abstract


### interface IEventPlayerChangeName : Sharp.Shared.Objects.IGameEvent

- FullName: `Sharp.Shared.GameEvents.IEventPlayerChangeName`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameEvents/IEventPlayerChangeName.cs:26
- Generated: false

#### Properties
- `Sharp.Shared.GameEntities.IPlayerController? Sharp.Shared.GameEvents.IEventPlayerChangeName.Controller` [L:28]
  - Modifiers: public, abstract
- `Sharp.Shared.Units.UserID Sharp.Shared.GameEvents.IEventPlayerChangeName.UserId` [L:29]
  - Modifiers: public, abstract
- `string Sharp.Shared.GameEvents.IEventPlayerChangeName.NewName` [L:33]
  - Modifiers: public, abstract, readonly
- `string Sharp.Shared.GameEvents.IEventPlayerChangeName.OldName` [L:31]
  - Modifiers: public, abstract, readonly


### interface IEventPlayerDeath : Sharp.Shared.Objects.IGameEvent

- FullName: `Sharp.Shared.GameEvents.IEventPlayerDeath`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameEvents/IEventPlayerDeath.cs:27
- Generated: false

#### Properties
- `Sharp.Shared.Enums.HitGroupType Sharp.Shared.GameEvents.IEventPlayerDeath.HitGroup` [L:53]
  - Modifiers: public, abstract
- `Sharp.Shared.GameEntities.IPlayerController? Sharp.Shared.GameEvents.IEventPlayerDeath.AssisterController` [L:37]
  - Modifiers: public, abstract
- `Sharp.Shared.GameEntities.IPlayerController? Sharp.Shared.GameEvents.IEventPlayerDeath.KillerController` [L:33]
  - Modifiers: public, abstract
- `Sharp.Shared.GameEntities.IPlayerController? Sharp.Shared.GameEvents.IEventPlayerDeath.VictimController` [L:29]
  - Modifiers: public, abstract
- `Sharp.Shared.GameEntities.IPlayerPawn? Sharp.Shared.GameEvents.IEventPlayerDeath.AssisterPawn` [L:38]
  - Modifiers: public, abstract
- `Sharp.Shared.GameEntities.IPlayerPawn? Sharp.Shared.GameEvents.IEventPlayerDeath.KillerPawn` [L:34]
  - Modifiers: public, abstract
- `Sharp.Shared.GameEntities.IPlayerPawn? Sharp.Shared.GameEvents.IEventPlayerDeath.VictimPawn` [L:30]
  - Modifiers: public, abstract
- `Sharp.Shared.Units.UserID Sharp.Shared.GameEvents.IEventPlayerDeath.AssisterUserId` [L:39]
  - Modifiers: public, abstract
- `Sharp.Shared.Units.UserID Sharp.Shared.GameEvents.IEventPlayerDeath.KillerUserId` [L:35]
  - Modifiers: public, abstract
- `Sharp.Shared.Units.UserID Sharp.Shared.GameEvents.IEventPlayerDeath.VictimUserId` [L:31]
  - Modifiers: public, abstract
- `bool Sharp.Shared.GameEvents.IEventPlayerDeath.AssistedFlash` [L:41]
  - Modifiers: public, abstract
- `bool Sharp.Shared.GameEvents.IEventPlayerDeath.AttackerBlind` [L:51]
  - Modifiers: public, abstract
- `bool Sharp.Shared.GameEvents.IEventPlayerDeath.Headshot` [L:43]
  - Modifiers: public, abstract
- `bool Sharp.Shared.GameEvents.IEventPlayerDeath.NoReplay` [L:48]
  - Modifiers: public, abstract
- `bool Sharp.Shared.GameEvents.IEventPlayerDeath.NoScope` [L:49]
  - Modifiers: public, abstract
- `bool Sharp.Shared.GameEvents.IEventPlayerDeath.ThruSmoke` [L:50]
  - Modifiers: public, abstract
- `float Sharp.Shared.GameEvents.IEventPlayerDeath.Distance` [L:52]
  - Modifiers: public, abstract
- `int Sharp.Shared.GameEvents.IEventPlayerDeath.ArmorDamage` [L:55]
  - Modifiers: public, abstract
- `int Sharp.Shared.GameEvents.IEventPlayerDeath.Damage` [L:54]
  - Modifiers: public, abstract
- `short Sharp.Shared.GameEvents.IEventPlayerDeath.Dominated` [L:44]
  - Modifiers: public, abstract
- `short Sharp.Shared.GameEvents.IEventPlayerDeath.Penetrated` [L:47]
  - Modifiers: public, abstract
- `short Sharp.Shared.GameEvents.IEventPlayerDeath.Revenge` [L:45]
  - Modifiers: public, abstract
- `short Sharp.Shared.GameEvents.IEventPlayerDeath.Wipe` [L:46]
  - Modifiers: public, abstract
- `string Sharp.Shared.GameEvents.IEventPlayerDeath.Weapon` [L:42]
  - Modifiers: public, abstract


### interface IEventPlayerHurt : Sharp.Shared.Objects.IGameEvent

- FullName: `Sharp.Shared.GameEvents.IEventPlayerHurt`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameEvents/IEventPlayerHurt.cs:27
- Generated: false

#### Properties
- `Sharp.Shared.Enums.HitGroupType Sharp.Shared.GameEvents.IEventPlayerHurt.HitGroup` [L:42]
  - Modifiers: public, abstract
- `Sharp.Shared.GameEntities.IPlayerController? Sharp.Shared.GameEvents.IEventPlayerHurt.KillerController` [L:33]
  - Modifiers: public, abstract
- `Sharp.Shared.GameEntities.IPlayerController? Sharp.Shared.GameEvents.IEventPlayerHurt.VictimController` [L:29]
  - Modifiers: public, abstract
- `Sharp.Shared.GameEntities.IPlayerPawn? Sharp.Shared.GameEvents.IEventPlayerHurt.KillerPawn` [L:34]
  - Modifiers: public, abstract
- `Sharp.Shared.GameEntities.IPlayerPawn? Sharp.Shared.GameEvents.IEventPlayerHurt.VictimPawn` [L:30]
  - Modifiers: public, abstract
- `Sharp.Shared.Units.UserID Sharp.Shared.GameEvents.IEventPlayerHurt.KillerUserId` [L:35]
  - Modifiers: public, abstract
- `Sharp.Shared.Units.UserID Sharp.Shared.GameEvents.IEventPlayerHurt.VictimUserId` [L:31]
  - Modifiers: public, abstract
- `int Sharp.Shared.GameEvents.IEventPlayerHurt.Armor` [L:38]
  - Modifiers: public, abstract
- `int Sharp.Shared.GameEvents.IEventPlayerHurt.ArmorDamage` [L:41]
  - Modifiers: public, abstract
- `int Sharp.Shared.GameEvents.IEventPlayerHurt.Damage` [L:40]
  - Modifiers: public, abstract
- `int Sharp.Shared.GameEvents.IEventPlayerHurt.Health` [L:37]
  - Modifiers: public, abstract
- `string Sharp.Shared.GameEvents.IEventPlayerHurt.Weapon` [L:39]
  - Modifiers: public, abstract


### interface IEventPlayerJump : Sharp.Shared.Objects.IGameEvent

- FullName: `Sharp.Shared.GameEvents.IEventPlayerJump`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameEvents/IEventPlayerJump.cs:25
- Generated: false

#### Properties
- `Sharp.Shared.GameEntities.IPlayerController? Sharp.Shared.GameEvents.IEventPlayerJump.Controller` [L:27]
  - Modifiers: public, abstract
- `Sharp.Shared.GameEntities.IPlayerPawn? Sharp.Shared.GameEvents.IEventPlayerJump.Pawn` [L:28]
  - Modifiers: public, abstract


### interface IEventPlayerSpawn : Sharp.Shared.Objects.IGameEvent

- FullName: `Sharp.Shared.GameEvents.IEventPlayerSpawn`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameEvents/IEventPlayerSpawn.cs:26
- Generated: false

#### Properties
- `Sharp.Shared.GameEntities.IPlayerController? Sharp.Shared.GameEvents.IEventPlayerSpawn.Controller` [L:28]
  - Modifiers: public, abstract
- `Sharp.Shared.GameEntities.IPlayerPawn? Sharp.Shared.GameEvents.IEventPlayerSpawn.Pawn` [L:29]
  - Modifiers: public, abstract
- `Sharp.Shared.Units.UserID Sharp.Shared.GameEvents.IEventPlayerSpawn.UserId` [L:30]
  - Modifiers: public, abstract


### interface IEventPlayerTeam : Sharp.Shared.Objects.IGameEvent

- FullName: `Sharp.Shared.GameEvents.IEventPlayerTeam`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameEvents/IEventPlayerTeam.cs:27
- Generated: false

#### Properties
- `Sharp.Shared.Enums.CStrikeTeam Sharp.Shared.GameEvents.IEventPlayerTeam.NewTeam` [L:33]
  - Modifiers: public, abstract, readonly
- `Sharp.Shared.Enums.CStrikeTeam Sharp.Shared.GameEvents.IEventPlayerTeam.OldTeam` [L:32]
  - Modifiers: public, abstract, readonly
- `Sharp.Shared.GameEntities.IPlayerController? Sharp.Shared.GameEvents.IEventPlayerTeam.Controller` [L:29]
  - Modifiers: public, abstract
- `Sharp.Shared.Units.UserID Sharp.Shared.GameEvents.IEventPlayerTeam.UserId` [L:30]
  - Modifiers: public, abstract
- `bool Sharp.Shared.GameEvents.IEventPlayerTeam.Bot` [L:37]
  - Modifiers: public, abstract
- `bool Sharp.Shared.GameEvents.IEventPlayerTeam.Disconnect` [L:35]
  - Modifiers: public, abstract
- `bool Sharp.Shared.GameEvents.IEventPlayerTeam.Silent` [L:36]
  - Modifiers: public, abstract


### interface IEventRoundEnd : Sharp.Shared.Objects.IGameEvent

- FullName: `Sharp.Shared.GameEvents.IEventRoundEnd`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameEvents/IEventRoundEnd.cs:25
- Generated: false

#### Properties
- `Sharp.Shared.Enums.CStrikeTeam Sharp.Shared.GameEvents.IEventRoundEnd.Winner` [L:27]
  - Modifiers: public, abstract
- `bool Sharp.Shared.GameEvents.IEventRoundEnd.NoMusic` [L:28]
  - Modifiers: public, abstract


### interface IEventSurvivalRespawnStatus : Sharp.Shared.Objects.IGameEvent

- FullName: `Sharp.Shared.GameEvents.IEventSurvivalRespawnStatus`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameEvents/IEventSurvivalRespawnStatus.cs:26
- Generated: false

#### Properties
- `Sharp.Shared.GameEntities.IPlayerController? Sharp.Shared.GameEvents.IEventSurvivalRespawnStatus.Controller` [L:28]
  - Modifiers: public, abstract
- `Sharp.Shared.GameEntities.IPlayerPawn? Sharp.Shared.GameEvents.IEventSurvivalRespawnStatus.Pawn` [L:29]
  - Modifiers: public, abstract
- `Sharp.Shared.Units.UserID Sharp.Shared.GameEvents.IEventSurvivalRespawnStatus.UserId` [L:30]
  - Modifiers: public, abstract
- `int Sharp.Shared.GameEvents.IEventSurvivalRespawnStatus.Duration` [L:33]
  - Modifiers: public, abstract
- `string Sharp.Shared.GameEvents.IEventSurvivalRespawnStatus.Text` [L:32]
  - Modifiers: public, abstract


### interface IEventWeaponFired : Sharp.Shared.Objects.IGameEvent

- FullName: `Sharp.Shared.GameEvents.IEventWeaponFired`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/GameEvents/IEventWeaponFired.cs:26
- Generated: false

#### Properties
- `Sharp.Shared.GameEntities.IPlayerController? Sharp.Shared.GameEvents.IEventWeaponFired.Controller` [L:28]
  - Modifiers: public, abstract
- `Sharp.Shared.GameEntities.IPlayerPawn? Sharp.Shared.GameEvents.IEventWeaponFired.Pawn` [L:29]
  - Modifiers: public, abstract
- `Sharp.Shared.Units.UserID Sharp.Shared.GameEvents.IEventWeaponFired.UserId` [L:30]
  - Modifiers: public, abstract
- `bool Sharp.Shared.GameEvents.IEventWeaponFired.Silenced` [L:33]
  - Modifiers: public, abstract
- `string Sharp.Shared.GameEvents.IEventWeaponFired.Weapon` [L:32]
  - Modifiers: public, abstract


