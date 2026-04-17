# Sharp.Shared.Types.CppProtobuf

Project: Sharp.Shared
Types: 9 (0 generated)

### struct CBaseUserCmdPb : System.ValueType

- FullName: `Sharp.Shared.Types.CppProtobuf.CBaseUserCmdPb`
- Kind: struct
- Modifiers: public, ref
- Source: Sharp.Shared/Types/CppProtobuf/UserCmdPb.cs:134
- Generated: false
- Attributes: `[StructLayout(2, Pack = 8, Size = 136)]`

Inheritance: object → System.ValueType → **CBaseUserCmdPb**

#### Fields
- `Sharp.Shared.Types.CEntityHandle<Sharp.Shared.GameEntities.IPlayerPawn> Sharp.Shared.Types.CppProtobuf.CBaseUserCmdPb.PawnEntityHandle` [L:188]
  - Attributes: `[FieldOffset(132)]`
- `Sharp.Shared.Types.CppProtobuf.CInButtonStatePb* Sharp.Shared.Types.CppProtobuf.CBaseUserCmdPb.ButtonState` [L:140]
  - Attributes: `[FieldOffset(56)]`
- `Sharp.Shared.Types.CppProtobuf.CMsgVector* Sharp.Shared.Types.CppProtobuf.CBaseUserCmdPb.ViewAngles` [L:143]
  - Attributes: `[FieldOffset(64)]`
- `Sharp.Shared.Types.CppProtobuf.RepeatedField<Sharp.Shared.Types.CppProtobuf.CSubtickMoveStepPb> Sharp.Shared.Types.CppProtobuf.CBaseUserCmdPb.SubtickMoves` [L:137]
  - Attributes: `[FieldOffset(24)]`
- `float Sharp.Shared.Types.CppProtobuf.CBaseUserCmdPb.ForwardMove` [L:155]
  - Attributes: `[FieldOffset(88)]`
- `float Sharp.Shared.Types.CppProtobuf.CBaseUserCmdPb.SideMove` [L:158]
  - Attributes: `[FieldOffset(92)]`
- `float Sharp.Shared.Types.CppProtobuf.CBaseUserCmdPb.UpMove` [L:161]
  - Attributes: `[FieldOffset(96)]`
- `int Sharp.Shared.Types.CppProtobuf.CBaseUserCmdPb.ClientTick` [L:152]
  - Attributes: `[FieldOffset(84)]`
- `int Sharp.Shared.Types.CppProtobuf.CBaseUserCmdPb.CmdFlags` [L:185]
  - Attributes: `[FieldOffset(128)]`
- `int Sharp.Shared.Types.CppProtobuf.CBaseUserCmdPb.Impulse` [L:164]
  - Attributes: `[FieldOffset(100)]`
- `int Sharp.Shared.Types.CppProtobuf.CBaseUserCmdPb.LegacyCommandNumber` [L:149]
  - Attributes: `[FieldOffset(80)]`
- `int Sharp.Shared.Types.CppProtobuf.CBaseUserCmdPb.MouseX` [L:173]
  - Attributes: `[FieldOffset(112)]`
- `int Sharp.Shared.Types.CppProtobuf.CBaseUserCmdPb.MouseY` [L:176]
  - Attributes: `[FieldOffset(116)]`
- `int Sharp.Shared.Types.CppProtobuf.CBaseUserCmdPb.RandomSeed` [L:170]
  - Attributes: `[FieldOffset(108)]`
- `int Sharp.Shared.Types.CppProtobuf.CBaseUserCmdPb.WeaponSelect` [L:167]
  - Attributes: `[FieldOffset(104)]`
- `uint Sharp.Shared.Types.CppProtobuf.CBaseUserCmdPb.ConsumedServerAngleChanges` [L:182]
  - Attributes: `[FieldOffset(124)]`
- `uint Sharp.Shared.Types.CppProtobuf.CBaseUserCmdPb.PredictionOffsetTicks` [L:179]
  - Attributes: `[FieldOffset(120)]`
- `void* Sharp.Shared.Types.CppProtobuf.CBaseUserCmdPb.ExecutionNotes` [L:146]
  - Attributes: `[FieldOffset(72)]`


### struct CCSGOInputHistoryEntryPb : System.ValueType

