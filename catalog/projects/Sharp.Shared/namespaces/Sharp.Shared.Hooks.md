# Sharp.Shared.Hooks

Project: Sharp.Shared
Types: 6 (0 generated)

### interface IDetourHook : Sharp.Shared.Hooks.IRuntimeNativeHook, System.IDisposable

- FullName: `Sharp.Shared.Hooks.IDetourHook`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/Hooks/IDetourHook.cs:25
- Generated: false

#### Methods
- `void Sharp.Shared.Hooks.IDetourHook.Prepare(nint pTargetFn, nint hookFn)` [L:49]
  - Modifiers: public, abstract
  - Summary: Prepare Hook
- `void Sharp.Shared.Hooks.IDetourHook.Prepare(string gamedata, nint hookFn)` [L:34]
  - Modifiers: public, abstract
  - Summary: Prepare hook


### interface IMidFuncHook : Sharp.Shared.Hooks.IRuntimeNativeHook, System.IDisposable

- FullName: `Sharp.Shared.Hooks.IMidFuncHook`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/Hooks/IMidFuncHook.cs:106
- Generated: false

#### Methods
- `void Sharp.Shared.Hooks.IMidFuncHook.Prepare(nint pTargetFn, nint hookFn)` [L:130]
  - Modifiers: public, abstract
  - Summary: Prepare Hook
- `void Sharp.Shared.Hooks.IMidFuncHook.Prepare(string gamedata, nint hookFn)` [L:115]
  - Modifiers: public, abstract
  - Summary: Prepare hook


### interface IRuntimeNativeHook

- FullName: `Sharp.Shared.Hooks.IRuntimeNativeHook`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/Hooks/IRuntimeNativeHook.cs:22
- Generated: false

#### Properties
- `nint Sharp.Shared.Hooks.IRuntimeNativeHook.Trampoline` [L:37]
  - Modifiers: public, abstract, readonly
  - Summary: Original address

#### Methods
- `bool Sharp.Shared.Hooks.IRuntimeNativeHook.Install()` [L:27]
  - Modifiers: public, abstract
  - Summary: Install hook
- `void Sharp.Shared.Hooks.IRuntimeNativeHook.Uninstall()` [L:32]
  - Modifiers: public, abstract
  - Summary: Uninstall hook


### interface IVirtualHook : Sharp.Shared.Hooks.IRuntimeNativeHook

- FullName: `Sharp.Shared.Hooks.IVirtualHook`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/Hooks/IVirtualHook.cs:25
- Generated: false

#### Methods
- `void Sharp.Shared.Hooks.IVirtualHook.Prepare(nint vTable, int offset, nint hookFn)` [L:57]
  - Modifiers: public, abstract
  - Summary: Prepare Hook
- `void Sharp.Shared.Hooks.IVirtualHook.Prepare(string module, string @class, int offset, nint hookFn)` [L:47]
  - Modifiers: public, abstract
  - Summary: Prepare Hook
- `void Sharp.Shared.Hooks.IVirtualHook.Prepare(string module, string @class, string function, nint hookFn)` [L:36]
  - Modifiers: public, abstract
  - Summary: Prepare Hook


### struct MidHookContext : System.ValueType

- FullName: `Sharp.Shared.Hooks.MidHookContext`
- Kind: struct
- Modifiers: public
- Source: Sharp.Shared/Hooks/IMidFuncHook.cs:66
- Generated: false
- Attributes: `[StructLayout(0, Size = 408, Pack = 8)]`
- Summary: Context structure for 64-bit MidHook.

Inheritance: object → System.ValueType → **MidHookContext**

