# Sharp.Shared.Types.Tier

Project: Sharp.Shared
Types: 7 (0 generated)

### struct CUtlLeanVectorBase<T, I> : System.ValueType, System.Collections.Generic.IEnumerable<T>, System.IDisposable

- FullName: `Sharp.Shared.Types.Tier.CUtlLeanVectorBase<T, I>`
- Kind: struct
- Modifiers: public
- Source: Sharp.Shared/Types/Tier/CUtlLeanVector.cs:31
- Generated: false
- Attributes: `[StructLayout(0, Pack = 8)]`
- Constraint: `where T : struct, unmanaged`
- Constraint: `where I : struct, unmanaged, System.Numerics.IBinaryInteger<I>, System.Numerics.IMinMaxValue<I>`

Inheritance: object → System.ValueType → **CUtlLeanVectorBase**

#### Properties
- `bool Sharp.Shared.Types.Tier.CUtlLeanVectorBase<T, I>.IsExternallyAllocated` [L:41]
  - Modifiers: public, readonly
- `int Sharp.Shared.Types.Tier.CUtlLeanVectorBase<T, I>.Count` [L:38]
  - Modifiers: public, readonly
- `int Sharp.Shared.Types.Tier.CUtlLeanVectorBase<T, I>.NumAllocated` [L:40]
  - Modifiers: public, readonly
- `int Sharp.Shared.Types.Tier.CUtlLeanVectorBase<T, I>.Size` [L:39]
  - Modifiers: public, readonly

#### Indexers
- `System.Span<T> Sharp.Shared.Types.Tier.CUtlLeanVectorBase<T, I>.this[System.Range range]` [L:51]
  - Modifiers: public, readonly
- `ref T Sharp.Shared.Types.Tier.CUtlLeanVectorBase<T, I>.this[System.Index index]` [L:49]
  - Modifiers: public, readonly

#### Methods
- `Sharp.Shared.Types.Tier.CUtlLeanVectorBase<T, I>.Enumerator Sharp.Shared.Types.Tier.CUtlLeanVectorBase<T, I>.GetEnumerator()` [L:314]
- `System.ReadOnlySpan<T> Sharp.Shared.Types.Tier.CUtlLeanVectorBase<T, I>.AsReadOnlySpan()` [L:46]
- `System.Span<T> Sharp.Shared.Types.Tier.CUtlLeanVectorBase<T, I>.AsSpan()` [L:43]
- `T* Sharp.Shared.Types.Tier.CUtlLeanVectorBase<T, I>.AddToTailGetPtr()` [L:173]
- `T* Sharp.Shared.Types.Tier.CUtlLeanVectorBase<T, I>.Base()` [L:60]
- `ref T Sharp.Shared.Types.Tier.CUtlLeanVectorBase<T, I>.AddToTailGetRef()` [L:161]
- `void Sharp.Shared.Types.Tier.CUtlLeanVectorBase<T, I>.Add(T item)` [L:155]
- `void Sharp.Shared.Types.Tier.CUtlLeanVectorBase<T, I>.Add(ref readonly T item)` [L:158]
- `void Sharp.Shared.Types.Tier.CUtlLeanVectorBase<T, I>.AddToTail(T value)` [L:140]
- `void Sharp.Shared.Types.Tier.CUtlLeanVectorBase<T, I>.AddToTail(ref T value)` [L:143]
- `void Sharp.Shared.Types.Tier.CUtlLeanVectorBase<T, I>.Dispose()` [L:55]
- `void Sharp.Shared.Types.Tier.CUtlLeanVectorBase<T, I>.EnsureCapacity(int num, [bool force = false])` [L:76]
- `void Sharp.Shared.Types.Tier.CUtlLeanVectorBase<T, I>.Insert(int index, T item)` [L:185]
- `void Sharp.Shared.Types.Tier.CUtlLeanVectorBase<T, I>.Purge()` [L:63]
- `void Sharp.Shared.Types.Tier.CUtlLeanVectorBase<T, I>.Remove(int index)` [L:224]
- `void Sharp.Shared.Types.Tier.CUtlLeanVectorBase<T, I>.RemoveAll()` [L:214]