- FullName: `Sharp.Shared.Types.CppProtobuf.CCSGOInputHistoryEntryPb`
- Kind: struct
- Modifiers: public
- Source: Sharp.Shared/Types/CppProtobuf/UserCmdPb.cs:47
- Generated: false
- Attributes: `[StructLayout(2, Pack = 8, Size = 120)]`

Inheritance: object → System.ValueType → **CCSGOInputHistoryEntryPb**

#### Fields
- `Sharp.Shared.Types.CppProtobuf.CMsgVector* Sharp.Shared.Types.CppProtobuf.CCSGOInputHistoryEntryPb.ShootPosition` [L:65]
  - Attributes: `[FieldOffset(64)]`
- `Sharp.Shared.Types.CppProtobuf.CMsgVector* Sharp.Shared.Types.CppProtobuf.CCSGOInputHistoryEntryPb.TargetAbsPositionCheck` [L:71]
  - Attributes: `[FieldOffset(80)]`
- `Sharp.Shared.Types.CppProtobuf.CMsgVector* Sharp.Shared.Types.CppProtobuf.CCSGOInputHistoryEntryPb.TargetAngPositionCheck` [L:74]
  - Attributes: `[FieldOffset(88)]`
- `Sharp.Shared.Types.CppProtobuf.CMsgVector* Sharp.Shared.Types.CppProtobuf.CCSGOInputHistoryEntryPb.TargetHeadPositionCheck` [L:68]
  - Attributes: `[FieldOffset(72)]`
- `Sharp.Shared.Types.CppProtobuf.CMsgVector* Sharp.Shared.Types.CppProtobuf.CCSGOInputHistoryEntryPb.ViewAngles` [L:50]
  - Attributes: `[FieldOffset(24)]`
- `Sharp.Shared.Types.CppProtobuf.CSGOInterpolationInfoPB* Sharp.Shared.Types.CppProtobuf.CCSGOInputHistoryEntryPb.PlayerInterp` [L:62]
  - Attributes: `[FieldOffset(56)]`
- `Sharp.Shared.Types.CppProtobuf.CSGOInterpolationInfoPB* Sharp.Shared.Types.CppProtobuf.CCSGOInputHistoryEntryPb.SvInterp0` [L:56]
  - Attributes: `[FieldOffset(40)]`
- `Sharp.Shared.Types.CppProtobuf.CSGOInterpolationInfoPB* Sharp.Shared.Types.CppProtobuf.CCSGOInputHistoryEntryPb.SvInterp1` [L:59]
  - Attributes: `[FieldOffset(48)]`
- `Sharp.Shared.Types.CppProtobuf.CSGOInterpolationInfoPB_CL* Sharp.Shared.Types.CppProtobuf.CCSGOInputHistoryEntryPb.ClInterp` [L:53]
  - Attributes: `[FieldOffset(32)]`
- `float Sharp.Shared.Types.CppProtobuf.CCSGOInputHistoryEntryPb.PlayerTickFraction` [L:86]
  - Attributes: `[FieldOffset(108)]`
- `float Sharp.Shared.Types.CppProtobuf.CCSGOInputHistoryEntryPb.RenderTickFraction` [L:80]
  - Attributes: `[FieldOffset(100)]`
- `int Sharp.Shared.Types.CppProtobuf.CCSGOInputHistoryEntryPb.FrameNumber` [L:89]
  - Attributes: `[FieldOffset(112)]`
- `int Sharp.Shared.Types.CppProtobuf.CCSGOInputHistoryEntryPb.PlayerTickCount` [L:83]
  - Attributes: `[FieldOffset(104)]`
- `int Sharp.Shared.Types.CppProtobuf.CCSGOInputHistoryEntryPb.RenderTickCount` [L:77]
  - Attributes: `[FieldOffset(96)]`
- `int Sharp.Shared.Types.CppProtobuf.CCSGOInputHistoryEntryPb.TargetEntIndex` [L:92]
  - Attributes: `[FieldOffset(116)]`


### struct CCSGOUserCmdPb : System.ValueType

- FullName: `Sharp.Shared.Types.CppProtobuf.CCSGOUserCmdPb`
- Kind: struct
- Modifiers: public, ref
- Source: Sharp.Shared/Types/CppProtobuf/UserCmdPb.cs:192
- Generated: false
- Attributes: `[StructLayout(2, Pack = 8, Size = 72)]`

