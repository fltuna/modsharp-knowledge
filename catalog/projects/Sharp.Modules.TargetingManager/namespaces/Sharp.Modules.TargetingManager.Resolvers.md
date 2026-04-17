# Sharp.Modules.TargetingManager.Resolvers

Project: Sharp.Modules.TargetingManager
Types: 11 (0 generated)

### class Alive : Sharp.Modules.TargetingManager.Resolvers.BaseResolver

- FullName: `Sharp.Modules.TargetingManager.Resolvers.Alive`
- Kind: class
- Modifiers: public, sealed
- Source: Sharp.Modules/TargetingManager/src/Resolvers/Alive.cs:26
- Generated: false

Inheritance: object → Sharp.Modules.TargetingManager.Resolvers.BaseResolver → **Alive**

#### Constructors
- `Sharp.Modules.TargetingManager.Resolvers.Alive.Alive(Sharp.Shared.ISharedSystem sharedSystem)` [L:28]

#### Methods
- `override System.Collections.Generic.IEnumerable<Sharp.Shared.Objects.IGameClient> Sharp.Modules.TargetingManager.Resolvers.Alive.Resolve(Sharp.Shared.Objects.IGameClient? activator)` [L:35]
  - Modifiers: public, override
- `override string Sharp.Modules.TargetingManager.Resolvers.Alive.GetTarget()` [L:32]
  - Modifiers: public, override


### class All : Sharp.Modules.TargetingManager.Resolvers.BaseResolver

- FullName: `Sharp.Modules.TargetingManager.Resolvers.All`
- Kind: class
- Modifiers: public, sealed
- Source: Sharp.Modules/TargetingManager/src/Resolvers/All.cs:26
- Generated: false

Inheritance: object → Sharp.Modules.TargetingManager.Resolvers.BaseResolver → **All**

#### Constructors
- `Sharp.Modules.TargetingManager.Resolvers.All.All(Sharp.Shared.ISharedSystem sharedSystem)` [L:28]

#### Methods
- `override System.Collections.Generic.IEnumerable<Sharp.Shared.Objects.IGameClient> Sharp.Modules.TargetingManager.Resolvers.All.Resolve(Sharp.Shared.Objects.IGameClient? activator)` [L:35]
  - Modifiers: public, override
- `override string Sharp.Modules.TargetingManager.Resolvers.All.GetTarget()` [L:32]
  - Modifiers: public, override


### class BaseResolver : Sharp.Modules.TargetingManager.Shared.ITargetResolver

- FullName: `Sharp.Modules.TargetingManager.Resolvers.BaseResolver`
- Kind: class
- Modifiers: public, abstract
- Source: Sharp.Modules/TargetingManager/src/Resolvers/Base.cs:27
- Generated: false

Inheritance: object → **BaseResolver**

#### Constructors
- `Sharp.Modules.TargetingManager.Resolvers.BaseResolver.BaseResolver(Sharp.Shared.ISharedSystem sharedSystem)` [L:33]
  - Modifiers: protected

#### Fields
- `readonly Sharp.Shared.Managers.IClientManager Sharp.Modules.TargetingManager.Resolvers.BaseResolver.ClientManager` [L:29]
  - Modifiers: protected, readonly
- `readonly Sharp.Shared.Managers.IEntityManager Sharp.Modules.TargetingManager.Resolvers.BaseResolver.EntityManager` [L:30]
  - Modifiers: protected, readonly
- `readonly Sharp.Shared.Managers.IPhysicsQueryManager Sharp.Modules.TargetingManager.Resolvers.BaseResolver.PhysicsQueryManager` [L:31]
  - Modifiers: protected, readonly

#### Methods
- `abstract System.Collections.Generic.IEnumerable<Sharp.Shared.Objects.IGameClient> Sharp.Modules.TargetingManager.Resolvers.BaseResolver.Resolve(Sharp.Shared.Objects.IGameClient? activator)` [L:42]
  - Modifiers: public, abstract
- `abstract string Sharp.Modules.TargetingManager.Resolvers.BaseResolver.GetTarget()` [L:40]
  - Modifiers: public, abstract


