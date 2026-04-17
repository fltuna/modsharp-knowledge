# Sharp.Shared.CStrike

Project: Sharp.Shared
Types: 14 (0 generated)

### interface IContextObject

- FullName: `Sharp.Shared.CStrike.IContextObject`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/CStrike/INativeObject.cs:9
- Generated: false

#### Properties
- `bool Sharp.Shared.CStrike.IContextObject.IsDisposed` [L:15]
  - Modifiers: public, abstract, readonly
  - Summary: Check if the pointer is no longer valid within the current context.


### interface IEntityComponent : Sharp.Shared.CStrike.ISchemaObject

- FullName: `Sharp.Shared.CStrike.IEntityComponent`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/CStrike/IEntityComponent.cs:24
- Generated: false

#### Properties
- `Sharp.Shared.GameEntities.IBaseEntity? Sharp.Shared.CStrike.IEntityComponent.ChainEntity` [L:34]
  - Modifiers: public, abstract, readonly
  - Summary: Schema Chain Entity
- `int Sharp.Shared.CStrike.IEntityComponent.ChainOffset` [L:29]
  - Modifiers: public, abstract, readonly
  - Summary: Schema Chain Offset


### interface IEntityObject : Sharp.Shared.CStrike.ISchemaObject

- FullName: `Sharp.Shared.CStrike.IEntityObject`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/CStrike/IEntityComponent.cs:37
- Generated: false


### interface IEntitySubclassVData : Sharp.Shared.CStrike.ISchemaObject

- FullName: `Sharp.Shared.CStrike.IEntitySubclassVData`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/CStrike/IEntitySubclassVData.cs:22
- Generated: false

#### Properties
- `string Sharp.Shared.CStrike.IEntitySubclassVData.Classname` [L:32]
  - Modifiers: public, abstract, readonly
  - Summary: VData classname
- `string Sharp.Shared.CStrike.IEntitySubclassVData.Key` [L:27]
  - Modifiers: public, abstract, readonly
  - Summary: Key in vdata file


### interface INativeCreatable<T>

- FullName: `Sharp.Shared.CStrike.INativeCreatable<T>`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/CStrike/INativeObject.cs:30
- Generated: false

#### Methods
- `T? Sharp.Shared.CStrike.INativeCreatable<out T>.Create(nint ptr)` [L:32]
  - Modifiers: public, static, abstract


### interface INativeObject : Sharp.Shared.CStrike.IContextObject, System.IEquatable<Sharp.Shared.CStrike.INativeObject>

- FullName: `Sharp.Shared.CStrike.INativeObject`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/CStrike/INativeObject.cs:18
- Generated: false

#### Methods
- `bool Sharp.Shared.CStrike.INativeObject.Equals(object? obj)` [L:27]
  - Modifiers: public, abstract
- `int Sharp.Shared.CStrike.INativeObject.GetHashCode()` [L:25]
  - Modifiers: public, abstract
- `nint Sharp.Shared.CStrike.INativeObject.GetAbsPtr()` [L:23]
  - Modifiers: public, abstract
  - Summary: Get pointer address


### interface INativeSizeable

- FullName: `Sharp.Shared.CStrike.INativeSizeable`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/CStrike/INativeObject.cs:35
- Generated: false

#### Properties
- `uint Sharp.Shared.CStrike.INativeSizeable.NativeSize` [L:37]
  - Modifiers: public, static, abstract, readonly


### interface ISchemaArray<T> : Sharp.Shared.CStrike.INativeObject

- FullName: `Sharp.Shared.CStrike.ISchemaArray<T>`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/CStrike/ISchemaArray.cs:25
- Generated: false
- Constraint: `where T : struct, unmanaged`

#### Properties
- `int Sharp.Shared.CStrike.ISchemaArray<T>.Size` [L:30]
  - Modifiers: public, abstract, readonly
  - Summary: Array size

#### Indexers
- `T Sharp.Shared.CStrike.ISchemaArray<T>.this[int index]` [L:35]
  - Modifiers: public, abstract
  - Summary: Indexer

#### Methods
- `Sharp.Shared.CStrike.ISchemaArray<T>.Enumerator Sharp.Shared.CStrike.ISchemaArray<T>.GetEnumerator()` [L:52]
  - Modifiers: public, abstract
  - Summary: You typically don't need to use this, as it provides zero-allocation enumeration for foreach