### struct Enumerator : System.ValueType, System.Collections.Generic.IEnumerator<T>, System.Collections.IEnumerator

- FullName: `Sharp.Shared.Types.Tier.CUtlLeanVectorBase<T, I>.Enumerator`
- Kind: struct
- Modifiers: public
- Source: Sharp.Shared/Types/Tier/CUtlLeanVector.cs:282
- Generated: false

Inheritance: object → System.ValueType → **Enumerator**

#### Constructors
- `Sharp.Shared.Types.Tier.CUtlLeanVectorBase<T, I>.Enumerator.Enumerator(Sharp.Shared.Types.Tier.CUtlLeanVectorBase<T, I> vector)` [L:287]

#### Properties
- `T Sharp.Shared.Types.Tier.CUtlLeanVectorBase<T, I>.Enumerator.Current` [L:305]
  - Modifiers: public, readonly

#### Methods
- `bool Sharp.Shared.Types.Tier.CUtlLeanVectorBase<T, I>.Enumerator.MoveNext()` [L:293]
- `void Sharp.Shared.Types.Tier.CUtlLeanVectorBase<T, I>.Enumerator.Dispose()` [L:309]
- `void Sharp.Shared.Types.Tier.CUtlLeanVectorBase<T, I>.Enumerator.Reset()` [L:300]


### struct CUtlMemory<T> : System.ValueType, System.IDisposable

- FullName: `Sharp.Shared.Types.Tier.CUtlMemory<T>`
- Kind: struct
- Modifiers: public
- Source: Sharp.Shared/Types/Tier/CUtlMemory.cs:27
- Generated: false
- Attributes: `[StructLayout(0)]`
- Constraint: `where T : struct, unmanaged`

Inheritance: object → System.ValueType → **CUtlMemory**

#### Constructors
- `Sharp.Shared.Types.Tier.CUtlMemory<T>.CUtlMemory(int growSize, int initAllocationCount)` [L:41]

#### Properties
- `bool Sharp.Shared.Types.Tier.CUtlMemory<T>.IsExternallyAllocated` [L:39]
  - Modifiers: public, readonly
- `bool Sharp.Shared.Types.Tier.CUtlMemory<T>.IsReadOnly` [L:38]
  - Modifiers: public, readonly
- `int Sharp.Shared.Types.Tier.CUtlMemory<T>.AllocationCount` [L:37]
  - Modifiers: public, readonly

#### Indexers
- `ref T Sharp.Shared.Types.Tier.CUtlMemory<T>.this[long index]` [L:66]
  - Modifiers: public, readonly

#### Methods
- `System.ReadOnlySpan<T> Sharp.Shared.Types.Tier.CUtlMemory<T>.AsReadOnlySpan()` [L:63]
- `System.Span<T> Sharp.Shared.Types.Tier.CUtlMemory<T>.AsSpan()` [L:60]
- `T* Sharp.Shared.Types.Tier.CUtlMemory<T>.Base()` [L:57]
- `void Sharp.Shared.Types.Tier.CUtlMemory<T>.Dispose()` [L:52]
- `void Sharp.Shared.Types.Tier.CUtlMemory<T>.EnsureCapacity(int num)` [L:162]
- `void Sharp.Shared.Types.Tier.CUtlMemory<T>.Grow(int num)` [L:182]
- `void Sharp.Shared.Types.Tier.CUtlMemory<T>.Purge()` [L:108]
- `void Sharp.Shared.Types.Tier.CUtlMemory<T>.Purge(int numElements)` [L:120]


### struct CUtlString : System.ValueType, System.IDisposable

- FullName: `Sharp.Shared.Types.Tier.CUtlString`
- Kind: struct
- Modifiers: public
- Source: Sharp.Shared/Types/Tier/CUtlString.cs:31
- Generated: false
- Attributes: `[StructLayout(0, Pack = 8, Size = 8)]`

Inheritance: object → System.ValueType → **CUtlString**

#### Constructors
- `Sharp.Shared.Types.Tier.CUtlString.CUtlString(byte* str)` [L:40]
- `Sharp.Shared.Types.Tier.CUtlString.CUtlString(string str)` [L:35]

