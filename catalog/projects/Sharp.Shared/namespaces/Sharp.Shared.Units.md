# Sharp.Shared.Units

Project: Sharp.Shared
Types: 6 (0 generated)

### struct EntityIndex : System.ValueType, System.IComparable<Sharp.Shared.Units.EntityIndex>, System.IEquatable<Sharp.Shared.Units.EntityIndex>, System.IFormattable, System.ISpanFormattable, System.IUtf8SpanFormattable, System.Numerics.IAdditionOperators<Sharp.Shared.Units.EntityIndex, Sharp.Shared.Units.EntityIndex, Sharp.Shared.Units.EntityIndex>, System.Numerics.IComparisonOperators<Sharp.Shared.Units.EntityIndex, Sharp.Shared.Units.EntityIndex, bool>, System.Numerics.IDecrementOperators<Sharp.Shared.Units.EntityIndex>, System.Numerics.IDivisionOperators<Sharp.Shared.Units.EntityIndex, Sharp.Shared.Units.EntityIndex, Sharp.Shared.Units.EntityIndex>, System.Numerics.IEqualityOperators<Sharp.Shared.Units.EntityIndex, Sharp.Shared.Units.EntityIndex, bool>, System.Numerics.IIncrementOperators<Sharp.Shared.Units.EntityIndex>, System.Numerics.IMultiplyOperators<Sharp.Shared.Units.EntityIndex, Sharp.Shared.Units.EntityIndex, Sharp.Shared.Units.EntityIndex>, System.Numerics.ISubtractionOperators<Sharp.Shared.Units.EntityIndex, Sharp.Shared.Units.EntityIndex, Sharp.Shared.Units.EntityIndex>, System.Numerics.IUnaryNegationOperators<Sharp.Shared.Units.EntityIndex, Sharp.Shared.Units.EntityIndex>, System.Numerics.IUnaryPlusOperators<Sharp.Shared.Units.EntityIndex, Sharp.Shared.Units.EntityIndex>

- FullName: `Sharp.Shared.Units.EntityIndex`
- Kind: struct
- Modifiers: public, readonly, partial
- Source: Sharp.Shared/Units/EntityIndex.cs:32
- Generated: false
- Attributes: `[JsonConverter(Sharp.Shared.Units.EntityIndex.EntityIndexJsonConverter)]` `[TypeConverter(Sharp.Shared.Units.EntityIndex.EntityIndexTypeConverter)]` `[TypeConverter(Sharp.Shared.Units.EntityIndex.EntityIndexTypeConverter)]` `[UnitOf]`

Inheritance: object → System.ValueType → **EntityIndex**

#### Constructors
- `Sharp.Shared.Units.EntityIndex.EntityIndex(Sharp.Shared.Objects.IGameClient client)` [L:44]
- `Sharp.Shared.Units.EntityIndex.EntityIndex(Sharp.Shared.Units.PlayerSlot slot)` [L:41]
- `Sharp.Shared.Units.EntityIndex.EntityIndex(int value)` [L:43]
- `Sharp.Shared.Units.EntityIndex.EntityIndex(int value)` [L:28]

#### Fields
- `static readonly Sharp.Shared.Units.EntityIndex Sharp.Shared.Units.EntityIndex.InvalidIndex` [L:39]
  - Modifiers: public, static, readonly
- `static readonly Sharp.Shared.Units.EntityIndex Sharp.Shared.Units.EntityIndex.WorldIndex` [L:38]
  - Modifiers: public, static, readonly

#### Methods
- `bool Sharp.Shared.Units.EntityIndex.Equals(Sharp.Shared.Units.EntityIndex other)` [L:43]
  - Modifiers: public, readonly
- `bool Sharp.Shared.Units.EntityIndex.Equals(Sharp.Shared.Units.EntityIndex other)` [L:58]
  - Modifiers: public, readonly
- `bool Sharp.Shared.Units.EntityIndex.IsNetworked()` [L:35]
  - Modifiers: public, readonly
  - Attributes: `[MethodImpl(256)]`
- `bool Sharp.Shared.Units.EntityIndex.TryFormat(System.Span<byte> utf8Destination, out int bytesWritten, System.ReadOnlySpan<char> format, System.IFormatProvider? provider)` [L:103]
  - Modifiers: public, readonly
- `bool Sharp.Shared.Units.EntityIndex.TryFormat(System.Span<byte> utf8Destination, out int bytesWritten, System.ReadOnlySpan<char> format, System.IFormatProvider? provider)` [L:88]
  - Modifiers: public, readonly
- `bool Sharp.Shared.Units.EntityIndex.TryFormat(System.Span<char> destination, out int charsWritten, System.ReadOnlySpan<char> format, System.IFormatProvider? provider)` [L:99]
  - Modifiers: public, readonly
- `bool Sharp.Shared.Units.EntityIndex.TryFormat(System.Span<char> destination, out int charsWritten, System.ReadOnlySpan<char> format, System.IFormatProvider? provider)` [L:84]
  - Modifiers: public, readonly
- `int Sharp.Shared.Units.EntityIndex.AsPrimitive()` [L:41]
  - Modifiers: public, readonly
- `int Sharp.Shared.Units.EntityIndex.AsPrimitive()` [L:26]
  - Modifiers: public, readonly
- `int Sharp.Shared.Units.EntityIndex.CompareTo(Sharp.Shared.Units.EntityIndex other)` [L:219]
  - Modifiers: public, readonly
- `override bool Sharp.Shared.Units.EntityIndex.Equals(object obj)` [L:48]
  - Modifiers: public, override, readonly
- `override bool Sharp.Shared.Units.EntityIndex.Equals(object obj)` [L:63]
  - Modifiers: public, override, readonly
- `override int Sharp.Shared.Units.EntityIndex.GetHashCode()` [L:74]
  - Modifiers: public, override, readonly
- `override int Sharp.Shared.Units.EntityIndex.GetHashCode()` [L:89]
  - Modifiers: public, override, readonly