- `System.Collections.Generic.IEnumerator<T> Sharp.Shared.CStrike.ISchemaArray<T>.AsEnumerable()` [L:46]
  - Modifiers: public, abstract
  - Summary: Converts to  for use with Linq/ZLinq
- `ref T Sharp.Shared.CStrike.ISchemaArray<T>.GetRef(int index)` [L:41]
  - Modifiers: public, abstract
  - Summary: Gets a reference to the element at the specified Use the ref keyword


### struct Enumerator : System.ValueType, System.Collections.Generic.IEnumerator<T>

- FullName: `Sharp.Shared.CStrike.ISchemaArray<T>.Enumerator`
- Kind: struct
- Modifiers: public
- Source: Sharp.Shared/CStrike/ISchemaArray.cs:57
- Generated: false
- Summary: You don't need to use this directly

Inheritance: object → System.ValueType → **Enumerator**

#### Constructors
- `Sharp.Shared.CStrike.ISchemaArray<T>.Enumerator.Enumerator(Sharp.Shared.CStrike.ISchemaArray<T> array)` [L:62]

#### Properties
- `T Sharp.Shared.CStrike.ISchemaArray<T>.Enumerator.Current` [L:68]
  - Modifiers: public, readonly

#### Methods
- `bool Sharp.Shared.CStrike.ISchemaArray<T>.Enumerator.MoveNext()` [L:72]
- `void Sharp.Shared.CStrike.ISchemaArray<T>.Enumerator.Dispose()` [L:78]
- `void Sharp.Shared.CStrike.ISchemaArray<T>.Enumerator.Reset()` [L:75]


### interface ISchemaEmbeddedList<T> : Sharp.Shared.CStrike.INativeObject

- FullName: `Sharp.Shared.CStrike.ISchemaEmbeddedList<T>`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/CStrike/ISchemaEmbeddedList.cs:25
- Generated: false

#### Properties
- `int Sharp.Shared.CStrike.ISchemaEmbeddedList<T>.Count` [L:30]
  - Modifiers: public, abstract, readonly
  - Summary: The number of elements

#### Indexers
- `T Sharp.Shared.CStrike.ISchemaEmbeddedList<T>.this[int index]` [L:35]
  - Modifiers: public, abstract
  - Summary: Indexer

#### Methods
- `Sharp.Shared.CStrike.ISchemaEmbeddedList<T>.Enumerator Sharp.Shared.CStrike.ISchemaEmbeddedList<T>.GetEnumerator()` [L:46]
  - Modifiers: public, abstract
  - Summary: You typically don't need to use this, as it provides zero-allocation enumeration for foreach
- `System.Collections.Generic.IEnumerator<T> Sharp.Shared.CStrike.ISchemaEmbeddedList<T>.AsEnumerable()` [L:40]
  - Modifiers: public, abstract
  - Summary: Convert to  for use with Linq/ZLinq


### struct Enumerator : System.ValueType, System.Collections.Generic.IEnumerator<T>

- FullName: `Sharp.Shared.CStrike.ISchemaEmbeddedList<T>.Enumerator`
- Kind: struct
- Modifiers: public
- Source: Sharp.Shared/CStrike/ISchemaEmbeddedList.cs:51
- Generated: false
- Summary: You don't need to use this

Inheritance: object → System.ValueType → **Enumerator**

#### Constructors
- `Sharp.Shared.CStrike.ISchemaEmbeddedList<T>.Enumerator.Enumerator(Sharp.Shared.CStrike.ISchemaEmbeddedList<T> list)` [L:56]

#### Properties
- `T Sharp.Shared.CStrike.ISchemaEmbeddedList<T>.Enumerator.Current` [L:62]
  - Modifiers: public, readonly

#### Methods
- `bool Sharp.Shared.CStrike.ISchemaEmbeddedList<T>.Enumerator.MoveNext()` [L:66]
- `void Sharp.Shared.CStrike.ISchemaEmbeddedList<T>.Enumerator.Dispose()` [L:72]
- `void Sharp.Shared.CStrike.ISchemaEmbeddedList<T>.Enumerator.Reset()` [L:69]


### interface ISchemaList<T> : Sharp.Shared.CStrike.INativeObject