#### Methods
- `System.ReadOnlySpan<byte> Sharp.Shared.Types.Tier.CUtlString.AsReadOnlySpan()` [L:49]
- `System.Span<byte> Sharp.Shared.Types.Tier.CUtlString.AsSpan()` [L:52]
- `bool Sharp.Shared.Types.Tier.CUtlString.IsEmpty()` [L:122]
  - Attributes: `[MethodImpl(256)]`
- `int Sharp.Shared.Types.Tier.CUtlString.Length()` [L:104]
  - Attributes: `[MethodImpl(256)]`
- `string Sharp.Shared.Types.Tier.CUtlString.Get()` [L:46]
- `void Sharp.Shared.Types.Tier.CUtlString.Dispose()` [L:55]
- `void Sharp.Shared.Types.Tier.CUtlString.SetString(string str)` [L:61]

#### Operators
- `static Sharp.Shared.Types.Tier.CUtlString.implicit operator Sharp.Shared.Types.Tier.CUtlString(byte* pString)` [L:43]
  - Modifiers: public, static


### struct CUtlSymbolLarge : System.ValueType, System.IComparable<Sharp.Shared.Types.Tier.CUtlSymbolLarge>, System.IEquatable<Sharp.Shared.Types.Tier.CUtlSymbolLarge>

- FullName: `Sharp.Shared.Types.Tier.CUtlSymbolLarge`
- Kind: struct
- Modifiers: public, readonly
- Source: Sharp.Shared/Types/Tier/CUtlSymbolLarge.cs:28
- Generated: false
- Attributes: `[StructLayout(0, Pack = 8, Size = 8)]`

Inheritance: object → System.ValueType → **CUtlSymbolLarge**

#### Constructors
- `Sharp.Shared.Types.Tier.CUtlSymbolLarge.CUtlSymbolLarge()` [L:32]
- `Sharp.Shared.Types.Tier.CUtlSymbolLarge.CUtlSymbolLarge(nint value)` [L:35]

#### Methods
- `bool Sharp.Shared.Types.Tier.CUtlSymbolLarge.Equals(Sharp.Shared.Types.Tier.CUtlSymbolLarge other)` [L:56]
  - Modifiers: public, readonly
- `int Sharp.Shared.Types.Tier.CUtlSymbolLarge.CompareTo(Sharp.Shared.Types.Tier.CUtlSymbolLarge other)` [L:53]
  - Modifiers: public, readonly
- `override bool Sharp.Shared.Types.Tier.CUtlSymbolLarge.Equals(object? obj)` [L:59]
  - Modifiers: public, override, readonly
- `override int Sharp.Shared.Types.Tier.CUtlSymbolLarge.GetHashCode()` [L:69]
  - Modifiers: public, override, readonly
- `string Sharp.Shared.Types.Tier.CUtlSymbolLarge.Get()` [L:38]
  - Modifiers: public, readonly

#### Operators
- `static bool Sharp.Shared.Types.Tier.CUtlSymbolLarge.operator !=(Sharp.Shared.Types.Tier.CUtlSymbolLarge lv, Sharp.Shared.Types.Tier.CUtlSymbolLarge rv)` [L:44]
  - Modifiers: public, static
- `static bool Sharp.Shared.Types.Tier.CUtlSymbolLarge.operator <(Sharp.Shared.Types.Tier.CUtlSymbolLarge lv, Sharp.Shared.Types.Tier.CUtlSymbolLarge rv)` [L:47]
  - Modifiers: public, static
- `static bool Sharp.Shared.Types.Tier.CUtlSymbolLarge.operator ==(Sharp.Shared.Types.Tier.CUtlSymbolLarge lv, Sharp.Shared.Types.Tier.CUtlSymbolLarge rv)` [L:41]
  - Modifiers: public, static
- `static bool Sharp.Shared.Types.Tier.CUtlSymbolLarge.operator >(Sharp.Shared.Types.Tier.CUtlSymbolLarge lv, Sharp.Shared.Types.Tier.CUtlSymbolLarge rv)` [L:50]
  - Modifiers: public, static


