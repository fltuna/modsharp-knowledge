# Sharp.Shared.Utilities

Project: Sharp.Shared
Types: 6 (0 generated)

### class EnumConverter<T>

- FullName: `Sharp.Shared.Utilities.EnumConverter<T>`
- Kind: class
- Modifiers: public, static
- Source: Sharp.Shared/Utilities/EnumConverter.cs:25
- Generated: false

Inheritance: object → **EnumConverter**

#### Methods
- `static T Sharp.Shared.Utilities.EnumConverter<T>.Convert(int value)` [L:42]
  - Modifiers: public, static
- `static T Sharp.Shared.Utilities.EnumConverter<T>.Convert(long value)` [L:45]
  - Modifiers: public, static


### class IntPtrExtensions

- FullName: `Sharp.Shared.Utilities.IntPtrExtensions`
- Kind: class
- Modifiers: public, static
- Source: Sharp.Shared/Utilities/IntPtrExtensions.cs:22
- Generated: false

Inheritance: object → **IntPtrExtensions**

#### Methods
- `static bool Sharp.Shared.Utilities.IntPtrExtensions.IsValid(nint ptr)` [L:42]
  - Modifiers: public, static, this
- `static nint Sharp.Shared.Utilities.IntPtrExtensions.Add(nint ptr, int offset)` [L:39]
  - Modifiers: public, static, this
- `static nint Sharp.Shared.Utilities.IntPtrExtensions.Dereference(nint ptr)` [L:24]
  - Modifiers: public, static, this
- `static nint Sharp.Shared.Utilities.IntPtrExtensions.Dereference(nint ptr, int dereferences)` [L:27]
  - Modifiers: public, static, this


### class NativeString

- FullName: `Sharp.Shared.Utilities.NativeString`
- Kind: class
- Modifiers: public, static
- Source: Sharp.Shared/Utilities/NativeString.cs:27
- Generated: false

Inheritance: object → **NativeString**

#### Methods
- `static int Sharp.Shared.Utilities.NativeString.CStringCmp(byte* s1, byte* s2)` [L:47]
  - Modifiers: public, static
- `static int Sharp.Shared.Utilities.NativeString.GetByteCount(string value)` [L:41]
  - Modifiers: public, static
- `static int Sharp.Shared.Utilities.NativeString.GetMaxByteCount(string value)` [L:44]
  - Modifiers: public, static
- `static string Sharp.Shared.Utilities.NativeString.ReadString(byte* ptr)` [L:29]
  - Modifiers: public, static
- `static string Sharp.Shared.Utilities.NativeString.ReadString(nint ptr)` [L:32]
  - Modifiers: public, static
- `static void Sharp.Shared.Utilities.NativeString.WriteString(byte* ptr, int size, string value)` [L:35]
  - Modifiers: public, static


### class SpanExtensions

- FullName: `Sharp.Shared.Utilities.SpanExtensions`
- Kind: class
- Modifiers: public, static
- Source: Sharp.Shared/Utilities/SpanExtensions.cs:26
- Generated: false

Inheritance: object → **SpanExtensions**

#### Methods
- `static int Sharp.Shared.Utilities.SpanExtensions.WriteStringUtf8(System.Span<byte> span, string value)` [L:50]
  - Modifiers: public, static, this
- `static int Sharp.Shared.Utilities.SpanExtensions.WriteStringUtf8(System.Span<byte> span, string value, out bool truncated)` [L:28]
  - Modifiers: public, static, this


### class StringExtensions

- FullName: `Sharp.Shared.Utilities.StringExtensions`
- Kind: class
- Modifiers: public, static
- Source: Sharp.Shared/Utilities/StringExtensions.cs:22
- Generated: false

Inheritance: object → **StringExtensions**

#### Methods
- `static string Sharp.Shared.Utilities.StringExtensions.StripBracket(string str)` [L:34]
  - Modifiers: public, static, this