- FullName: `Sharp.Shared.CStrike.ISchemaList<T>`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/CStrike/ISchemaList.cs:26
- Generated: false
- Constraint: `where T : struct, unmanaged`

#### Properties
- `int Sharp.Shared.CStrike.ISchemaList<T>.Count` [L:31]
  - Modifiers: public, abstract, readonly
  - Summary: Number of elements

#### Indexers
- `T Sharp.Shared.CStrike.ISchemaList<T>.this[int index]` [L:36]
  - Modifiers: public, abstract
  - Summary: Indexer

#### Methods
- `Sharp.Shared.CStrike.ISchemaList<T>.Enumerator Sharp.Shared.CStrike.ISchemaList<T>.GetEnumerator()` [L:58]
  - Modifiers: public, abstract
  - Summary: You typically don't need to use this, as it provides zero-allocation enumeration for foreach
- `Sharp.Shared.Types.Tier.CUtlVector<T>* Sharp.Shared.CStrike.ISchemaList<T>.GetUtlVector()` [L:47]
  - Modifiers: public, abstract
  - Summary: Gets the  pointer
- `System.Collections.Generic.IEnumerator<T> Sharp.Shared.CStrike.ISchemaList<T>.AsEnumerable()` [L:52]
  - Modifiers: public, abstract
  - Summary: Converts to  for use with Linq/ZLinq
- `ref T Sharp.Shared.CStrike.ISchemaList<T>.GetRef(int index)` [L:42]
  - Modifiers: public, abstract
  - Summary: Gets a reference to the element at the specified Use the ref keyword
- `void Sharp.Shared.CStrike.ISchemaList<T>.SetStateChanged()` [L:63]
  - Modifiers: public, abstract
  - Summary: Invokes Schema StateChanged


### struct Enumerator : System.ValueType, System.Collections.Generic.IEnumerator<T>

- FullName: `Sharp.Shared.CStrike.ISchemaList<T>.Enumerator`
- Kind: struct
- Modifiers: public
- Source: Sharp.Shared/CStrike/ISchemaList.cs:68
- Generated: false
- Summary: You don't need to use this

Inheritance: object → System.ValueType → **Enumerator**

#### Constructors
- `Sharp.Shared.CStrike.ISchemaList<T>.Enumerator.Enumerator(Sharp.Shared.CStrike.ISchemaList<T> list)` [L:73]

#### Properties
- `T Sharp.Shared.CStrike.ISchemaList<T>.Enumerator.Current` [L:79]
  - Modifiers: public, readonly

#### Methods
- `bool Sharp.Shared.CStrike.ISchemaList<T>.Enumerator.MoveNext()` [L:83]
- `void Sharp.Shared.CStrike.ISchemaList<T>.Enumerator.Dispose()` [L:89]
- `void Sharp.Shared.CStrike.ISchemaList<T>.Enumerator.Reset()` [L:86]


### interface ISchemaObject : Sharp.Shared.CStrike.INativeObject

- FullName: `Sharp.Shared.CStrike.ISchemaObject`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/CStrike/ISchemaObject.cs:26
- Generated: false

#### Methods
- `Sharp.Shared.CStrike.ISchemaArray<T> Sharp.Shared.CStrike.ISchemaObject.GetSchemaFixedArray<T>(string fieldName, [ushort extraOffset = 0]) where T : unmanaged` [L:128]
  - Modifiers: public, abstract
  - Summary: Gets the value of a Schema member variable
- `Sharp.Shared.CStrike.ISchemaList<T> Sharp.Shared.CStrike.ISchemaObject.GetSchemaList<T>(string fieldName, [bool isStruct = false], [ushort extraOffset = 0]) where T : unmanaged` [L:134]
  - Modifiers: public, abstract
  - Summary: Gets the value of a Schema member variable
- `Sharp.Shared.Types.Vector Sharp.Shared.CStrike.ISchemaObject.GetNetVar<T>(string fieldName, [ushort extraOffset = 0], [Sharp.Shared.Types.Vector? _ = null]) where T : System.IComparable<Sharp.Shared.Types.Vector>` [L:102]
  - Modifiers: public, abstract
  - Summary: Gets the value of a Schema member variable