- `override string Sharp.Shared.Units.EntityIndex.ToString()` [L:79]
  - Modifiers: public, override, readonly
- `override string Sharp.Shared.Units.EntityIndex.ToString()` [L:94]
  - Modifiers: public, override, readonly
- `static Sharp.Shared.Units.EntityIndex Sharp.Shared.Units.EntityIndex.Parse(string s)` [L:109]
  - Modifiers: public, static
- `static bool Sharp.Shared.Units.EntityIndex.TryParse(string s, out Sharp.Shared.Units.EntityIndex result)` [L:114]
  - Modifiers: public, static
- `string Sharp.Shared.Units.EntityIndex.ToString(string? format, System.IFormatProvider? formatProvider)` [L:96]
  - Modifiers: public, readonly
- `string Sharp.Shared.Units.EntityIndex.ToString(string? format, System.IFormatProvider? formatProvider)` [L:81]
  - Modifiers: public, readonly

#### Operators
- `static Sharp.Shared.Units.EntityIndex Sharp.Shared.Units.EntityIndex.operator *(Sharp.Shared.Units.EntityIndex x, Sharp.Shared.Units.EntityIndex y)` [L:149]
  - Modifiers: public, static
- `static Sharp.Shared.Units.EntityIndex Sharp.Shared.Units.EntityIndex.operator *(Sharp.Shared.Units.EntityIndex x, int y)` [L:200]
  - Modifiers: public, static
- `static Sharp.Shared.Units.EntityIndex Sharp.Shared.Units.EntityIndex.operator +(Sharp.Shared.Units.EntityIndex value)` [L:138]
  - Modifiers: public, static
- `static Sharp.Shared.Units.EntityIndex Sharp.Shared.Units.EntityIndex.operator +(Sharp.Shared.Units.EntityIndex x, Sharp.Shared.Units.EntityIndex y)` [L:130]
  - Modifiers: public, static
- `static Sharp.Shared.Units.EntityIndex Sharp.Shared.Units.EntityIndex.operator +(Sharp.Shared.Units.EntityIndex x, int y)` [L:184]
  - Modifiers: public, static
- `static Sharp.Shared.Units.EntityIndex Sharp.Shared.Units.EntityIndex.operator ++(Sharp.Shared.Units.EntityIndex x)` [L:166]
  - Modifiers: public, static
- `static Sharp.Shared.Units.EntityIndex Sharp.Shared.Units.EntityIndex.operator -(Sharp.Shared.Units.EntityIndex value)` [L:147]
  - Modifiers: public, static
- `static Sharp.Shared.Units.EntityIndex Sharp.Shared.Units.EntityIndex.operator -(Sharp.Shared.Units.EntityIndex x, Sharp.Shared.Units.EntityIndex y)` [L:139]
  - Modifiers: public, static
- `static Sharp.Shared.Units.EntityIndex Sharp.Shared.Units.EntityIndex.operator -(Sharp.Shared.Units.EntityIndex x, int y)` [L:192]
  - Modifiers: public, static
- `static Sharp.Shared.Units.EntityIndex Sharp.Shared.Units.EntityIndex.operator --(Sharp.Shared.Units.EntityIndex x)` [L:174]
  - Modifiers: public, static
- `static Sharp.Shared.Units.EntityIndex Sharp.Shared.Units.EntityIndex.operator /(Sharp.Shared.Units.EntityIndex x, Sharp.Shared.Units.EntityIndex y)` [L:158]
  - Modifiers: public, static
- `static Sharp.Shared.Units.EntityIndex Sharp.Shared.Units.EntityIndex.operator /(Sharp.Shared.Units.EntityIndex x, int y)` [L:209]
  - Modifiers: public, static
- `static Sharp.Shared.Units.EntityIndex.explicit operator Sharp.Shared.Units.EntityIndex(int value)` [L:38]
  - Modifiers: public, static
- `static Sharp.Shared.Units.EntityIndex.explicit operator int(Sharp.Shared.Units.EntityIndex value)` [L:33]
  - Modifiers: public, static
- `static Sharp.Shared.Units.EntityIndex.implicit operator Sharp.Shared.Units.EntityIndex(int value)` [L:53]
  - Modifiers: public, static
- `static Sharp.Shared.Units.EntityIndex.implicit operator int(Sharp.Shared.Units.EntityIndex value)` [L:48]
  - Modifiers: public, static
- `static bool Sharp.Shared.Units.EntityIndex.operator !=(Sharp.Shared.Units.EntityIndex x, Sharp.Shared.Units.EntityIndex y)` [L:69]
  - Modifiers: public, static
- `static bool Sharp.Shared.Units.EntityIndex.operator !=(Sharp.Shared.Units.EntityIndex x, Sharp.Shared.Units.EntityIndex y)` [L:84]
  - Modifiers: public, static
- `static bool Sharp.Shared.Units.EntityIndex.operator <(Sharp.Shared.Units.EntityIndex x, Sharp.Shared.Units.EntityIndex y)` [L:228]
  - Modifiers: public, static
- `static bool Sharp.Shared.Units.EntityIndex.operator <=(Sharp.Shared.Units.EntityIndex x, Sharp.Shared.Units.EntityIndex y)` [L:238]
  - Modifiers: public, static
- `static bool Sharp.Shared.Units.EntityIndex.operator ==(Sharp.Shared.Units.EntityIndex x, Sharp.Shared.Units.EntityIndex y)` [L:64]
  - Modifiers: public, static
- `static bool Sharp.Shared.Units.EntityIndex.operator ==(Sharp.Shared.Units.EntityIndex x, Sharp.Shared.Units.EntityIndex y)` [L:79]
  - Modifiers: public, static
- `static bool Sharp.Shared.Units.EntityIndex.operator >(Sharp.Shared.Units.EntityIndex x, Sharp.Shared.Units.EntityIndex y)` [L:223]
  - Modifiers: public, static