#### Fields
- `Sharp.Shared.Hooks.Xmm Sharp.Shared.Hooks.MidHookContext.xmm0` [L:68]
- `Sharp.Shared.Hooks.Xmm Sharp.Shared.Hooks.MidHookContext.xmm1` [L:69]
- `Sharp.Shared.Hooks.Xmm Sharp.Shared.Hooks.MidHookContext.xmm10` [L:78]
- `Sharp.Shared.Hooks.Xmm Sharp.Shared.Hooks.MidHookContext.xmm11` [L:79]
- `Sharp.Shared.Hooks.Xmm Sharp.Shared.Hooks.MidHookContext.xmm12` [L:80]
- `Sharp.Shared.Hooks.Xmm Sharp.Shared.Hooks.MidHookContext.xmm13` [L:81]
- `Sharp.Shared.Hooks.Xmm Sharp.Shared.Hooks.MidHookContext.xmm14` [L:82]
- `Sharp.Shared.Hooks.Xmm Sharp.Shared.Hooks.MidHookContext.xmm15` [L:83]
- `Sharp.Shared.Hooks.Xmm Sharp.Shared.Hooks.MidHookContext.xmm2` [L:70]
- `Sharp.Shared.Hooks.Xmm Sharp.Shared.Hooks.MidHookContext.xmm3` [L:71]
- `Sharp.Shared.Hooks.Xmm Sharp.Shared.Hooks.MidHookContext.xmm4` [L:72]
- `Sharp.Shared.Hooks.Xmm Sharp.Shared.Hooks.MidHookContext.xmm5` [L:73]
- `Sharp.Shared.Hooks.Xmm Sharp.Shared.Hooks.MidHookContext.xmm6` [L:74]
- `Sharp.Shared.Hooks.Xmm Sharp.Shared.Hooks.MidHookContext.xmm7` [L:75]
- `Sharp.Shared.Hooks.Xmm Sharp.Shared.Hooks.MidHookContext.xmm8` [L:76]
- `Sharp.Shared.Hooks.Xmm Sharp.Shared.Hooks.MidHookContext.xmm9` [L:77]
- `nint Sharp.Shared.Hooks.MidHookContext.r10` [L:91]
- `nint Sharp.Shared.Hooks.MidHookContext.r11` [L:90]
- `nint Sharp.Shared.Hooks.MidHookContext.r12` [L:89]
- `nint Sharp.Shared.Hooks.MidHookContext.r13` [L:88]
- `nint Sharp.Shared.Hooks.MidHookContext.r14` [L:87]
- `nint Sharp.Shared.Hooks.MidHookContext.r15` [L:86]
- `nint Sharp.Shared.Hooks.MidHookContext.r8` [L:93]
- `nint Sharp.Shared.Hooks.MidHookContext.r9` [L:92]
- `nint Sharp.Shared.Hooks.MidHookContext.rax` [L:99]
- `nint Sharp.Shared.Hooks.MidHookContext.rbp` [L:100]
- `nint Sharp.Shared.Hooks.MidHookContext.rbx` [L:98]
- `nint Sharp.Shared.Hooks.MidHookContext.rcx` [L:97]
- `nint Sharp.Shared.Hooks.MidHookContext.rdi` [L:94]
- `nint Sharp.Shared.Hooks.MidHookContext.rdx` [L:96]
- `nint Sharp.Shared.Hooks.MidHookContext.rflags` [L:85]
- `nint Sharp.Shared.Hooks.MidHookContext.rip` [L:103]
- `nint Sharp.Shared.Hooks.MidHookContext.rsi` [L:95]
- `nint Sharp.Shared.Hooks.MidHookContext.rsp` [L:101]
- `nint Sharp.Shared.Hooks.MidHookContext.trampoline_rsp` [L:102]


### struct Xmm : System.ValueType

- FullName: `Sharp.Shared.Hooks.Xmm`
- Kind: struct
- Modifiers: public
- Source: Sharp.Shared/Hooks/IMidFuncHook.cs:27
- Generated: false
- Attributes: `[StructLayout(2, Size = 16, Pack = 8)]`

Inheritance: object → System.ValueType → **Xmm**

#### Fields
- `byte* Sharp.Shared.Hooks.Xmm.U8` [L:30]
  - Attributes: `[FieldOffset(0)]`
- `double* Sharp.Shared.Hooks.Xmm.F64` [L:45]
  - Attributes: `[FieldOffset(0)]`
- `float* Sharp.Shared.Hooks.Xmm.F32` [L:42]
  - Attributes: `[FieldOffset(0)]`
- `ulong* Sharp.Shared.Hooks.Xmm.U64` [L:39]
  - Attributes: `[FieldOffset(0)]`
- `ushort* Sharp.Shared.Hooks.Xmm.U16` [L:33]
  - Attributes: `[FieldOffset(0)]`
- `ushort* Sharp.Shared.Hooks.Xmm.U32` [L:36]
  - Attributes: `[FieldOffset(0)]`


