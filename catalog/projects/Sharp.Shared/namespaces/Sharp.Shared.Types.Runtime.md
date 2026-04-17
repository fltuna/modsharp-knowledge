# Sharp.Shared.Types.Runtime

Project: Sharp.Shared
Types: 3 (0 generated)

### struct NativeFixedSpan<T> : System.ValueType

- FullName: `Sharp.Shared.Types.Runtime.NativeFixedSpan<T>`
- Kind: struct
- Modifiers: public
- Source: Sharp.Shared/Types/Runtime/NativeSpan.cs:58
- Generated: false
- Attributes: `[StructLayout(0)]`
- Constraint: `where T : struct, unmanaged`

Inheritance: object → System.ValueType → **NativeFixedSpan**

#### Constructors
- `Sharp.Shared.Types.Runtime.NativeFixedSpan<T>.NativeFixedSpan(T* data, int count, int length)` [L:64]

#### Fields
- `int Sharp.Shared.Types.Runtime.NativeFixedSpan<T>.Count` [L:61]
- `readonly T* Sharp.Shared.Types.Runtime.NativeFixedSpan<T>.Data` [L:60]
  - Modifiers: public, readonly
- `readonly int Sharp.Shared.Types.Runtime.NativeFixedSpan<T>.Length` [L:62]
  - Modifiers: public, readonly

#### Indexers
- `T Sharp.Shared.Types.Runtime.NativeFixedSpan<T>.this[int index]` [L:77]

#### Methods
- `readonly System.ReadOnlySpan<T> Sharp.Shared.Types.Runtime.NativeFixedSpan<T>.AsReadOnlySpan()` [L:74]
  - Modifiers: public, readonly
- `readonly System.Span<T> Sharp.Shared.Types.Runtime.NativeFixedSpan<T>.AsSpan()` [L:71]
  - Modifiers: public, readonly
- `void Sharp.Shared.Types.Runtime.NativeFixedSpan<T>.Set(int index, T value)` [L:83]


### struct NativeList<T> : System.ValueType

- FullName: `Sharp.Shared.Types.Runtime.NativeList<T>`
- Kind: struct
- Modifiers: public, readonly
- Source: Sharp.Shared/Types/Runtime/NativeList.cs:26
- Generated: false
- Attributes: `[StructLayout(0)]`
- Constraint: `where T : struct, unmanaged`

Inheritance: object → System.ValueType → **NativeList**

#### Fields
- `readonly int Sharp.Shared.Types.Runtime.NativeList<T>.Count` [L:30]
  - Modifiers: public, readonly

#### Indexers
- `ref T Sharp.Shared.Types.Runtime.NativeList<T>.this[int index]` [L:32]
  - Modifiers: public, readonly

#### Methods
- `System.Collections.Generic.IEnumerator<T> Sharp.Shared.Types.Runtime.NativeList<T>.GetEnumerator()` [L:37]
  - Modifiers: public, readonly
  - Summary: Note: The Enumerator yields copies by value. Use the indexer for by-reference access.


### struct NativeSpan<T> : System.ValueType

- FullName: `Sharp.Shared.Types.Runtime.NativeSpan<T>`
- Kind: struct
- Modifiers: public, readonly
- Source: Sharp.Shared/Types/Runtime/NativeSpan.cs:27
- Generated: false
- Attributes: `[StructLayout(0)]`
- Constraint: `where T : struct, unmanaged`

Inheritance: object → System.ValueType → **NativeSpan**

#### Constructors
- `Sharp.Shared.Types.Runtime.NativeSpan<T>.NativeSpan(T* data, int length)` [L:32]

#### Fields
- `readonly T* Sharp.Shared.Types.Runtime.NativeSpan<T>.Data` [L:29]
  - Modifiers: public, readonly
- `readonly int Sharp.Shared.Types.Runtime.NativeSpan<T>.Length` [L:30]
  - Modifiers: public, readonly

#### Indexers
- `T Sharp.Shared.Types.Runtime.NativeSpan<T>.this[int index]` [L:47]

#### Methods
- `System.Span<T> Sharp.Shared.Types.Runtime.NativeSpan<T>.AsSpan()` [L:44]
  - Modifiers: public, readonly
- `void Sharp.Shared.Types.Runtime.NativeSpan<T>.Set(int index, T value)` [L:53]
  - Modifiers: public, readonly

#### Operators
- `static Sharp.Shared.Types.Runtime.NativeSpan<T>.implicit operator Sharp.Shared.Types.Runtime.NativeSpan<T>(System.Span<T> span)` [L:38]
  - Modifiers: public, static
- `static Sharp.Shared.Types.Runtime.NativeSpan<T>.implicit operator System.Span<T>(Sharp.Shared.Types.Runtime.NativeSpan<T> span)` [L:41]
  - Modifiers: public, static


