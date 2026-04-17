# Sharp.Core.Helpers

Project: Sharp.Core
Types: 1 (0 generated)

### class SchemaSystem

- FullName: `Sharp.Core.Helpers.SchemaSystem`
- Kind: class
- Modifiers: public, static
- Source: Sharp.Core/Helpers/SchemaSystem.cs:34
- Generated: false

Inheritance: object → **SchemaSystem**

#### Methods
- `static Sharp.Shared.DataMapField? Sharp.Core.Helpers.SchemaSystem.GetDataMapField(string classname, string fieldName)` [L:412]
  - Modifiers: public, static
- `static Sharp.Shared.SchemaField Sharp.Core.Helpers.SchemaSystem.GetSchemaField(string classname, string field)` [L:36]
  - Modifiers: public, static
- `static Sharp.Shared.Types.Vector Sharp.Core.Helpers.SchemaSystem.GetNetVarVector(nint ptr, string classname, string field, [ushort extraOffset = 0])` [L:131]
  - Modifiers: public, static
- `static System.Collections.Generic.List<Sharp.Shared.DataMapField> Sharp.Core.Helpers.SchemaSystem.GetDataMapFields(string classname)` [L:405]
  - Modifiers: public, static
- `static bool Sharp.Core.Helpers.SchemaSystem.FindNetVar(string classname, string field)` [L:390]
  - Modifiers: public, static
- `static bool Sharp.Core.Helpers.SchemaSystem.GetNetVarBool(nint ptr, string classname, string field, [ushort extraOffset = 0])` [L:98]
  - Modifiers: public, static
- `static byte Sharp.Core.Helpers.SchemaSystem.GetNetVarByte(nint ptr, string classname, string field, [ushort extraOffset = 0])` [L:101]
  - Modifiers: public, static
- `static byte Sharp.Core.Helpers.SchemaSystem.GetSchemaClassAlignOf(string classname)` [L:89]
  - Modifiers: public, static
- `static float Sharp.Core.Helpers.SchemaSystem.GetNetVarFloat(nint ptr, string classname, string field, [ushort extraOffset = 0])` [L:122]
  - Modifiers: public, static
- `static int Sharp.Core.Helpers.SchemaSystem.GetNetVarInt32(nint ptr, string classname, string field, [ushort extraOffset = 0])` [L:110]
  - Modifiers: public, static
- `static int Sharp.Core.Helpers.SchemaSystem.GetNetVarOffset(string classname, string field)` [L:92]
  - Modifiers: public, static
- `static int Sharp.Core.Helpers.SchemaSystem.GetNetVarOffset(string classname, string field, ushort extraOffset)` [L:95]
  - Modifiers: public, static
- `static int Sharp.Core.Helpers.SchemaSystem.GetSchemaClassSize(string classname)` [L:86]
  - Modifiers: public, static
- `static long Sharp.Core.Helpers.SchemaSystem.GetNetVarInt64(nint ptr, string classname, string field, [ushort extraOffset = 0])` [L:116]
  - Modifiers: public, static
- `static nint Sharp.Core.Helpers.SchemaSystem.GetDataMapInputFunc(string classname, string fieldName)` [L:419]
  - Modifiers: public, static
- `static nint Sharp.Core.Helpers.SchemaSystem.GetNetVarPointer(nint ptr, string classname, string field, [ushort extraOffset = 0])` [L:125]
  - Modifiers: public, static
- `static ref Sharp.Shared.Types.Tier.CUtlString Sharp.Core.Helpers.SchemaSystem.GetNetVarUtlStringRef(nint ptr, string classname, string field, [ushort extraOffset = 0])` [L:164]
  - Modifiers: public, static
- `static ref Sharp.Shared.Types.Tier.CUtlSymbolLarge Sharp.Core.Helpers.SchemaSystem.GetNetVarUtlSymbolLargeRef(nint ptr, string classname, string field, [ushort extraOffset = 0])` [L:145]
  - Modifiers: public, static
- `static short Sharp.Core.Helpers.SchemaSystem.GetNetVarInt16(nint ptr, string classname, string field, [ushort extraOffset = 0])` [L:104]
  - Modifiers: public, static
- `static string Sharp.Core.Helpers.SchemaSystem.GetNetVarString(nint ptr, string classname, string field, [ushort extraOffset = 0])` [L:128]
  - Modifiers: public, static
- `static string Sharp.Core.Helpers.SchemaSystem.GetNetVarUtlString(nint ptr, string classname, string field, [ushort extraOffset = 0])` [L:156]
  - Modifiers: public, static