### class Bots : Sharp.Modules.TargetingManager.Resolvers.BaseResolver

- FullName: `Sharp.Modules.TargetingManager.Resolvers.Bots`
- Kind: class
- Modifiers: public, sealed
- Source: Sharp.Modules/TargetingManager/src/Resolvers/Bots.cs:26
- Generated: false

Inheritance: object → Sharp.Modules.TargetingManager.Resolvers.BaseResolver → **Bots**

#### Constructors
- `Sharp.Modules.TargetingManager.Resolvers.Bots.Bots(Sharp.Shared.ISharedSystem sharedSystem)` [L:28]

#### Methods
- `override System.Collections.Generic.IEnumerable<Sharp.Shared.Objects.IGameClient> Sharp.Modules.TargetingManager.Resolvers.Bots.Resolve(Sharp.Shared.Objects.IGameClient? activator)` [L:35]
  - Modifiers: public, override
- `override string Sharp.Modules.TargetingManager.Resolvers.Bots.GetTarget()` [L:32]
  - Modifiers: public, override


### class Ct : Sharp.Modules.TargetingManager.Resolvers.BaseResolver

- FullName: `Sharp.Modules.TargetingManager.Resolvers.Ct`
- Kind: class
- Modifiers: public, sealed
- Source: Sharp.Modules/TargetingManager/src/Resolvers/Ct.cs:27
- Generated: false

Inheritance: object → Sharp.Modules.TargetingManager.Resolvers.BaseResolver → **Ct**

#### Constructors
- `Sharp.Modules.TargetingManager.Resolvers.Ct.Ct(Sharp.Shared.ISharedSystem sharedSystem)` [L:29]

#### Methods
- `override System.Collections.Generic.IEnumerable<Sharp.Shared.Objects.IGameClient> Sharp.Modules.TargetingManager.Resolvers.Ct.Resolve(Sharp.Shared.Objects.IGameClient? activator)` [L:36]
  - Modifiers: public, override
- `override string Sharp.Modules.TargetingManager.Resolvers.Ct.GetTarget()` [L:33]
  - Modifiers: public, override


### class Dead : Sharp.Modules.TargetingManager.Resolvers.BaseResolver

- FullName: `Sharp.Modules.TargetingManager.Resolvers.Dead`
- Kind: class
- Modifiers: public, sealed
- Source: Sharp.Modules/TargetingManager/src/Resolvers/Dead.cs:26
- Generated: false

Inheritance: object → Sharp.Modules.TargetingManager.Resolvers.BaseResolver → **Dead**

#### Constructors
- `Sharp.Modules.TargetingManager.Resolvers.Dead.Dead(Sharp.Shared.ISharedSystem sharedSystem)` [L:28]

#### Methods
- `override System.Collections.Generic.IEnumerable<Sharp.Shared.Objects.IGameClient> Sharp.Modules.TargetingManager.Resolvers.Dead.Resolve(Sharp.Shared.Objects.IGameClient? activator)` [L:35]
  - Modifiers: public, override
- `override string Sharp.Modules.TargetingManager.Resolvers.Dead.GetTarget()` [L:32]
  - Modifiers: public, override


### class Me : Sharp.Modules.TargetingManager.Resolvers.BaseResolver

- FullName: `Sharp.Modules.TargetingManager.Resolvers.Me`
- Kind: class
- Modifiers: public, sealed
- Source: Sharp.Modules/TargetingManager/src/Resolvers/Me.cs:26
- Generated: false

Inheritance: object → Sharp.Modules.TargetingManager.Resolvers.BaseResolver → **Me**

#### Constructors
- `Sharp.Modules.TargetingManager.Resolvers.Me.Me(Sharp.Shared.ISharedSystem sharedSystem)` [L:28]

#### Methods
- `override System.Collections.Generic.IEnumerable<Sharp.Shared.Objects.IGameClient> Sharp.Modules.TargetingManager.Resolvers.Me.Resolve(Sharp.Shared.Objects.IGameClient? activator)` [L:35]
  - Modifiers: public, override
- `override string Sharp.Modules.TargetingManager.Resolvers.Me.GetTarget()` [L:32]
  - Modifiers: public, override


