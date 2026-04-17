# Sharp.Core.Bridges.Forwards.Extern

Project: Sharp.Core
Types: 8 (0 generated)

### class GiveNamedItem

- FullName: `Sharp.Core.Bridges.Forwards.Extern.GiveNamedItem`
- Kind: class
- Modifiers: public, static
- Source: Sharp.Core/Bridges/Forwards/Extern/GiveNamedItem.cs:29
- Generated: false

Inheritance: object → **GiveNamedItem**

#### Methods
- `static Sharp.Shared.Enums.EHookAction Sharp.Core.Bridges.Forwards.Extern.GiveNamedItem.OnCanAcquirePreExport(nint ptrClient, nint ptrController, nint ptrPawn, ushort itemIndex, Sharp.Shared.Enums.EAcquireMethod method, Sharp.Shared.Enums.EAcquireResult* acquireResult)` [L:114]
  - Modifiers: public, static
  - Attributes: `[UnmanagedCallersOnly]`
- `static Sharp.Shared.Enums.EHookAction Sharp.Core.Bridges.Forwards.Extern.GiveNamedItem.OnGiveNamedItemPreExport(nint ptrClient, nint ptrController, nint ptrPawn, sbyte* ptrClassname, bool* ignoredCEconItemView)` [L:63]
  - Modifiers: public, static
  - Attributes: `[UnmanagedCallersOnly]`
- `static void Sharp.Core.Bridges.Forwards.Extern.GiveNamedItem.OnGiveGloveItemPostExport(nint ptrClient, nint ptrController, nint ptrPawn)` [L:110]
  - Modifiers: public, static
  - Attributes: `[UnmanagedCallersOnly]`
- `static void Sharp.Core.Bridges.Forwards.Extern.GiveNamedItem.OnGiveNamedItemPostExport(nint ptrClient, nint ptrController, nint ptrPawn, sbyte* ptrClassname, byte ignoredCEconItemView, Sharp.Shared.Enums.EHookAction hookAction, nint returnValue)` [L:95]
  - Modifiers: public, static
  - Attributes: `[UnmanagedCallersOnly]`

#### Events
- `static Sharp.Core.Bridges.Forwards.Extern.GiveNamedItem.DelegateCanAcquirePre? Sharp.Core.Bridges.Forwards.Extern.GiveNamedItem.OnCanAcquirePre` [L:58]
  - Modifiers: public, static
- `static Sharp.Core.Bridges.Forwards.Extern.GiveNamedItem.DelegateGiveGloveItemPost? Sharp.Core.Bridges.Forwards.Extern.GiveNamedItem.OnGiveGloveItemPost` [L:60]
  - Modifiers: public, static
- `static Sharp.Core.Bridges.Forwards.Extern.GiveNamedItem.DelegateGiveNamedItemPost? Sharp.Core.Bridges.Forwards.Extern.GiveNamedItem.OnGiveNamedItemPost` [L:56]
  - Modifiers: public, static
- `static Sharp.Core.Bridges.Forwards.Extern.GiveNamedItem.DelegateGiveNamedItemPre? Sharp.Core.Bridges.Forwards.Extern.GiveNamedItem.OnGiveNamedItemPre` [L:54]
  - Modifiers: public, static


### delegate DelegateCanAcquirePre : System.MulticastDelegate

- FullName: `Sharp.Core.Bridges.Forwards.Extern.GiveNamedItem.DelegateCanAcquirePre`
- Kind: delegate
- Modifiers: public, sealed
- Source: Sharp.Core/Bridges/Forwards/Extern/GiveNamedItem.cs:45
- Generated: false
- Invoke: `virtual Sharp.Shared.Types.HookReturnValue<Sharp.Shared.Enums.EAcquireResult> Sharp.Core.Bridges.Forwards.Extern.GiveNamedItem.DelegateCanAcquirePre.Invoke(nint ptrClient, nint ptrController, nint ptrPawn, ushort itemIndex, Sharp.Shared.Enums.EAcquireMethod acquireMethod, Sharp.Shared.Enums.EAcquireResult defaultResult)`

Inheritance: object → System.Delegate → System.MulticastDelegate → **DelegateCanAcquirePre**


### delegate DelegateGiveGloveItemPost : System.MulticastDelegate

- FullName: `Sharp.Core.Bridges.Forwards.Extern.GiveNamedItem.DelegateGiveGloveItemPost`
- Kind: delegate
- Modifiers: public, sealed
- Source: Sharp.Core/Bridges/Forwards/Extern/GiveNamedItem.cs:52
- Generated: false
- Invoke: `virtual void Sharp.Core.Bridges.Forwards.Extern.GiveNamedItem.DelegateGiveGloveItemPost.Invoke(nint ptrClient, nint ptrController, nint ptrPawn)`

Inheritance: object → System.Delegate → System.MulticastDelegate → **DelegateGiveGloveItemPost**


### delegate DelegateGiveNamedItemPost : System.MulticastDelegate