- `static string Sharp.Shared.Utilities.StringExtensions.StripQuote(string str)` [L:24]
  - Modifiers: public, static, this


### class Utils

- FullName: `Sharp.Shared.Utilities.Utils`
- Kind: class
- Modifiers: public, static
- Source: Sharp.Shared/Utilities/Utils.cs:27
- Generated: false

Inheritance: object → **Utils**

#### Methods
- `static Sharp.Shared.Types.Color Sharp.Shared.Utilities.Utils.GetColor(nint ptr, int offset)` [L:316]
  - Modifiers: public, static, this
- `static Sharp.Shared.Types.Vector Sharp.Shared.Utilities.Utils.GetVector(nint ptr, int offset)` [L:310]
  - Modifiers: public, static, this
- `static bool Sharp.Shared.Utilities.Utils.GetBool(nint ptr, int offset)` [L:188]
  - Modifiers: public, static, this
- `static bool Sharp.Shared.Utilities.Utils.GetObjectVarBool(nint @this, int objectOffset, int varOffset)` [L:225]
  - Modifiers: public, static, this
- `static byte Sharp.Shared.Utilities.Utils.GetByte(nint ptr, int offset)` [L:194]
  - Modifiers: public, static, this
- `static double Sharp.Shared.Utilities.Utils.GetDouble(nint ptr, int offset)` [L:97]
  - Modifiers: public, static, this
- `static double Sharp.Shared.Utilities.Utils.GetObjectVarDouble(nint @this, int objectOffset, int varOffset)` [L:239]
  - Modifiers: public, static, this
- `static float Sharp.Shared.Utilities.Utils.GetFloat(nint ptr, int offset)` [L:84]
  - Modifiers: public, static, this
- `static float Sharp.Shared.Utilities.Utils.GetObjectVarFloat(nint @this, int objectOffset, int varOffset)` [L:232]
  - Modifiers: public, static, this
- `static int Sharp.Shared.Utilities.Utils.GetInt32(nint ptr, int offset)` [L:136]
  - Modifiers: public, static, this
- `static int Sharp.Shared.Utilities.Utils.GetObjectVarInt32(nint @this, int objectOffset, int varOffset)` [L:260]
  - Modifiers: public, static, this
- `static long Sharp.Shared.Utilities.Utils.GetInt64(nint ptr, int offset)` [L:110]
  - Modifiers: public, static, this
- `static long Sharp.Shared.Utilities.Utils.GetObjectVarInt64(nint @this, int objectOffset, int varOffset)` [L:274]
  - Modifiers: public, static, this
- `static nint Sharp.Shared.Utilities.Utils.GetObjectPtr(nint @this, int objectOffset)` [L:288]
  - Modifiers: public, static, this
- `static nint Sharp.Shared.Utilities.Utils.GetVirtualMethod(nint @this, int offset)` [L:295]
  - Modifiers: public, static, this
- `static short Sharp.Shared.Utilities.Utils.GetInt16(nint ptr, int offset)` [L:162]
  - Modifiers: public, static, this
- `static short Sharp.Shared.Utilities.Utils.GetObjectVarInt16(nint @this, int objectOffset, int varOffset)` [L:246]
  - Modifiers: public, static, this
- `static string Sharp.Shared.Utilities.Utils.GetObjectVarString(nint @this, int objectOffset, int varOffset)` [L:217]
  - Modifiers: public, static, this
- `static string Sharp.Shared.Utilities.Utils.GetPtrString(nint ptr, int offset)` [L:210]
  - Modifiers: public, static, this
- `static string Sharp.Shared.Utilities.Utils.GetString(nint ptr, int offset)` [L:207]
  - Modifiers: public, static, this
- `static string Sharp.Shared.Utilities.Utils.ReadString(byte* ptr)` [L:32]
  - Modifiers: public, static
- `static string Sharp.Shared.Utilities.Utils.ReadString(sbyte* ptr)` [L:29]
  - Modifiers: public, static