- `bool Sharp.Shared.CStrike.ISchemaObject.FindNetVar(string field)` [L:257]
  - Modifiers: public, abstract
  - Summary: Checks if a Schema member variable exists
- `bool Sharp.Shared.CStrike.ISchemaObject.GetNetVar<T>(string fieldName, [ushort extraOffset = 0], [bool? _ = null]) where T : System.IComparable<bool>` [L:36]
  - Modifiers: public, abstract
  - Summary: Gets the value of a Schema member variable
- `byte Sharp.Shared.CStrike.ISchemaObject.GetNetVar<T>(string fieldName, [ushort extraOffset = 0], [byte? _ = null]) where T : System.IComparable<byte>` [L:42]
  - Modifiers: public, abstract
  - Summary: Gets the value of a Schema member variable
- `float Sharp.Shared.CStrike.ISchemaObject.GetNetVar<T>(string fieldName, [ushort extraOffset = 0], [float? _ = null]) where T : System.IComparable<float>` [L:84]
  - Modifiers: public, abstract
  - Summary: Gets the value of a Schema member variable
- `int Sharp.Shared.CStrike.ISchemaObject.GetNetVar<T>(string fieldName, [ushort extraOffset = 0], [int? _ = null]) where T : System.IComparable<int>` [L:60]
  - Modifiers: public, abstract
  - Summary: Gets the value of a Schema member variable
- `int Sharp.Shared.CStrike.ISchemaObject.GetNetVarOffset(string field)` [L:263]
  - Modifiers: public, abstract
  - Summary: Gets the offset of a Schema member variable
- `long Sharp.Shared.CStrike.ISchemaObject.GetNetVar<T>(string fieldName, [ushort extraOffset = 0], [long? _ = null]) where T : System.IComparable<long>` [L:72]
  - Modifiers: public, abstract
  - Summary: Gets the value of a Schema member variable
- `nint Sharp.Shared.CStrike.ISchemaObject.GetNetVar<T>(string fieldName, [ushort extraOffset = 0], [nint? _ = null]) where T : System.IComparable<nint>` [L:90]
  - Modifiers: public, abstract
  - Summary: Gets the value of a Schema member variable
- `ref Sharp.Shared.Types.Tier.CUtlString Sharp.Shared.CStrike.ISchemaObject.GetNetVarUtlStringRef(string fieldName, [ushort extraOffset = 0])` [L:123]
  - Modifiers: public, abstract
  - Summary: Gets the value of a Schema member variable
- `ref Sharp.Shared.Types.Tier.CUtlSymbolLarge Sharp.Shared.CStrike.ISchemaObject.GetNetVarUtlSymbolLargeRef(string fieldName, [ushort extraOffset = 0])` [L:113]
  - Modifiers: public, abstract
  - Summary: Gets the value of a Schema member variable
- `short Sharp.Shared.CStrike.ISchemaObject.GetNetVar<T>(string fieldName, [ushort extraOffset = 0], [short? _ = null]) where T : System.IComparable<short>` [L:48]
  - Modifiers: public, abstract
  - Summary: Gets the value of a Schema member variable
- `string Sharp.Shared.CStrike.ISchemaObject.GetNetVar<T>(string fieldName, [ushort extraOffset = 0], [string? _ = null]) where T : System.IComparable<string>` [L:96]
  - Modifiers: public, abstract
  - Summary: Gets the value of a Schema member variable
- `string Sharp.Shared.CStrike.ISchemaObject.GetNetVarUtlString(string fieldName, [ushort extraOffset = 0])` [L:118]
  - Modifiers: public, abstract
  - Summary: Gets the value of a Schema member variable
- `string Sharp.Shared.CStrike.ISchemaObject.GetNetVarUtlSymbolLarge(string fieldName, [ushort extraOffset = 0])` [L:108]
  - Modifiers: public, abstract
  - Summary: Gets the value of a Schema member variable
- `string Sharp.Shared.CStrike.ISchemaObject.GetSchemaClassname()` [L:31]
  - Modifiers: public, abstract
  - Summary: Gets the Schema DynamicBinding
- `uint Sharp.Shared.CStrike.ISchemaObject.GetNetVar<T>(string fieldName, [ushort extraOffset = 0], [uint? _ = null]) where T : System.IComparable<uint>` [L:66]
  - Modifiers: public, abstract
  - Summary: Gets the value of a Schema member variable