### struct CUtlVector<T> : System.ValueType, System.Collections.Generic.IEnumerable<T>, System.IDisposable

- FullName: `Sharp.Shared.Types.Tier.CUtlVector<T>`
- Kind: struct
- Modifiers: public
- Source: Sharp.Shared/Types/Tier/CUtlVector.cs:29
- Generated: false
- Attributes: `[StructLayout(0, Pack = 8, Size = 24)]`
- Constraint: `where T : struct, unmanaged`

Inheritance: object → System.ValueType → **CUtlVector**

#### Constructors
- `Sharp.Shared.Types.Tier.CUtlVector<T>.CUtlVector([int growSize = 0], [int initSize = 0])` [L:37]

#### Properties
- `int Sharp.Shared.Types.Tier.CUtlVector<T>.Count` [L:35]
  - Modifiers: public, readonly
- `int Sharp.Shared.Types.Tier.CUtlVector<T>.Size` [L:34]
  - Modifiers: public, readonly

#### Indexers
- `ref T Sharp.Shared.Types.Tier.CUtlVector<T>.this[long index]` [L:54]
  - Modifiers: public, readonly

#### Methods
- `Sharp.Shared.Types.Tier.CUtlVector<T>.Enumerator Sharp.Shared.Types.Tier.CUtlVector<T>.GetEnumerator()` [L:66]
- `System.ReadOnlySpan<T> Sharp.Shared.Types.Tier.CUtlVector<T>.AsReadOnlySpan()` [L:48]
- `System.Span<T> Sharp.Shared.Types.Tier.CUtlVector<T>.AsSpan()` [L:45]
- `T* Sharp.Shared.Types.Tier.CUtlVector<T>.AddToTailGetPtr()` [L:114]
- `T* Sharp.Shared.Types.Tier.CUtlVector<T>.Base()` [L:51]
- `ref T Sharp.Shared.Types.Tier.CUtlVector<T>.AddToTailGetRef()` [L:106]
- `ref T Sharp.Shared.Types.Tier.CUtlVector<T>.Element(long index)` [L:56]
- `void Sharp.Shared.Types.Tier.CUtlVector<T>.Add(T item)` [L:85]
- `void Sharp.Shared.Types.Tier.CUtlVector<T>.Add(ref readonly T item)` [L:88]
- `void Sharp.Shared.Types.Tier.CUtlVector<T>.Dispose()` [L:40]
- `void Sharp.Shared.Types.Tier.CUtlVector<T>.Purge()` [L:211]
- `void Sharp.Shared.Types.Tier.CUtlVector<T>.PurgeAndDeleteElements()` [L:191]
  - Summary: Frees the unmanaged memory pointed to by each element, then clears and deallocates the vector's own memory.
- `void Sharp.Shared.Types.Tier.CUtlVector<T>.Remove(int index)` [L:160]
- `void Sharp.Shared.Types.Tier.CUtlVector<T>.RemoveAll()` [L:217]


### struct Enumerator : System.ValueType, System.Collections.Generic.IEnumerator<T>, System.Collections.IEnumerator

- FullName: `Sharp.Shared.Types.Tier.CUtlVector<T>.Enumerator`
- Kind: struct
- Modifiers: public
- Source: Sharp.Shared/Types/Tier/CUtlVector.cs:227
- Generated: false

Inheritance: object → System.ValueType → **Enumerator**

#### Constructors
- `Sharp.Shared.Types.Tier.CUtlVector<T>.Enumerator.Enumerator(Sharp.Shared.Types.Tier.CUtlVector<T> vector)` [L:232]

#### Properties
- `T Sharp.Shared.Types.Tier.CUtlVector<T>.Enumerator.Current` [L:250]
  - Modifiers: public, readonly

#### Methods
- `bool Sharp.Shared.Types.Tier.CUtlVector<T>.Enumerator.MoveNext()` [L:238]
- `void Sharp.Shared.Types.Tier.CUtlVector<T>.Enumerator.Dispose()` [L:254]
- `void Sharp.Shared.Types.Tier.CUtlVector<T>.Enumerator.Reset()` [L:245]


