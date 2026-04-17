# Sharp.Core.Bridges

Project: Sharp.Core
Types: 2 (0 generated)

### struct ForwardItem : System.ValueType

- FullName: `Sharp.Core.Bridges.ForwardItem`
- Kind: struct
- Modifiers: public
- Source: Sharp.Core/Bridges/Adapter.cs:33
- Generated: false
- Attributes: `[StructLayout(0)]`

Inheritance: object → System.ValueType → **ForwardItem**

#### Fields
- `nint Sharp.Core.Bridges.ForwardItem.Func` [L:36]
- `sbyte* Sharp.Core.Bridges.ForwardItem.Name` [L:35]
- `uint Sharp.Core.Bridges.ForwardItem.InstallCount` [L:37]

#### Properties
- `string Sharp.Core.Bridges.ForwardItem.NameString` [L:39]
  - Modifiers: public, readonly


### struct NativeItem : System.ValueType

- FullName: `Sharp.Core.Bridges.NativeItem`
- Kind: struct
- Modifiers: public
- Source: Sharp.Core/Bridges/Adapter.cs:52
- Generated: false
- Attributes: `[StructLayout(0)]`

Inheritance: object → System.ValueType → **NativeItem**

#### Fields
- `nint Sharp.Core.Bridges.NativeItem.Func` [L:55]
- `sbyte* Sharp.Core.Bridges.NativeItem.Name` [L:54]

#### Properties
- `string Sharp.Core.Bridges.NativeItem.NameString` [L:57]
  - Modifiers: public, readonly