- `ulong Sharp.Shared.CStrike.ISchemaObject.GetNetVar<T>(string fieldName, [ushort extraOffset = 0], [ulong? _ = null]) where T : System.IComparable<ulong>` [L:78]
  - Modifiers: public, abstract
  - Summary: Gets the value of a Schema member variable
- `ushort Sharp.Shared.CStrike.ISchemaObject.GetNetVar<T>(string fieldName, [ushort extraOffset = 0], [ushort? _ = null]) where T : System.IComparable<ushort>` [L:54]
  - Modifiers: public, abstract
  - Summary: Gets the value of a Schema member variable
- `void Sharp.Shared.CStrike.ISchemaObject.NetworkStateChanged(string field, [bool isStruct = false], [ushort extraOffset = 0])` [L:268]
  - Modifiers: public, abstract
  - Summary: Automatically calls NetworkStateChanged or StateChanged
- `void Sharp.Shared.CStrike.ISchemaObject.SetNetVar(string field, Sharp.Shared.Types.Vector value, [bool isStruct = false], [ushort extraOffset = 0])` [L:234]
  - Modifiers: public, abstract
  - Summary: Sets the value of a Schema member
- `void Sharp.Shared.CStrike.ISchemaObject.SetNetVar(string field, bool value, [bool isStruct = false], [ushort extraOffset = 0])` [L:144]
  - Modifiers: public, abstract
  - Summary: Sets the value of a Schema member
- `void Sharp.Shared.CStrike.ISchemaObject.SetNetVar(string field, byte value, [bool isStruct = false], [ushort extraOffset = 0])` [L:153]
  - Modifiers: public, abstract
  - Summary: Sets the value of a Schema member
- `void Sharp.Shared.CStrike.ISchemaObject.SetNetVar(string field, float value, [bool isStruct = false], [ushort extraOffset = 0])` [L:216]
  - Modifiers: public, abstract
  - Summary: Sets the value of a Schema member
- `void Sharp.Shared.CStrike.ISchemaObject.SetNetVar(string field, int value, [bool isStruct = false], [ushort extraOffset = 0])` [L:180]
  - Modifiers: public, abstract
  - Summary: Sets the value of a Schema member
- `void Sharp.Shared.CStrike.ISchemaObject.SetNetVar(string field, long value, [bool isStruct = false], [ushort extraOffset = 0])` [L:198]
  - Modifiers: public, abstract
  - Summary: Sets the value of a Schema member
- `void Sharp.Shared.CStrike.ISchemaObject.SetNetVar(string field, short value, [bool isStruct = false], [ushort extraOffset = 0])` [L:162]
  - Modifiers: public, abstract
  - Summary: Sets the value of a Schema member
- `void Sharp.Shared.CStrike.ISchemaObject.SetNetVar(string field, string value, int maxLen, [bool isStruct = false], [ushort extraOffset = 0])` [L:225]
  - Modifiers: public, abstract
  - Summary: Sets the value of a Schema member
- `void Sharp.Shared.CStrike.ISchemaObject.SetNetVar(string field, uint value, [bool isStruct = false], [ushort extraOffset = 0])` [L:189]
  - Modifiers: public, abstract
  - Summary: Sets the value of a Schema member
- `void Sharp.Shared.CStrike.ISchemaObject.SetNetVar(string field, ulong value, [bool isStruct = false], [ushort extraOffset = 0])` [L:207]
  - Modifiers: public, abstract
  - Summary: Sets the value of a Schema member
- `void Sharp.Shared.CStrike.ISchemaObject.SetNetVar(string field, ushort value, [bool isStruct = false], [ushort extraOffset = 0])` [L:171]
  - Modifiers: public, abstract
  - Summary: Sets the value of a Schema member
- `void Sharp.Shared.CStrike.ISchemaObject.SetNetVarUtlString(string field, string value, [bool isStruct = false], [ushort extraOffset = 0])` [L:251]
  - Modifiers: public, abstract
  - Summary: Sets the value of a Schema member
- `void Sharp.Shared.CStrike.ISchemaObject.SetNetVarUtlSymbolLarge(string field, string value, [bool isStruct = false], [ushort extraOffset = 0])` [L:243]
  - Modifiers: public, abstract
  - Summary: Sets the value of a Schema member


