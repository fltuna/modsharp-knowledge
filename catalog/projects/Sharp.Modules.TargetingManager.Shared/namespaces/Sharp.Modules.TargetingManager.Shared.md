# Sharp.Modules.TargetingManager.Shared

Project: Sharp.Modules.TargetingManager.Shared
Types: 3 (0 generated)

### interface ITargetResolver

- FullName: `Sharp.Modules.TargetingManager.Shared.ITargetResolver`
- Kind: interface
- Modifiers: public
- Source: Sharp.Modules/TargetingManager/Shared/ITargetResolver.cs:25
- Generated: false

#### Methods
- `System.Collections.Generic.IEnumerable<Sharp.Shared.Objects.IGameClient> Sharp.Modules.TargetingManager.Shared.ITargetResolver.Resolve(Sharp.Shared.Objects.IGameClient? activator)` [L:29]
  - Modifiers: public, abstract
- `string Sharp.Modules.TargetingManager.Shared.ITargetResolver.GetTarget()` [L:27]
  - Modifiers: public, abstract


### interface ITargetingManager

- FullName: `Sharp.Modules.TargetingManager.Shared.ITargetingManager`
- Kind: interface
- Modifiers: public
- Source: Sharp.Modules/TargetingManager/Shared/ITargetingManager.cs:25
- Generated: false

#### Fields
- `const string Sharp.Modules.TargetingManager.Shared.ITargetingManager.Identity = "ITargetingManager"` [L:27]
  - Modifiers: public, static, const

#### Methods
- `System.Collections.Generic.IEnumerable<Sharp.Shared.Objects.IGameClient> Sharp.Modules.TargetingManager.Shared.ITargetingManager.GetByTarget(Sharp.Shared.Objects.IGameClient? activator, string target)` [L:50]
  - Modifiers: public, abstract
  - Summary: Resolves a target string into a list of game clients.
- `bool Sharp.Modules.TargetingManager.Shared.ITargetingManager.RegisterResolver(string ownerIdentity, Sharp.Modules.TargetingManager.Shared.ITargetResolver resolver)` [L:61]
  - Modifiers: public, abstract
  - Summary: Register a custom target resolver.


### class PredefinedTargets

- FullName: `Sharp.Modules.TargetingManager.Shared.PredefinedTargets`
- Kind: class
- Modifiers: public, static
- Source: Sharp.Modules/TargetingManager/Shared/PredefinedTargets.cs:22
- Generated: false

Inheritance: object → **PredefinedTargets**

#### Fields
- `const string Sharp.Modules.TargetingManager.Shared.PredefinedTargets.Aim = "@aim"` [L:27]
  - Modifiers: public, static, const
- `const string Sharp.Modules.TargetingManager.Shared.PredefinedTargets.Alive = "@alive"` [L:33]
  - Modifiers: public, static, const
- `const string Sharp.Modules.TargetingManager.Shared.PredefinedTargets.All = "@all"` [L:24]
  - Modifiers: public, static, const
- `const string Sharp.Modules.TargetingManager.Shared.PredefinedTargets.Bots = "@bots"` [L:39]
  - Modifiers: public, static, const
- `const string Sharp.Modules.TargetingManager.Shared.PredefinedTargets.Ct = "@ct"` [L:29]
  - Modifiers: public, static, const
- `const string Sharp.Modules.TargetingManager.Shared.PredefinedTargets.Dead = "@dead"` [L:34]
  - Modifiers: public, static, const
- `const string Sharp.Modules.TargetingManager.Shared.PredefinedTargets.Me = "@me"` [L:36]
  - Modifiers: public, static, const
- `const string Sharp.Modules.TargetingManager.Shared.PredefinedTargets.None = "@!all"` [L:25]
  - Modifiers: public, static, const
- `const string Sharp.Modules.TargetingManager.Shared.PredefinedTargets.NotMe = "@!me"` [L:37]
  - Modifiers: public, static, const
- `const string Sharp.Modules.TargetingManager.Shared.PredefinedTargets.Spec = "@spec"` [L:31]
  - Modifiers: public, static, const
- `const string Sharp.Modules.TargetingManager.Shared.PredefinedTargets.T = "@t"` [L:30]
  - Modifiers: public, static, const