- `static bool Sharp.Shared.Units.EntityIndex.operator >=(Sharp.Shared.Units.EntityIndex x, Sharp.Shared.Units.EntityIndex y)` [L:233]
  - Modifiers: public, static


### struct NetworkReceiver : System.ValueType, System.Collections.Generic.IEnumerable<Sharp.Shared.Units.PlayerSlot>, System.IEquatable<Sharp.Shared.Units.NetworkReceiver>, System.IFormattable, System.ISpanFormattable, System.IUtf8SpanFormattable, System.Numerics.IEqualityOperators<Sharp.Shared.Units.NetworkReceiver, Sharp.Shared.Units.NetworkReceiver, bool>

- FullName: `Sharp.Shared.Units.NetworkReceiver`
- Kind: struct
- Modifiers: public, readonly, partial
- Source: Sharp.Shared/Units/NetworkReceiver.cs:29
- Generated: false
- Attributes: `[TypeConverter(Sharp.Shared.Units.NetworkReceiver.NetworkReceiverTypeConverter)]` `[TypeConverter(Sharp.Shared.Units.NetworkReceiver.NetworkReceiverTypeConverter)]` `[UnitOf]`

Inheritance: object → System.ValueType → **NetworkReceiver**

#### Constructors
- `Sharp.Shared.Units.NetworkReceiver.NetworkReceiver(System.Collections.Generic.IEnumerable<Sharp.Shared.Units.PlayerSlot> players)` [L:33]
- `Sharp.Shared.Units.NetworkReceiver.NetworkReceiver(System.Collections.Generic.IReadOnlyCollection<Sharp.Shared.Units.PlayerSlot> players)` [L:36]
- `Sharp.Shared.Units.NetworkReceiver.NetworkReceiver(ulong value)` [L:28]
- `Sharp.Shared.Units.NetworkReceiver.NetworkReceiver(ulong value)` [L:28]

#### Methods
- `Sharp.Shared.Units.NetworkReceiver Sharp.Shared.Units.NetworkReceiver.Append(Sharp.Shared.Units.PlayerSlot slot)` [L:51]
  - Modifiers: public, readonly
- `Sharp.Shared.Units.NetworkReceiver Sharp.Shared.Units.NetworkReceiver.Remove(Sharp.Shared.Units.PlayerSlot slot)` [L:54]
  - Modifiers: public, readonly
- `Sharp.Shared.Units.NetworkReceiver.Enumerator Sharp.Shared.Units.NetworkReceiver.GetEnumerator()` [L:77]
  - Modifiers: public, readonly
- `Sharp.Shared.Units.PlayerSlot[] Sharp.Shared.Units.NetworkReceiver.GetClientsArray()` [L:68]
  - Modifiers: public, readonly
- `System.Collections.Generic.IEnumerable<Sharp.Shared.Units.PlayerSlot> Sharp.Shared.Units.NetworkReceiver.GetClients()` [L:57]
  - Modifiers: public, readonly
- `bool Sharp.Shared.Units.NetworkReceiver.Equals(Sharp.Shared.Units.NetworkReceiver other)` [L:43]
  - Modifiers: public, readonly
- `bool Sharp.Shared.Units.NetworkReceiver.Equals(Sharp.Shared.Units.NetworkReceiver other)` [L:43]
  - Modifiers: public, readonly
- `bool Sharp.Shared.Units.NetworkReceiver.HasClient(Sharp.Shared.Units.PlayerSlot slot)` [L:48]
  - Modifiers: public, readonly
- `bool Sharp.Shared.Units.NetworkReceiver.IsEmpty()` [L:39]
  - Modifiers: public, readonly
- `bool Sharp.Shared.Units.NetworkReceiver.IsFull()` [L:42]
  - Modifiers: public, readonly
- `bool Sharp.Shared.Units.NetworkReceiver.TryFormat(System.Span<byte> utf8Destination, out int bytesWritten, System.ReadOnlySpan<char> format, System.IFormatProvider? provider)` [L:88]
  - Modifiers: public, readonly
- `bool Sharp.Shared.Units.NetworkReceiver.TryFormat(System.Span<byte> utf8Destination, out int bytesWritten, System.ReadOnlySpan<char> format, System.IFormatProvider? provider)` [L:88]
  - Modifiers: public, readonly
- `bool Sharp.Shared.Units.NetworkReceiver.TryFormat(System.Span<char> destination, out int charsWritten, System.ReadOnlySpan<char> format, System.IFormatProvider? provider)` [L:84]
  - Modifiers: public, readonly
- `bool Sharp.Shared.Units.NetworkReceiver.TryFormat(System.Span<char> destination, out int charsWritten, System.ReadOnlySpan<char> format, System.IFormatProvider? provider)` [L:84]
  - Modifiers: public, readonly
- `int Sharp.Shared.Units.NetworkReceiver.Count()` [L:45]
  - Modifiers: public, readonly
- `override bool Sharp.Shared.Units.NetworkReceiver.Equals(object obj)` [L:48]
  - Modifiers: public, override, readonly
- `override bool Sharp.Shared.Units.NetworkReceiver.Equals(object obj)` [L:48]
  - Modifiers: public, override, readonly
- `override int Sharp.Shared.Units.NetworkReceiver.GetHashCode()` [L:74]
  - Modifiers: public, override, readonly
- `override int Sharp.Shared.Units.NetworkReceiver.GetHashCode()` [L:74]
  - Modifiers: public, override, readonly
- `override string Sharp.Shared.Units.NetworkReceiver.ToString()` [L:79]
  - Modifiers: public, override, readonly
- `override string Sharp.Shared.Units.NetworkReceiver.ToString()` [L:79]
  - Modifiers: public, override, readonly
- `string Sharp.Shared.Units.NetworkReceiver.DestructureTransform()` [L:74]
  - Modifiers: public, readonly
- `string Sharp.Shared.Units.NetworkReceiver.ToString(string? format, System.IFormatProvider? formatProvider)` [L:81]
  - Modifiers: public, readonly
