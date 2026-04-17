# Sharp.Modules.InputManager.Shared

Project: Sharp.Modules.InputManager.Shared
Types: 4 (0 generated)

### interface IInputListenerRegistry

- FullName: `Sharp.Modules.InputManager.Shared.IInputListenerRegistry`
- Kind: interface
- Modifiers: public
- Source: Sharp.Modules/InputManager/Shared/IInputManager.cs:37
- Generated: false

#### Methods
- `void Sharp.Modules.InputManager.Shared.IInputListenerRegistry.AddCombinationListener(Sharp.Modules.InputManager.Shared.InputKey[] keys, System.Action<Sharp.Shared.Objects.IGameClient> action, [Sharp.Modules.InputManager.Shared.InputState state = Sharp.Modules.InputManager.Shared.InputState.KeyDown])` [L:60]
  - Modifiers: public, abstract
  - Summary: Add a combination key listener (all keys must be pressed simultaneously)
- `void Sharp.Modules.InputManager.Shared.IInputListenerRegistry.AddInputListener(Sharp.Modules.InputManager.Shared.InputKey key, System.Action<Sharp.Shared.Objects.IGameClient> action, [Sharp.Modules.InputManager.Shared.InputState state = Sharp.Modules.InputManager.Shared.InputState.KeyDown], [float holdDuration = 0])` [L:49]
  - Modifiers: public, abstract
  - Summary: Add a single key input listener


### interface IInputManager

- FullName: `Sharp.Modules.InputManager.Shared.IInputManager`
- Kind: interface
- Modifiers: public
- Source: Sharp.Modules/InputManager/Shared/IInputManager.cs:25
- Generated: false

#### Fields
- `const string Sharp.Modules.InputManager.Shared.IInputManager.Identity = "IInputManager"` [L:27]
  - Modifiers: public, static, const

#### Methods
- `Sharp.Modules.InputManager.Shared.IInputListenerRegistry Sharp.Modules.InputManager.Shared.IInputManager.GetInputListenerRegistry(string moduleIdentity)` [L:34]
  - Modifiers: public, abstract
  - Summary: Get or create an input listener registry for a module


### enum InputKey : System.Enum

- FullName: `Sharp.Modules.InputManager.Shared.InputKey`
- Kind: enum
- Modifiers: public
- Source: Sharp.Modules/InputManager/Shared/InputKey.cs:28
- Generated: false
- Summary: Input Keys

Inheritance: object → System.ValueType → System.Enum → **InputKey**

#### Enum Members
- `Sharp.Modules.InputManager.Shared.InputKey.A = 2` [L:32]
  - Modifiers: public, static, const
- `Sharp.Modules.InputManager.Shared.InputKey.Attack1 = 10` [L:40]
  - Modifiers: public, static, const
- `Sharp.Modules.InputManager.Shared.InputKey.Attack2 = 11` [L:41]
  - Modifiers: public, static, const
- `Sharp.Modules.InputManager.Shared.InputKey.D = 3` [L:33]
  - Modifiers: public, static, const
- `Sharp.Modules.InputManager.Shared.InputKey.E = 6` [L:36]
  - Modifiers: public, static, const
- `Sharp.Modules.InputManager.Shared.InputKey.F = 4` [L:34]
  - Modifiers: public, static, const
- `Sharp.Modules.InputManager.Shared.InputKey.R = 7` [L:37]
  - Modifiers: public, static, const
- `Sharp.Modules.InputManager.Shared.InputKey.S = 1` [L:31]
  - Modifiers: public, static, const
- `Sharp.Modules.InputManager.Shared.InputKey.Shift = 9` [L:39]
  - Modifiers: public, static, const
- `Sharp.Modules.InputManager.Shared.InputKey.Space = 8` [L:38]
  - Modifiers: public, static, const
- `Sharp.Modules.InputManager.Shared.InputKey.Tab = 5` [L:35]
  - Modifiers: public, static, const
- `Sharp.Modules.InputManager.Shared.InputKey.W = 0` [L:30]
  - Modifiers: public, static, const

#### Obsolete Members
- `Sharp.Modules.InputManager.Shared.InputKey.F3 = 12` [L:44] — Currently does nothing. It will be implemented in the future release. This is just a placeholder.
- `Sharp.Modules.InputManager.Shared.InputKey.F4 = 13` [L:47] — Currently does nothing. It will be implemented in the future release. This is just a placeholder.
- `Sharp.Modules.InputManager.Shared.InputKey.G = 14` [L:50] — Currently does nothing. It will be implemented in the future release. This is just a placeholder.


### enum InputState : System.Enum

- FullName: `Sharp.Modules.InputManager.Shared.InputState`
- Kind: enum
- Modifiers: public
- Source: Sharp.Modules/InputManager/Shared/InputState.cs:25
- Generated: false
- Summary: Defines different states of key input

Inheritance: object → System.ValueType → System.Enum → **InputState**

#### Enum Members
- `Sharp.Modules.InputManager.Shared.InputState.KeyDown = 0` [L:30]
  - Modifiers: public, static, const
  - Summary: Key was just pressed this frame
- `Sharp.Modules.InputManager.Shared.InputState.KeyHold = 1` [L:35]
  - Modifiers: public, static, const
  - Summary: Key is being held down
- `Sharp.Modules.InputManager.Shared.InputState.KeyUp = 2` [L:40]
  - Modifiers: public, static, const
  - Summary: Key was just released this frame