### class None : Sharp.Modules.TargetingManager.Resolvers.BaseResolver

- FullName: `Sharp.Modules.TargetingManager.Resolvers.None`
- Kind: class
- Modifiers: public, sealed
- Source: Sharp.Modules/TargetingManager/src/Resolvers/None.cs:26
- Generated: false

Inheritance: object → Sharp.Modules.TargetingManager.Resolvers.BaseResolver → **None**

#### Constructors
- `Sharp.Modules.TargetingManager.Resolvers.None.None(Sharp.Shared.ISharedSystem sharedSystem)` [L:28]

#### Methods
- `override System.Collections.Generic.IEnumerable<Sharp.Shared.Objects.IGameClient> Sharp.Modules.TargetingManager.Resolvers.None.Resolve(Sharp.Shared.Objects.IGameClient? activator)` [L:35]
  - Modifiers: public, override
- `override string Sharp.Modules.TargetingManager.Resolvers.None.GetTarget()` [L:32]
  - Modifiers: public, override


### class NotMe : Sharp.Modules.TargetingManager.Resolvers.BaseResolver

- FullName: `Sharp.Modules.TargetingManager.Resolvers.NotMe`
- Kind: class
- Modifiers: public, sealed
- Source: Sharp.Modules/TargetingManager/src/Resolvers/NotMe.cs:26
- Generated: false

Inheritance: object → Sharp.Modules.TargetingManager.Resolvers.BaseResolver → **NotMe**

#### Constructors
- `Sharp.Modules.TargetingManager.Resolvers.NotMe.NotMe(Sharp.Shared.ISharedSystem sharedSystem)` [L:28]

#### Methods
- `override System.Collections.Generic.IEnumerable<Sharp.Shared.Objects.IGameClient> Sharp.Modules.TargetingManager.Resolvers.NotMe.Resolve(Sharp.Shared.Objects.IGameClient? activator)` [L:35]
  - Modifiers: public, override
- `override string Sharp.Modules.TargetingManager.Resolvers.NotMe.GetTarget()` [L:32]
  - Modifiers: public, override


### class Spec : Sharp.Modules.TargetingManager.Resolvers.BaseResolver

- FullName: `Sharp.Modules.TargetingManager.Resolvers.Spec`
- Kind: class
- Modifiers: public, sealed
- Source: Sharp.Modules/TargetingManager/src/Resolvers/Spec.cs:27
- Generated: false

Inheritance: object → Sharp.Modules.TargetingManager.Resolvers.BaseResolver → **Spec**

#### Constructors
- `Sharp.Modules.TargetingManager.Resolvers.Spec.Spec(Sharp.Shared.ISharedSystem sharedSystem)` [L:29]

#### Methods
- `override System.Collections.Generic.IEnumerable<Sharp.Shared.Objects.IGameClient> Sharp.Modules.TargetingManager.Resolvers.Spec.Resolve(Sharp.Shared.Objects.IGameClient? handler)` [L:36]
  - Modifiers: public, override
- `override string Sharp.Modules.TargetingManager.Resolvers.Spec.GetTarget()` [L:33]
  - Modifiers: public, override


### class Te : Sharp.Modules.TargetingManager.Resolvers.BaseResolver

- FullName: `Sharp.Modules.TargetingManager.Resolvers.Te`
- Kind: class
- Modifiers: public, sealed
- Source: Sharp.Modules/TargetingManager/src/Resolvers/Te.cs:27
- Generated: false

Inheritance: object → Sharp.Modules.TargetingManager.Resolvers.BaseResolver → **Te**

#### Constructors
- `Sharp.Modules.TargetingManager.Resolvers.Te.Te(Sharp.Shared.ISharedSystem sharedSystem)` [L:29]

#### Methods
- `override System.Collections.Generic.IEnumerable<Sharp.Shared.Objects.IGameClient> Sharp.Modules.TargetingManager.Resolvers.Te.Resolve(Sharp.Shared.Objects.IGameClient? handler)` [L:36]
  - Modifiers: public, override
- `override string Sharp.Modules.TargetingManager.Resolvers.Te.GetTarget()` [L:33]
  - Modifiers: public, override