- `string Sharp.Shared.Units.NetworkReceiver.ToString(string? format, System.IFormatProvider? formatProvider)` [L:81]
  - Modifiers: public, readonly
- `ulong Sharp.Shared.Units.NetworkReceiver.AsPrimitive()` [L:26]
  - Modifiers: public, readonly
- `ulong Sharp.Shared.Units.NetworkReceiver.AsPrimitive()` [L:26]
  - Modifiers: public, readonly

#### Operators
- `static Sharp.Shared.Units.NetworkReceiver.explicit operator Sharp.Shared.Units.NetworkReceiver(ulong value)` [L:38]
  - Modifiers: public, static
- `static Sharp.Shared.Units.NetworkReceiver.explicit operator ulong(Sharp.Shared.Units.NetworkReceiver value)` [L:33]
  - Modifiers: public, static
- `static Sharp.Shared.Units.NetworkReceiver.implicit operator Sharp.Shared.Units.NetworkReceiver(ulong value)` [L:38]
  - Modifiers: public, static
- `static Sharp.Shared.Units.NetworkReceiver.implicit operator ulong(Sharp.Shared.Units.NetworkReceiver value)` [L:33]
  - Modifiers: public, static
- `static bool Sharp.Shared.Units.NetworkReceiver.operator !=(Sharp.Shared.Units.NetworkReceiver x, Sharp.Shared.Units.NetworkReceiver y)` [L:69]
  - Modifiers: public, static
- `static bool Sharp.Shared.Units.NetworkReceiver.operator !=(Sharp.Shared.Units.NetworkReceiver x, Sharp.Shared.Units.NetworkReceiver y)` [L:69]
  - Modifiers: public, static
- `static bool Sharp.Shared.Units.NetworkReceiver.operator ==(Sharp.Shared.Units.NetworkReceiver x, Sharp.Shared.Units.NetworkReceiver y)` [L:64]
  - Modifiers: public, static
- `static bool Sharp.Shared.Units.NetworkReceiver.operator ==(Sharp.Shared.Units.NetworkReceiver x, Sharp.Shared.Units.NetworkReceiver y)` [L:64]
  - Modifiers: public, static


### struct Enumerator : System.ValueType, System.Collections.Generic.IEnumerator<Sharp.Shared.Units.PlayerSlot>, System.Collections.IEnumerator

- FullName: `Sharp.Shared.Units.NetworkReceiver.Enumerator`
- Kind: struct
- Modifiers: public
- Source: Sharp.Shared/Units/NetworkReceiver.cs:86
- Generated: false

Inheritance: object → System.ValueType → **Enumerator**

#### Constructors
- `Sharp.Shared.Units.NetworkReceiver.Enumerator.Enumerator(ulong value)` [L:92]

#### Properties
- `Sharp.Shared.Units.PlayerSlot Sharp.Shared.Units.NetworkReceiver.Enumerator.Current` [L:99]
  - Modifiers: public, readonly

#### Methods
- `bool Sharp.Shared.Units.NetworkReceiver.Enumerator.MoveNext()` [L:102]
- `void Sharp.Shared.Units.NetworkReceiver.Enumerator.Dispose()` [L:127]
- `void Sharp.Shared.Units.NetworkReceiver.Enumerator.Reset()` [L:121]


### struct PlayerSlot : System.ValueType, System.IComparable<Sharp.Shared.Units.PlayerSlot>, System.IEquatable<Sharp.Shared.Units.PlayerSlot>, System.IFormattable, System.ISpanFormattable, System.IUtf8SpanFormattable, System.Numerics.IAdditionOperators<Sharp.Shared.Units.PlayerSlot, Sharp.Shared.Units.PlayerSlot, Sharp.Shared.Units.PlayerSlot>, System.Numerics.IComparisonOperators<Sharp.Shared.Units.PlayerSlot, Sharp.Shared.Units.PlayerSlot, bool>, System.Numerics.IDecrementOperators<Sharp.Shared.Units.PlayerSlot>, System.Numerics.IDivisionOperators<Sharp.Shared.Units.PlayerSlot, Sharp.Shared.Units.PlayerSlot, Sharp.Shared.Units.PlayerSlot>, System.Numerics.IEqualityOperators<Sharp.Shared.Units.PlayerSlot, Sharp.Shared.Units.PlayerSlot, bool>, System.Numerics.IIncrementOperators<Sharp.Shared.Units.PlayerSlot>, System.Numerics.IMultiplyOperators<Sharp.Shared.Units.PlayerSlot, Sharp.Shared.Units.PlayerSlot, Sharp.Shared.Units.PlayerSlot>, System.Numerics.ISubtractionOperators<Sharp.Shared.Units.PlayerSlot, Sharp.Shared.Units.PlayerSlot, Sharp.Shared.Units.PlayerSlot>, System.Numerics.IUnaryNegationOperators<Sharp.Shared.Units.PlayerSlot, Sharp.Shared.Units.PlayerSlot>, System.Numerics.IUnaryPlusOperators<Sharp.Shared.Units.PlayerSlot, Sharp.Shared.Units.PlayerSlot>

- FullName: `Sharp.Shared.Units.PlayerSlot`
- Kind: struct
- Modifiers: public, readonly, partial
- Source: Sharp.Shared/Units/PlayerSlot.cs:33
- Generated: false
- Attributes: `[JsonConverter(Sharp.Shared.Units.PlayerSlot.PlayerSlotJsonConverter)]` `[TypeConverter(Sharp.Shared.Units.PlayerSlot.PlayerSlotTypeConverter)]` `[TypeConverter(Sharp.Shared.Units.PlayerSlot.PlayerSlotTypeConverter)]` `[UnitOf]`

Inheritance: object → System.ValueType → **PlayerSlot**