- `static string Sharp.Shared.Utilities.Utils.ReadStringUtf8(nint ptr, int offset)` [L:46]
  - Modifiers: public, static, this
- `static uint Sharp.Shared.Utilities.Utils.GetObjectVarUInt32(nint @this, int objectOffset, int varOffset)` [L:267]
  - Modifiers: public, static, this
- `static uint Sharp.Shared.Utilities.Utils.GetUInt32(nint ptr, int offset)` [L:149]
  - Modifiers: public, static, this
- `static ulong Sharp.Shared.Utilities.Utils.GetObjectVarUInt64(nint @this, int objectOffset, int varOffset)` [L:281]
  - Modifiers: public, static, this
- `static ulong Sharp.Shared.Utilities.Utils.GetUInt64(nint ptr, int offset)` [L:123]
  - Modifiers: public, static, this
- `static ushort Sharp.Shared.Utilities.Utils.GetObjectVarUInt16(nint @this, int objectOffset, int varOffset)` [L:253]
  - Modifiers: public, static, this
- `static ushort Sharp.Shared.Utilities.Utils.GetUInt16(nint ptr, int offset)` [L:175]
  - Modifiers: public, static, this
- `static void Sharp.Shared.Utilities.Utils.SetColor(nint ptr, int offset, Sharp.Shared.Types.Color value)` [L:319]
  - Modifiers: public, static, this
- `static void Sharp.Shared.Utilities.Utils.WriteBool(nint ptr, int offset, bool value)` [L:191]
  - Modifiers: public, static, this
- `static void Sharp.Shared.Utilities.Utils.WriteByte(nint ptr, int offset, byte value)` [L:201]
  - Modifiers: public, static, this
- `static void Sharp.Shared.Utilities.Utils.WriteDouble(nint ptr, int offset, double value)` [L:104]
  - Modifiers: public, static, this
- `static void Sharp.Shared.Utilities.Utils.WriteFloat(nint ptr, int offset, float value)` [L:91]
  - Modifiers: public, static, this
- `static void Sharp.Shared.Utilities.Utils.WriteInt16(nint ptr, int offset, short value)` [L:169]
  - Modifiers: public, static, this
- `static void Sharp.Shared.Utilities.Utils.WriteInt32(nint ptr, int offset, int value)` [L:143]
  - Modifiers: public, static, this
- `static void Sharp.Shared.Utilities.Utils.WriteInt64(nint ptr, int offset, long value)` [L:117]
  - Modifiers: public, static, this
- `static void Sharp.Shared.Utilities.Utils.WritePtr(nint @this, int offset, nint ptr)` [L:304]
  - Modifiers: public, static, this
- `static void Sharp.Shared.Utilities.Utils.WriteString(sbyte* ptr, int size, string value)` [L:35]
  - Modifiers: public, static
- `static void Sharp.Shared.Utilities.Utils.WriteStringUtf8(char* ptr, int size, string value)` [L:60]
  - Modifiers: public, static
- `static void Sharp.Shared.Utilities.Utils.WriteStringUtf8(nint ptr, int offset, string value, int maxlen)` [L:53]
  - Modifiers: public, static, this
- `static void Sharp.Shared.Utilities.Utils.WriteUInt16(nint ptr, int offset, ushort value)` [L:182]
  - Modifiers: public, static, this
- `static void Sharp.Shared.Utilities.Utils.WriteUInt32(nint ptr, int offset, uint value)` [L:156]
  - Modifiers: public, static, this
- `static void Sharp.Shared.Utilities.Utils.WriteUInt64(nint ptr, int offset, ulong value)` [L:130]
  - Modifiers: public, static, this
- `static void Sharp.Shared.Utilities.Utils.WriteVector(nint ptr, int offset, Sharp.Shared.Types.Vector vector)` [L:313]
  - Modifiers: public, static, this