Inheritance: object → System.ValueType → **CCSGOUserCmdPb**

#### Fields
- `Sharp.Shared.Types.CppProtobuf.CBaseUserCmdPb* Sharp.Shared.Types.CppProtobuf.CCSGOUserCmdPb.BaseUserCmd` [L:198]
  - Attributes: `[FieldOffset(48)]`
- `Sharp.Shared.Types.CppProtobuf.RepeatedField<Sharp.Shared.Types.CppProtobuf.CCSGOInputHistoryEntryPb> Sharp.Shared.Types.CppProtobuf.CCSGOUserCmdPb.InputHistoryEntry` [L:195]
  - Attributes: `[FieldOffset(24)]`
- `bool Sharp.Shared.Types.CppProtobuf.CCSGOUserCmdPb.IsPredictingBodyShot` [L:204]
  - Attributes: `[FieldOffset(57)]`
- `bool Sharp.Shared.Types.CppProtobuf.CCSGOUserCmdPb.IsPredictingHeadShot` [L:207]
  - Attributes: `[FieldOffset(58)]`
- `bool Sharp.Shared.Types.CppProtobuf.CCSGOUserCmdPb.IsPredictingKillShot` [L:210]
  - Attributes: `[FieldOffset(59)]`
- `bool Sharp.Shared.Types.CppProtobuf.CCSGOUserCmdPb.LeftHandDesired` [L:201]
  - Attributes: `[FieldOffset(56)]`
- `int Sharp.Shared.Types.CppProtobuf.CCSGOUserCmdPb.Attack1StartHistoryIndex` [L:213]
  - Attributes: `[FieldOffset(60)]`
- `int Sharp.Shared.Types.CppProtobuf.CCSGOUserCmdPb.Attack2StartHistoryIndex` [L:216]
  - Attributes: `[FieldOffset(64)]`


### struct CInButtonStatePb : System.ValueType

- FullName: `Sharp.Shared.Types.CppProtobuf.CInButtonStatePb`
- Kind: struct
- Modifiers: public, ref
- Source: Sharp.Shared/Types/CppProtobuf/UserCmdPb.cs:121
- Generated: false
- Attributes: `[StructLayout(2, Pack = 8, Size = 32)]`

Inheritance: object → System.ValueType → **CInButtonStatePb**

#### Fields
- `Sharp.Shared.Enums.UserCommandButtons Sharp.Shared.Types.CppProtobuf.CInButtonStatePb.ButtonChanged` [L:127]
  - Attributes: `[FieldOffset(32)]`
- `Sharp.Shared.Enums.UserCommandButtons Sharp.Shared.Types.CppProtobuf.CInButtonStatePb.ButtonPressed` [L:124]
  - Attributes: `[FieldOffset(24)]`
- `Sharp.Shared.Enums.UserCommandButtons Sharp.Shared.Types.CppProtobuf.CInButtonStatePb.ButtonScroll` [L:130]
  - Attributes: `[FieldOffset(40)]`


### struct CMsgVector : System.ValueType

- FullName: `Sharp.Shared.Types.CppProtobuf.CMsgVector`
- Kind: struct
- Modifiers: public
- Source: Sharp.Shared/Types/CppProtobuf/CMsgVector.cs:25
- Generated: false
- Attributes: `[StructLayout(2, Pack = 8, Size = 36)]`

Inheritance: object → System.ValueType → **CMsgVector**

#### Fields
- `Sharp.Shared.Types.Vector Sharp.Shared.Types.CppProtobuf.CMsgVector.Value` [L:28]
  - Attributes: `[FieldOffset(24)]`


### struct CSGOInterpolationInfoPB : System.ValueType

- FullName: `Sharp.Shared.Types.CppProtobuf.CSGOInterpolationInfoPB`
- Kind: struct
- Modifiers: public
- Source: Sharp.Shared/Types/CppProtobuf/UserCmdPb.cs:27
- Generated: false
- Attributes: `[StructLayout(2, Pack = 8, Size = 36)]`

Inheritance: object → System.ValueType → **CSGOInterpolationInfoPB**