#### Constructors
- `Sharp.Shared.Units.PlayerSlot.PlayerSlot(Sharp.Shared.GameEntities.IPlayerController controller)` [L:49]
- `Sharp.Shared.Units.PlayerSlot.PlayerSlot(Sharp.Shared.Units.EntityIndex index)` [L:39]
- `Sharp.Shared.Units.PlayerSlot.PlayerSlot(byte value)` [L:43]
- `Sharp.Shared.Units.PlayerSlot.PlayerSlot(byte value)` [L:28]

#### Fields
- `static readonly Sharp.Shared.Units.PlayerSlot Sharp.Shared.Units.PlayerSlot.MaxPlayerCount` [L:37]
  - Modifiers: public, static, readonly
- `static readonly Sharp.Shared.Units.PlayerSlot Sharp.Shared.Units.PlayerSlot.MaxPlayerSlot` [L:35]
  - Modifiers: public, static, readonly

#### Methods
- `bool Sharp.Shared.Units.PlayerSlot.Equals(Sharp.Shared.Units.PlayerSlot other)` [L:43]
  - Modifiers: public, readonly
- `bool Sharp.Shared.Units.PlayerSlot.Equals(Sharp.Shared.Units.PlayerSlot other)` [L:58]
  - Modifiers: public, readonly
- `bool Sharp.Shared.Units.PlayerSlot.IsValid()` [L:52]
  - Modifiers: public, readonly
- `bool Sharp.Shared.Units.PlayerSlot.TryFormat(System.Span<byte> utf8Destination, out int bytesWritten, System.ReadOnlySpan<char> format, System.IFormatProvider? provider)` [L:103]
  - Modifiers: public, readonly
- `bool Sharp.Shared.Units.PlayerSlot.TryFormat(System.Span<byte> utf8Destination, out int bytesWritten, System.ReadOnlySpan<char> format, System.IFormatProvider? provider)` [L:88]
  - Modifiers: public, readonly
- `bool Sharp.Shared.Units.PlayerSlot.TryFormat(System.Span<char> destination, out int charsWritten, System.ReadOnlySpan<char> format, System.IFormatProvider? provider)` [L:99]
  - Modifiers: public, readonly
- `bool Sharp.Shared.Units.PlayerSlot.TryFormat(System.Span<char> destination, out int charsWritten, System.ReadOnlySpan<char> format, System.IFormatProvider? provider)` [L:84]
  - Modifiers: public, readonly
- `byte Sharp.Shared.Units.PlayerSlot.AsPrimitive()` [L:41]
  - Modifiers: public, readonly
- `byte Sharp.Shared.Units.PlayerSlot.AsPrimitive()` [L:26]
  - Modifiers: public, readonly
- `int Sharp.Shared.Units.PlayerSlot.CompareTo(Sharp.Shared.Units.PlayerSlot other)` [L:219]
  - Modifiers: public, readonly
- `override bool Sharp.Shared.Units.PlayerSlot.Equals(object obj)` [L:48]
  - Modifiers: public, override, readonly
- `override bool Sharp.Shared.Units.PlayerSlot.Equals(object obj)` [L:63]
  - Modifiers: public, override, readonly
- `override int Sharp.Shared.Units.PlayerSlot.GetHashCode()` [L:74]
  - Modifiers: public, override, readonly
- `override int Sharp.Shared.Units.PlayerSlot.GetHashCode()` [L:89]
  - Modifiers: public, override, readonly
- `override string Sharp.Shared.Units.PlayerSlot.ToString()` [L:79]
  - Modifiers: public, override, readonly
- `override string Sharp.Shared.Units.PlayerSlot.ToString()` [L:94]
  - Modifiers: public, override, readonly
- `static Sharp.Shared.Units.PlayerSlot Sharp.Shared.Units.PlayerSlot.Parse(string s)` [L:109]
  - Modifiers: public, static
- `static bool Sharp.Shared.Units.PlayerSlot.TryParse(string s, out Sharp.Shared.Units.PlayerSlot result)` [L:114]
  - Modifiers: public, static
- `string Sharp.Shared.Units.PlayerSlot.ToString(string? format, System.IFormatProvider? formatProvider)` [L:96]
  - Modifiers: public, readonly
- `string Sharp.Shared.Units.PlayerSlot.ToString(string? format, System.IFormatProvider? formatProvider)` [L:81]
  - Modifiers: public, readonly

#### Operators
- `static Sharp.Shared.Units.PlayerSlot Sharp.Shared.Units.PlayerSlot.operator *(Sharp.Shared.Units.PlayerSlot x, Sharp.Shared.Units.PlayerSlot y)` [L:149]
  - Modifiers: public, static
- `static Sharp.Shared.Units.PlayerSlot Sharp.Shared.Units.PlayerSlot.operator *(Sharp.Shared.Units.PlayerSlot x, byte y)` [L:200]
  - Modifiers: public, static
- `static Sharp.Shared.Units.PlayerSlot Sharp.Shared.Units.PlayerSlot.operator +(Sharp.Shared.Units.PlayerSlot value)` [L:138]
  - Modifiers: public, static
- `static Sharp.Shared.Units.PlayerSlot Sharp.Shared.Units.PlayerSlot.operator +(Sharp.Shared.Units.PlayerSlot x, Sharp.Shared.Units.PlayerSlot y)` [L:130]
  - Modifiers: public, static
- `static Sharp.Shared.Units.PlayerSlot Sharp.Shared.Units.PlayerSlot.operator +(Sharp.Shared.Units.PlayerSlot x, byte y)` [L:184]
  - Modifiers: public, static
- `static Sharp.Shared.Units.PlayerSlot Sharp.Shared.Units.PlayerSlot.operator ++(Sharp.Shared.Units.PlayerSlot x)` [L:166]
  - Modifiers: public, static
- `static Sharp.Shared.Units.PlayerSlot Sharp.Shared.Units.PlayerSlot.operator -(Sharp.Shared.Units.PlayerSlot value)` [L:147]
  - Modifiers: public, static