- FullName: `Sharp.Core.Bridges.Forwards.Extern.GiveNamedItem.DelegateGiveNamedItemPost`
- Kind: delegate
- Modifiers: public, sealed
- Source: Sharp.Core/Bridges/Forwards/Extern/GiveNamedItem.cs:37
- Generated: false
- Invoke: `virtual void Sharp.Core.Bridges.Forwards.Extern.GiveNamedItem.DelegateGiveNamedItemPost.Invoke(nint ptrClient, nint ptrController, nint ptrPawn, string classname, bool ignoredCEconItemView, Sharp.Shared.Enums.EHookAction hookAction, nint returnValue)`

Inheritance: object → System.Delegate → System.MulticastDelegate → **DelegateGiveNamedItemPost**


### delegate DelegateGiveNamedItemPre : System.MulticastDelegate

- FullName: `Sharp.Core.Bridges.Forwards.Extern.GiveNamedItem.DelegateGiveNamedItemPre`
- Kind: delegate
- Modifiers: public, sealed
- Source: Sharp.Core/Bridges/Forwards/Extern/GiveNamedItem.cs:31
- Generated: false
- Invoke: `virtual Sharp.Shared.Types.HookReturnValue<Sharp.Shared.GameEntities.IBaseWeapon> Sharp.Core.Bridges.Forwards.Extern.GiveNamedItem.DelegateGiveNamedItemPre.Invoke(nint ptrClient, nint ptrController, nint ptrPawn, ref string classname, ref bool ignoredCEconItemView)`

Inheritance: object → System.Delegate → System.MulticastDelegate → **DelegateGiveNamedItemPre**


### class HandleCommandJoinTeam

- FullName: `Sharp.Core.Bridges.Forwards.Extern.HandleCommandJoinTeam`
- Kind: class
- Modifiers: public, static
- Source: Sharp.Core/Bridges/Forwards/Extern/HandleCommandJoinTeam.cs:27
- Generated: false

Inheritance: object → **HandleCommandJoinTeam**

#### Methods
- `static Sharp.Shared.Enums.EHookAction Sharp.Core.Bridges.Forwards.Extern.HandleCommandJoinTeam.OnHandleCommandJoinTeamPreExport(nint ptrClient, nint ptrController, int* pTeam, bool* pQueue, int* pCoachTeam, bool* returnValue)` [L:48]
  - Modifiers: public, static
  - Attributes: `[UnmanagedCallersOnly]`
- `static void Sharp.Core.Bridges.Forwards.Extern.HandleCommandJoinTeam.OnHandleCommandJoinTeamPostExport(nint ptrClient, nint ptrController, int team, byte queue, int coachTeam, Sharp.Shared.Enums.EHookAction hookAction, byte returnValue)` [L:82]
  - Modifiers: public, static
  - Attributes: `[UnmanagedCallersOnly]`

#### Events
- `static Sharp.Core.Bridges.Forwards.Extern.HandleCommandJoinTeam.DelegateHandleCommandJoinTeamPost? Sharp.Core.Bridges.Forwards.Extern.HandleCommandJoinTeam.OnHandleCommandJoinTeamPost` [L:45]
  - Modifiers: public, static
- `static Sharp.Core.Bridges.Forwards.Extern.HandleCommandJoinTeam.DelegateHandleCommandJoinTeamPre? Sharp.Core.Bridges.Forwards.Extern.HandleCommandJoinTeam.OnHandleCommandJoinTeamPre` [L:43]
  - Modifiers: public, static


### delegate DelegateHandleCommandJoinTeamPost : System.MulticastDelegate

- FullName: `Sharp.Core.Bridges.Forwards.Extern.HandleCommandJoinTeam.DelegateHandleCommandJoinTeamPost`
- Kind: delegate
- Modifiers: public, sealed
- Source: Sharp.Core/Bridges/Forwards/Extern/HandleCommandJoinTeam.cs:35
- Generated: false
- Invoke: `virtual void Sharp.Core.Bridges.Forwards.Extern.HandleCommandJoinTeam.DelegateHandleCommandJoinTeamPost.Invoke(nint ptrClient, nint pController, int team, bool queue, int coachTeam, Sharp.Shared.Enums.EHookAction hookAction, bool returnValue)`

Inheritance: object → System.Delegate → System.MulticastDelegate → **DelegateHandleCommandJoinTeamPost**


### delegate DelegateHandleCommandJoinTeamPre : System.MulticastDelegate

- FullName: `Sharp.Core.Bridges.Forwards.Extern.HandleCommandJoinTeam.DelegateHandleCommandJoinTeamPre`
- Kind: delegate
- Modifiers: public, sealed
- Source: Sharp.Core/Bridges/Forwards/Extern/HandleCommandJoinTeam.cs:29
- Generated: false
- Invoke: `virtual Sharp.Shared.Types.HookReturnValue<bool> Sharp.Core.Bridges.Forwards.Extern.HandleCommandJoinTeam.DelegateHandleCommandJoinTeamPre.Invoke(nint ptrClient, nint ptrController, ref int team, ref bool queue, ref int coachTeam)`

Inheritance: object → System.Delegate → System.MulticastDelegate → **DelegateHandleCommandJoinTeamPre**