- `static string Sharp.Core.Helpers.SchemaSystem.GetNetVarUtlSymbolLarge(nint ptr, string classname, string field, [ushort extraOffset = 0])` [L:134]
  - Modifiers: public, static
- `static uint Sharp.Core.Helpers.SchemaSystem.GetNetVarUInt32(nint ptr, string classname, string field, [ushort extraOffset = 0])` [L:113]
  - Modifiers: public, static
- `static ulong Sharp.Core.Helpers.SchemaSystem.GetNetVarUInt64(nint ptr, string classname, string field, [ushort extraOffset = 0])` [L:119]
  - Modifiers: public, static
- `static ushort Sharp.Core.Helpers.SchemaSystem.GetNetVarUInt16(nint ptr, string classname, string field, [ushort extraOffset = 0])` [L:107]
  - Modifiers: public, static
- `static void Sharp.Core.Helpers.SchemaSystem.NetVarStateChanged(nint ptr, Sharp.Shared.SchemaClass schemaClass, Sharp.Shared.SchemaClassField schemaField, [ushort extraOffset = 0], [bool isStruct = false])` [L:368]
  - Modifiers: public, static
- `static void Sharp.Core.Helpers.SchemaSystem.NetworkStateChanged(nint ptr, string classname, string field, [bool isStruct = false], [ushort extraOffset = 0])` [L:448]
  - Modifiers: public, static
- `static void Sharp.Core.Helpers.SchemaSystem.SetNetVarBool(nint ptr, string classname, string field, bool value, [bool isStruct = false], [ushort extraOffset = 0])` [L:172]
  - Modifiers: public, static
- `static void Sharp.Core.Helpers.SchemaSystem.SetNetVarByte(nint ptr, string classname, string field, byte value, [bool isStruct = false], [ushort extraOffset = 0])` [L:180]
  - Modifiers: public, static
- `static void Sharp.Core.Helpers.SchemaSystem.SetNetVarFloat(nint ptr, string classname, string field, float value, [bool isStruct = false], [ushort extraOffset = 0])` [L:285]
  - Modifiers: public, static
- `static void Sharp.Core.Helpers.SchemaSystem.SetNetVarInt16(nint ptr, string classname, string field, short value, [bool isStruct = false], [ushort extraOffset = 0])` [L:195]
  - Modifiers: public, static
- `static void Sharp.Core.Helpers.SchemaSystem.SetNetVarInt32(nint ptr, string classname, string field, int value, [bool isStruct = false], [ushort extraOffset = 0])` [L:225]
  - Modifiers: public, static
- `static void Sharp.Core.Helpers.SchemaSystem.SetNetVarInt64(nint ptr, string classname, string field, long value, [bool isStruct = false], [ushort extraOffset = 0])` [L:255]
  - Modifiers: public, static
- `static void Sharp.Core.Helpers.SchemaSystem.SetNetVarString(nint ptr, string classname, string field, string value, int length, [bool isStruct = false], [ushort extraOffset = 0])` [L:300]
  - Modifiers: public, static
- `static void Sharp.Core.Helpers.SchemaSystem.SetNetVarUInt16(nint ptr, string classname, string field, ushort value, [bool isStruct = false], [ushort extraOffset = 0])` [L:210]
  - Modifiers: public, static
- `static void Sharp.Core.Helpers.SchemaSystem.SetNetVarUInt32(nint ptr, string classname, string field, uint value, [bool isStruct = false], [ushort extraOffset = 0])` [L:240]
  - Modifiers: public, static
- `static void Sharp.Core.Helpers.SchemaSystem.SetNetVarUInt64(nint ptr, string classname, string field, ulong value, [bool isStruct = false], [ushort extraOffset = 0])` [L:270]
  - Modifiers: public, static
- `static void Sharp.Core.Helpers.SchemaSystem.SetNetVarUtlString(nint ptr, string classname, string field, string value, [bool isStruct = false], [ushort extraOffset = 0])` [L:335]
  - Modifiers: public, static
- `static void Sharp.Core.Helpers.SchemaSystem.SetNetVarUtlSymbolLarge(nint ptr, string classname, string field, string value, [bool isStruct = false], [ushort extraOffset = 0])` [L:316]
  - Modifiers: public, static
- `static void Sharp.Core.Helpers.SchemaSystem.SetNetVarVector(nint ptr, string classname, string field, Sharp.Shared.Types.Vector value, [bool isStruct = false], [ushort extraOffset = 0])` [L:351]
  - Modifiers: public, static