- `static Sharp.Shared.Units.PlayerSlot Sharp.Shared.Units.PlayerSlot.operator -(Sharp.Shared.Units.PlayerSlot x, Sharp.Shared.Units.PlayerSlot y)` [L:139]
  - Modifiers: public, static
- `static Sharp.Shared.Units.PlayerSlot Sharp.Shared.Units.PlayerSlot.operator -(Sharp.Shared.Units.PlayerSlot x, byte y)` [L:192]
  - Modifiers: public, static
- `static Sharp.Shared.Units.PlayerSlot Sharp.Shared.Units.PlayerSlot.operator --(Sharp.Shared.Units.PlayerSlot x)` [L:174]
  - Modifiers: public, static
- `static Sharp.Shared.Units.PlayerSlot Sharp.Shared.Units.PlayerSlot.operator /(Sharp.Shared.Units.PlayerSlot x, Sharp.Shared.Units.PlayerSlot y)` [L:158]
  - Modifiers: public, static
- `static Sharp.Shared.Units.PlayerSlot Sharp.Shared.Units.PlayerSlot.operator /(Sharp.Shared.Units.PlayerSlot x, byte y)` [L:209]
  - Modifiers: public, static
- `static Sharp.Shared.Units.PlayerSlot.explicit operator Sharp.Shared.Units.PlayerSlot(byte value)` [L:38]
  - Modifiers: public, static
- `static Sharp.Shared.Units.PlayerSlot.explicit operator byte(Sharp.Shared.Units.PlayerSlot value)` [L:33]
  - Modifiers: public, static
- `static Sharp.Shared.Units.PlayerSlot.implicit operator Sharp.Shared.Units.PlayerSlot(byte value)` [L:53]
  - Modifiers: public, static
- `static Sharp.Shared.Units.PlayerSlot.implicit operator byte(Sharp.Shared.Units.PlayerSlot value)` [L:48]
  - Modifiers: public, static
- `static bool Sharp.Shared.Units.PlayerSlot.operator !=(Sharp.Shared.Units.PlayerSlot x, Sharp.Shared.Units.PlayerSlot y)` [L:69]
  - Modifiers: public, static
- `static bool Sharp.Shared.Units.PlayerSlot.operator !=(Sharp.Shared.Units.PlayerSlot x, Sharp.Shared.Units.PlayerSlot y)` [L:84]
  - Modifiers: public, static
- `static bool Sharp.Shared.Units.PlayerSlot.operator <(Sharp.Shared.Units.PlayerSlot x, Sharp.Shared.Units.PlayerSlot y)` [L:228]
  - Modifiers: public, static
- `static bool Sharp.Shared.Units.PlayerSlot.operator <=(Sharp.Shared.Units.PlayerSlot x, Sharp.Shared.Units.PlayerSlot y)` [L:238]
  - Modifiers: public, static
- `static bool Sharp.Shared.Units.PlayerSlot.operator ==(Sharp.Shared.Units.PlayerSlot x, Sharp.Shared.Units.PlayerSlot y)` [L:64]
  - Modifiers: public, static
- `static bool Sharp.Shared.Units.PlayerSlot.operator ==(Sharp.Shared.Units.PlayerSlot x, Sharp.Shared.Units.PlayerSlot y)` [L:79]
  - Modifiers: public, static
- `static bool Sharp.Shared.Units.PlayerSlot.operator >(Sharp.Shared.Units.PlayerSlot x, Sharp.Shared.Units.PlayerSlot y)` [L:223]
  - Modifiers: public, static
- `static bool Sharp.Shared.Units.PlayerSlot.operator >=(Sharp.Shared.Units.PlayerSlot x, Sharp.Shared.Units.PlayerSlot y)` [L:233]
  - Modifiers: public, static


### struct SteamID : System.ValueType, System.IComparable<Sharp.Shared.Units.SteamID>, System.IEquatable<Sharp.Shared.Units.SteamID>, System.IFormattable, System.ISpanFormattable, System.IUtf8SpanFormattable, System.Numerics.IComparisonOperators<Sharp.Shared.Units.SteamID, Sharp.Shared.Units.SteamID, bool>, System.Numerics.IEqualityOperators<Sharp.Shared.Units.SteamID, Sharp.Shared.Units.SteamID, bool>

- FullName: `Sharp.Shared.Units.SteamID`
- Kind: struct
- Modifiers: public, readonly, partial
- Source: Sharp.Shared/Units/SteamId.cs:32
- Generated: false
- Attributes: `[JsonConverter(Sharp.Shared.Units.SteamID.SteamIDJsonConverter)]` `[TypeConverter(Sharp.Shared.Units.SteamID.SteamIDTypeConverter)]` `[TypeConverter(Sharp.Shared.Units.SteamID.SteamIDTypeConverter)]` `[UnitOf]`

Inheritance: object → System.ValueType → **SteamID**

#### Constructors
- `Sharp.Shared.Units.SteamID.SteamID(ulong value)` [L:35]
- `Sharp.Shared.Units.SteamID.SteamID(ulong value)` [L:28]

#### Properties
- `Sharp.Shared.Enums.SteamAccountType Sharp.Shared.Units.SteamID.AccountType` [L:42]
  - Modifiers: public, readonly
- `Sharp.Shared.Enums.SteamUniverse Sharp.Shared.Units.SteamID.Universe` [L:44]
  - Modifiers: public, readonly
- `uint Sharp.Shared.Units.SteamID.AccountId` [L:38]
  - Modifiers: public, readonly
- `uint Sharp.Shared.Units.SteamID.AccountInstance` [L:40]
  - Modifiers: public, readonly

#### Methods
- `bool Sharp.Shared.Units.SteamID.Equals(Sharp.Shared.Units.SteamID other)` [L:43]
  - Modifiers: public, readonly
- `bool Sharp.Shared.Units.SteamID.Equals(Sharp.Shared.Units.SteamID other)` [L:50]
  - Modifiers: public, readonly
- `bool Sharp.Shared.Units.SteamID.IsValidUserId()` [L:35]
  - Modifiers: public, readonly
  - Attributes: `[MethodImpl(256)]`
