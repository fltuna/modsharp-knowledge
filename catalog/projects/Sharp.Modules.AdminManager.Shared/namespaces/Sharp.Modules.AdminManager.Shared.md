# Sharp.Modules.AdminManager.Shared

Project: Sharp.Modules.AdminManager.Shared
Types: 6 (0 generated)

### record AdminManifest : System.IEquatable<Sharp.Modules.AdminManager.Shared.AdminManifest>

- FullName: `Sharp.Modules.AdminManager.Shared.AdminManifest`
- Kind: record
- Modifiers: public
- Source: Sharp.Modules/AdminManager/Shared/AdminTableManifest.cs:31
- Generated: false

Inheritance: object → **AdminManifest**

#### Constructors
- `Sharp.Modules.AdminManager.Shared.AdminManifest.AdminManifest(ulong Identity, byte Immunity, System.Collections.Generic.HashSet<string> Permissions)` [L:31]

#### Properties
- `System.Collections.Generic.HashSet<string> Sharp.Modules.AdminManager.Shared.AdminManifest.Permissions` [L:31]
- `byte Sharp.Modules.AdminManager.Shared.AdminManifest.Immunity` [L:31]
- `ulong Sharp.Modules.AdminManager.Shared.AdminManifest.Identity` [L:31]


### record AdminTableManifest : System.IEquatable<Sharp.Modules.AdminManager.Shared.AdminTableManifest>

- FullName: `Sharp.Modules.AdminManager.Shared.AdminTableManifest`
- Kind: record
- Modifiers: public
- Source: Sharp.Modules/AdminManager/Shared/AdminTableManifest.cs:24
- Generated: false

Inheritance: object → **AdminTableManifest**

#### Constructors
- `Sharp.Modules.AdminManager.Shared.AdminTableManifest.AdminTableManifest(System.Collections.Generic.Dictionary<string, System.Collections.Generic.HashSet<string>> PermissionCollection, System.Collections.Generic.List<Sharp.Modules.AdminManager.Shared.RoleManifest> Roles, System.Collections.Generic.List<Sharp.Modules.AdminManager.Shared.AdminManifest> Admins)` [L:24]

#### Properties
- `System.Collections.Generic.Dictionary<string, System.Collections.Generic.HashSet<string>> Sharp.Modules.AdminManager.Shared.AdminTableManifest.PermissionCollection` [L:25]
- `System.Collections.Generic.List<Sharp.Modules.AdminManager.Shared.AdminManifest> Sharp.Modules.AdminManager.Shared.AdminTableManifest.Admins` [L:27]
- `System.Collections.Generic.List<Sharp.Modules.AdminManager.Shared.RoleManifest> Sharp.Modules.AdminManager.Shared.AdminTableManifest.Roles` [L:26]


### interface IAdmin

- FullName: `Sharp.Modules.AdminManager.Shared.IAdmin`
- Kind: interface
- Modifiers: public
- Source: Sharp.Modules/AdminManager/Shared/IAdmin.cs:25
- Generated: false

#### Properties
- `Sharp.Shared.Units.SteamID Sharp.Modules.AdminManager.Shared.IAdmin.Identity` [L:30]
  - Modifiers: public, abstract, readonly
  - Summary: The admin's Steam identity.
- `System.Collections.Generic.IReadOnlySet<string> Sharp.Modules.AdminManager.Shared.IAdmin.Permissions` [L:40]
  - Modifiers: public, abstract, readonly
  - Summary: The resolved set of granted permissions (after merge and deny processing).
- `byte Sharp.Modules.AdminManager.Shared.IAdmin.Immunity` [L:35]
  - Modifiers: public, abstract, readonly
  - Summary: Immunity level (0–255). Higher value = more protection against other admins.

#### Methods
- `bool Sharp.Modules.AdminManager.Shared.IAdmin.HasPermission(string permission)` [L:47]
  - Modifiers: public, abstract
  - Summary: Checks whether this admin has the specified permission.


### interface IAdminCommandRegistry

