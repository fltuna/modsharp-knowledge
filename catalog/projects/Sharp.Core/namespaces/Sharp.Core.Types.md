# Sharp.Core.Types

Project: Sharp.Core
Types: 2 (0 generated)

### struct EntityKeyValuesVariant : System.ValueType

- FullName: `Sharp.Core.Types.EntityKeyValuesVariant`
- Kind: struct
- Modifiers: public
- Source: Sharp.Core/Types/EntityKeyValuesVariant.cs:27
- Generated: false
- Attributes: `[StructLayout(2, Size = 24)]`

Inheritance: object → System.ValueType → **EntityKeyValuesVariant**

#### Constructors
- `Sharp.Core.Types.EntityKeyValuesVariant.EntityKeyValuesVariant(string key, in Sharp.Shared.Types.KeyValuesVariantValueItem value)` [L:35]

#### Fields
- `Sharp.Core.Types.EntityKeyValuesVariantValue Sharp.Core.Types.EntityKeyValuesVariant.Value` [L:33]
  - Attributes: `[FieldOffset(8)]`
- `byte* Sharp.Core.Types.EntityKeyValuesVariant.Key` [L:30]
  - Attributes: `[FieldOffset(0)]`

#### Methods
- `void Sharp.Core.Types.EntityKeyValuesVariant.Update(string key, in Sharp.Shared.Types.KeyValuesVariantValueItem value)` [L:41]


### struct EntityKeyValuesVariantValue : System.ValueType

- FullName: `Sharp.Core.Types.EntityKeyValuesVariantValue`
- Kind: struct
- Modifiers: public, readonly
- Source: Sharp.Core/Types/EntityKeyValuesVariantValue.cs:29
- Generated: false
- Attributes: `[StructLayout(2, Size = 16)]`

Inheritance: object → System.ValueType → **EntityKeyValuesVariantValue**

#### Operators
- `static Sharp.Core.Types.EntityKeyValuesVariantValue.implicit operator Sharp.Core.Types.EntityKeyValuesVariantValue(Sharp.Shared.Types.KeyValuesVariantValueItem item)` [L:49]
  - Modifiers: public, static