- `bool Sharp.Shared.Units.SteamID.TryFormat(System.Span<byte> utf8Destination, out int bytesWritten, System.ReadOnlySpan<char> format, System.IFormatProvider? provider)` [L:95]
  - Modifiers: public, readonly
- `bool Sharp.Shared.Units.SteamID.TryFormat(System.Span<byte> utf8Destination, out int bytesWritten, System.ReadOnlySpan<char> format, System.IFormatProvider? provider)` [L:88]
  - Modifiers: public, readonly
- `bool Sharp.Shared.Units.SteamID.TryFormat(System.Span<char> destination, out int charsWritten, System.ReadOnlySpan<char> format, System.IFormatProvider? provider)` [L:91]
  - Modifiers: public, readonly
- `bool Sharp.Shared.Units.SteamID.TryFormat(System.Span<char> destination, out int charsWritten, System.ReadOnlySpan<char> format, System.IFormatProvider? provider)` [L:84]
  - Modifiers: public, readonly
- `int Sharp.Shared.Units.SteamID.CompareTo(Sharp.Shared.Units.SteamID other)` [L:122]
  - Modifiers: public, readonly
- `override bool Sharp.Shared.Units.SteamID.Equals(object obj)` [L:55]
  - Modifiers: public, override, readonly
- `override bool Sharp.Shared.Units.SteamID.Equals(object obj)` [L:48]
  - Modifiers: public, override, readonly
- `override int Sharp.Shared.Units.SteamID.GetHashCode()` [L:81]
  - Modifiers: public, override, readonly
- `override int Sharp.Shared.Units.SteamID.GetHashCode()` [L:74]
  - Modifiers: public, override, readonly
- `override string Sharp.Shared.Units.SteamID.ToString()` [L:79]
  - Modifiers: public, override, readonly
- `override string Sharp.Shared.Units.SteamID.ToString()` [L:86]
  - Modifiers: public, override, readonly
- `static Sharp.Shared.Units.SteamID Sharp.Shared.Units.SteamID.Parse(string s)` [L:101]
  - Modifiers: public, static
- `static bool Sharp.Shared.Units.SteamID.TryParse(string s, out Sharp.Shared.Units.SteamID result)` [L:106]
  - Modifiers: public, static
- `string Sharp.Shared.Units.SteamID.DestructureTransform()` [L:46]
  - Modifiers: public, readonly
- `string Sharp.Shared.Units.SteamID.ToString(string? format, System.IFormatProvider? formatProvider)` [L:81]
  - Modifiers: public, readonly
- `string Sharp.Shared.Units.SteamID.ToString(string? format, System.IFormatProvider? formatProvider)` [L:88]
  - Modifiers: public, readonly
- `ulong Sharp.Shared.Units.SteamID.AsPrimitive()` [L:26]
  - Modifiers: public, readonly
- `ulong Sharp.Shared.Units.SteamID.AsPrimitive()` [L:33]
  - Modifiers: public, readonly

#### Operators
- `static Sharp.Shared.Units.SteamID.explicit operator Sharp.Shared.Units.SteamID(ulong value)` [L:38]
  - Modifiers: public, static
- `static Sharp.Shared.Units.SteamID.explicit operator ulong(Sharp.Shared.Units.SteamID value)` [L:33]
  - Modifiers: public, static
- `static Sharp.Shared.Units.SteamID.implicit operator Sharp.Shared.Units.SteamID(ulong value)` [L:45]
  - Modifiers: public, static
- `static Sharp.Shared.Units.SteamID.implicit operator ulong(Sharp.Shared.Units.SteamID value)` [L:40]
  - Modifiers: public, static
- `static bool Sharp.Shared.Units.SteamID.operator !=(Sharp.Shared.Units.SteamID x, Sharp.Shared.Units.SteamID y)` [L:69]
  - Modifiers: public, static
- `static bool Sharp.Shared.Units.SteamID.operator !=(Sharp.Shared.Units.SteamID x, Sharp.Shared.Units.SteamID y)` [L:76]
  - Modifiers: public, static
- `static bool Sharp.Shared.Units.SteamID.operator <(Sharp.Shared.Units.SteamID x, Sharp.Shared.Units.SteamID y)` [L:131]
  - Modifiers: public, static
- `static bool Sharp.Shared.Units.SteamID.operator <=(Sharp.Shared.Units.SteamID x, Sharp.Shared.Units.SteamID y)` [L:141]
  - Modifiers: public, static
- `static bool Sharp.Shared.Units.SteamID.operator ==(Sharp.Shared.Units.SteamID x, Sharp.Shared.Units.SteamID y)` [L:64]
  - Modifiers: public, static
- `static bool Sharp.Shared.Units.SteamID.operator ==(Sharp.Shared.Units.SteamID x, Sharp.Shared.Units.SteamID y)` [L:71]
  - Modifiers: public, static
- `static bool Sharp.Shared.Units.SteamID.operator >(Sharp.Shared.Units.SteamID x, Sharp.Shared.Units.SteamID y)` [L:126]
  - Modifiers: public, static
- `static bool Sharp.Shared.Units.SteamID.operator >=(Sharp.Shared.Units.SteamID x, Sharp.Shared.Units.SteamID y)` [L:136]
  - Modifiers: public, static


### struct UserID : System.ValueType, System.IComparable<Sharp.Shared.Units.UserID>, System.IEquatable<Sharp.Shared.Units.UserID>, System.IFormattable, System.ISpanFormattable, System.IUtf8SpanFormattable, System.Numerics.IComparisonOperators<Sharp.Shared.Units.UserID, Sharp.Shared.Units.UserID, bool>, System.Numerics.IEqualityOperators<Sharp.Shared.Units.UserID, Sharp.Shared.Units.UserID, bool>