- FullName: `Sharp.Modules.AdminManager.Shared.IAdminCommandRegistry`
- Kind: interface
- Modifiers: public
- Source: Sharp.Modules/AdminManager/Shared/IAdminCommandRegistry.cs:27
- Generated: false

#### Methods
- `void Sharp.Modules.AdminManager.Shared.IAdminCommandRegistry.RegisterAdminCommand(string command, System.Action<Sharp.Shared.Objects.IGameClient?, Sharp.Shared.Types.StringCommand> call, System.Collections.Immutable.ImmutableArray<string> permissions)` [L:56]
  - Modifiers: public, abstract
  - Summary: Registers an admin-protected command and its required permissions.
- `void Sharp.Modules.AdminManager.Shared.IAdminCommandRegistry.RegisterPermissions(System.Collections.Immutable.ImmutableArray<string> permissions)` [L:73]
  - Modifiers: public, abstract
  - Summary: Registers concrete permissions into the global permission index under this module's scope.


### interface IAdminManager

- FullName: `Sharp.Modules.AdminManager.Shared.IAdminManager`
- Kind: interface
- Modifiers: public
- Source: Sharp.Modules/AdminManager/Shared/IAdminManager.cs:26
- Generated: false

#### Fields
- `const char Sharp.Modules.AdminManager.Shared.IAdminManager.DenyOperator = '!'` [L:29]
  - Modifiers: public, static, const
- `const char Sharp.Modules.AdminManager.Shared.IAdminManager.RolesOperator = '@'` [L:28]
  - Modifiers: public, static, const
- `const char Sharp.Modules.AdminManager.Shared.IAdminManager.SeparatorOperator = ':'` [L:31]
  - Modifiers: public, static, const
- `const char Sharp.Modules.AdminManager.Shared.IAdminManager.WildCardOperator = '*'` [L:30]
  - Modifiers: public, static, const
- `const string Sharp.Modules.AdminManager.Shared.IAdminManager.Identity = "IAdminManager"` [L:33]
  - Modifiers: public, static, const

#### Methods
- `Sharp.Modules.AdminManager.Shared.IAdmin? Sharp.Modules.AdminManager.Shared.IAdminManager.GetAdmin(Sharp.Shared.Units.SteamID identity)` [L:47]
  - Modifiers: public, abstract
  - Summary: Gets the resolved admin snapshot for a Steam identity.
- `Sharp.Modules.AdminManager.Shared.IAdminCommandRegistry Sharp.Modules.AdminManager.Shared.IAdminManager.GetCommandRegistry(string moduleIdentity)` [L:129]
  - Modifiers: public, abstract
  - Summary: Gets the admin command registry for a module scope.
- `void Sharp.Modules.AdminManager.Shared.IAdminManager.MountAdminManifest(string moduleIdentity, System.Func<Sharp.Modules.AdminManager.Shared.AdminTableManifest> call)` [L:107]
  - Modifiers: public, abstract
  - Summary: Mounts (or remounts) one module's admin manifest snapshot into the global admin graph.


### record RoleManifest : System.IEquatable<Sharp.Modules.AdminManager.Shared.RoleManifest>

- FullName: `Sharp.Modules.AdminManager.Shared.RoleManifest`
- Kind: record
- Modifiers: public
- Source: Sharp.Modules/AdminManager/Shared/AdminTableManifest.cs:29
- Generated: false

Inheritance: object → **RoleManifest**

#### Constructors
- `Sharp.Modules.AdminManager.Shared.RoleManifest.RoleManifest(string Name, byte Immunity, System.Collections.Generic.HashSet<string> Permissions)` [L:29]

#### Properties
- `System.Collections.Generic.HashSet<string> Sharp.Modules.AdminManager.Shared.RoleManifest.Permissions` [L:29]
- `byte Sharp.Modules.AdminManager.Shared.RoleManifest.Immunity` [L:29]
- `string Sharp.Modules.AdminManager.Shared.RoleManifest.Name` [L:29]