#### Fields
- `float Sharp.Shared.Types.CppProtobuf.CSGOInterpolationInfoPB.Fraction` [L:30]
  - Attributes: `[FieldOffset(24)]`
- `int Sharp.Shared.Types.CppProtobuf.CSGOInterpolationInfoPB.DestTick` [L:36]
  - Attributes: `[FieldOffset(32)]`
- `int Sharp.Shared.Types.CppProtobuf.CSGOInterpolationInfoPB.SrcTick` [L:33]
  - Attributes: `[FieldOffset(28)]`


### struct CSGOInterpolationInfoPB_CL : System.ValueType

- FullName: `Sharp.Shared.Types.CppProtobuf.CSGOInterpolationInfoPB_CL`
- Kind: struct
- Modifiers: public
- Source: Sharp.Shared/Types/CppProtobuf/UserCmdPb.cs:40
- Generated: false
- Attributes: `[StructLayout(2, Pack = 8, Size = 28)]`

Inheritance: object → System.ValueType → **CSGOInterpolationInfoPB_CL**

#### Fields
- `float Sharp.Shared.Types.CppProtobuf.CSGOInterpolationInfoPB_CL.Fraction` [L:43]
  - Attributes: `[FieldOffset(24)]`


### struct CSubtickMoveStepPb : System.ValueType

- FullName: `Sharp.Shared.Types.CppProtobuf.CSubtickMoveStepPb`
- Kind: struct
- Modifiers: public
- Source: Sharp.Shared/Types/CppProtobuf/UserCmdPb.cs:96
- Generated: false
- Attributes: `[StructLayout(2, Pack = 8, Size = 56)]`

Inheritance: object → System.ValueType → **CSubtickMoveStepPb**

#### Fields
- `Sharp.Shared.Enums.UserCommandButtons Sharp.Shared.Types.CppProtobuf.CSubtickMoveStepPb.Buttons` [L:99]
  - Attributes: `[FieldOffset(24)]`
- `bool Sharp.Shared.Types.CppProtobuf.CSubtickMoveStepPb.Pressed` [L:102]
  - Attributes: `[FieldOffset(32)]`
- `float Sharp.Shared.Types.CppProtobuf.CSubtickMoveStepPb.AnalogForwardDelta` [L:108]
  - Attributes: `[FieldOffset(40)]`
- `float Sharp.Shared.Types.CppProtobuf.CSubtickMoveStepPb.AnalogLeftDelta` [L:111]
  - Attributes: `[FieldOffset(44)]`
- `float Sharp.Shared.Types.CppProtobuf.CSubtickMoveStepPb.AnalogPitchDelta` [L:114]
  - Attributes: `[FieldOffset(48)]`
- `float Sharp.Shared.Types.CppProtobuf.CSubtickMoveStepPb.AnalogYawDelta` [L:117]
  - Attributes: `[FieldOffset(52)]`
- `float Sharp.Shared.Types.CppProtobuf.CSubtickMoveStepPb.When` [L:105]
  - Attributes: `[FieldOffset(36)]`


### struct RepeatedField<T> : System.ValueType

- FullName: `Sharp.Shared.Types.CppProtobuf.RepeatedField<T>`
- Kind: struct
- Modifiers: public, readonly, ref
- Source: Sharp.Shared/Types/CppProtobuf/ProtobufRepeatField.cs:26
- Generated: false
- Attributes: `[StructLayout(0, Pack = 8, Size = 24)]`
- Constraint: `where T : struct, unmanaged`

Inheritance: object → System.ValueType → **RepeatedField**

#### Fields
- `readonly int Sharp.Shared.Types.CppProtobuf.RepeatedField<T>.nCurrentSize` [L:30]
  - Modifiers: public, readonly
- `readonly int Sharp.Shared.Types.CppProtobuf.RepeatedField<T>.nTotalSize` [L:32]
  - Modifiers: public, readonly

#### Properties
- `int Sharp.Shared.Types.CppProtobuf.RepeatedField<T>.nAllocatedSize` [L:37]
  - Modifiers: public, readonly

#### Indexers
- `T* Sharp.Shared.Types.CppProtobuf.RepeatedField<T>.this[int index]` [L:39]
  - Modifiers: public, readonly