- FullName: `Sharp.Shared.Units.UserID`
- Kind: struct
- Modifiers: public, readonly, partial
- Source: Sharp.Shared/Units/UserID.cs:30
- Generated: false
- Attributes: `[JsonConverter(Sharp.Shared.Units.UserID.UserIDJsonConverter)]` `[TypeConverter(Sharp.Shared.Units.UserID.UserIDTypeConverter)]` `[TypeConverter(Sharp.Shared.Units.UserID.UserIDTypeConverter)]` `[UnitOf]`

Inheritance: object → System.ValueType → **UserID**

#### Constructors
- `Sharp.Shared.Units.UserID.UserID(ushort value)` [L:28]
- `Sharp.Shared.Units.UserID.UserID(ushort value)` [L:35]

#### Methods
- `bool Sharp.Shared.Units.UserID.Equals(Sharp.Shared.Units.UserID other)` [L:50]
  - Modifiers: public, readonly
- `bool Sharp.Shared.Units.UserID.Equals(Sharp.Shared.Units.UserID other)` [L:43]
  - Modifiers: public, readonly
- `bool Sharp.Shared.Units.UserID.TryFormat(System.Span<byte> utf8Destination, out int bytesWritten, System.ReadOnlySpan<char> format, System.IFormatProvider? provider)` [L:88]
  - Modifiers: public, readonly
- `bool Sharp.Shared.Units.UserID.TryFormat(System.Span<byte> utf8Destination, out int bytesWritten, System.ReadOnlySpan<char> format, System.IFormatProvider? provider)` [L:95]
  - Modifiers: public, readonly
- `bool Sharp.Shared.Units.UserID.TryFormat(System.Span<char> destination, out int charsWritten, System.ReadOnlySpan<char> format, System.IFormatProvider? provider)` [L:91]
  - Modifiers: public, readonly
- `bool Sharp.Shared.Units.UserID.TryFormat(System.Span<char> destination, out int charsWritten, System.ReadOnlySpan<char> format, System.IFormatProvider? provider)` [L:84]
  - Modifiers: public, readonly
- `int Sharp.Shared.Units.UserID.CompareTo(Sharp.Shared.Units.UserID other)` [L:122]
  - Modifiers: public, readonly
- `override bool Sharp.Shared.Units.UserID.Equals(object obj)` [L:55]
  - Modifiers: public, override, readonly
- `override bool Sharp.Shared.Units.UserID.Equals(object obj)` [L:48]
  - Modifiers: public, override, readonly
- `override int Sharp.Shared.Units.UserID.GetHashCode()` [L:81]
  - Modifiers: public, override, readonly
- `override int Sharp.Shared.Units.UserID.GetHashCode()` [L:74]
  - Modifiers: public, override, readonly
- `override string Sharp.Shared.Units.UserID.ToString()` [L:79]
  - Modifiers: public, override, readonly
- `override string Sharp.Shared.Units.UserID.ToString()` [L:86]
  - Modifiers: public, override, readonly
- `static Sharp.Shared.Units.UserID Sharp.Shared.Units.UserID.Parse(string s)` [L:101]
  - Modifiers: public, static
- `static bool Sharp.Shared.Units.UserID.TryParse(string s, out Sharp.Shared.Units.UserID result)` [L:106]
  - Modifiers: public, static
- `string Sharp.Shared.Units.UserID.ToString(string? format, System.IFormatProvider? formatProvider)` [L:88]
  - Modifiers: public, readonly
- `string Sharp.Shared.Units.UserID.ToString(string? format, System.IFormatProvider? formatProvider)` [L:81]
  - Modifiers: public, readonly
- `ushort Sharp.Shared.Units.UserID.AsPrimitive()` [L:26]
  - Modifiers: public, readonly
- `ushort Sharp.Shared.Units.UserID.AsPrimitive()` [L:33]
  - Modifiers: public, readonly

#### Operators
- `static Sharp.Shared.Units.UserID.explicit operator Sharp.Shared.Units.UserID(ushort value)` [L:38]
  - Modifiers: public, static
- `static Sharp.Shared.Units.UserID.explicit operator ushort(Sharp.Shared.Units.UserID value)` [L:33]
  - Modifiers: public, static
- `static Sharp.Shared.Units.UserID.implicit operator Sharp.Shared.Units.UserID(ushort value)` [L:45]
  - Modifiers: public, static
- `static Sharp.Shared.Units.UserID.implicit operator ushort(Sharp.Shared.Units.UserID value)` [L:40]
  - Modifiers: public, static
- `static bool Sharp.Shared.Units.UserID.operator !=(Sharp.Shared.Units.UserID x, Sharp.Shared.Units.UserID y)` [L:76]
  - Modifiers: public, static
- `static bool Sharp.Shared.Units.UserID.operator !=(Sharp.Shared.Units.UserID x, Sharp.Shared.Units.UserID y)` [L:69]
  - Modifiers: public, static
- `static bool Sharp.Shared.Units.UserID.operator <(Sharp.Shared.Units.UserID x, Sharp.Shared.Units.UserID y)` [L:131]
  - Modifiers: public, static
- `static bool Sharp.Shared.Units.UserID.operator <=(Sharp.Shared.Units.UserID x, Sharp.Shared.Units.UserID y)` [L:141]
  - Modifiers: public, static
- `static bool Sharp.Shared.Units.UserID.operator ==(Sharp.Shared.Units.UserID x, Sharp.Shared.Units.UserID y)` [L:71]
  - Modifiers: public, static
- `static bool Sharp.Shared.Units.UserID.operator ==(Sharp.Shared.Units.UserID x, Sharp.Shared.Units.UserID y)` [L:64]
  - Modifiers: public, static
- `static bool Sharp.Shared.Units.UserID.operator >(Sharp.Shared.Units.UserID x, Sharp.Shared.Units.UserID y)` [L:126]
  - Modifiers: public, static
- `static bool Sharp.Shared.Units.UserID.operator >=(Sharp.Shared.Units.UserID x, Sharp.Shared.Units.UserID y)` [L:136]
  - Modifiers: public, static


