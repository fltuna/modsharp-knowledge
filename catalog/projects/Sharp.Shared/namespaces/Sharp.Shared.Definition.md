# Sharp.Shared.Definition

Project: Sharp.Shared
Types: 3 (0 generated)

### class ChatColor

- FullName: `Sharp.Shared.Definition.ChatColor`
- Kind: class
- Modifiers: public, static
- Source: Sharp.Shared/Definition/ChatColor.cs:27
- Generated: false

Inheritance: object → **ChatColor**

#### Fields
- `const char Sharp.Shared.Definition.ChatColor.NewLine = '\u2029'` [L:47]
  - Modifiers: public, static, const
- `const string Sharp.Shared.Definition.ChatColor.Blue = "\v"` [L:40]
  - Modifiers: public, static, const
- `const string Sharp.Shared.Definition.ChatColor.DarkBlue = "\f"` [L:41]
  - Modifiers: public, static, const
- `const string Sharp.Shared.Definition.ChatColor.DarkRed = "\u0002"` [L:30]
  - Modifiers: public, static, const
- `const string Sharp.Shared.Definition.ChatColor.Gold = "\u0010"` [L:38]
  - Modifiers: public, static, const
- `const string Sharp.Shared.Definition.ChatColor.Green = "\u0004"` [L:32]
  - Modifiers: public, static, const
- `const string Sharp.Shared.Definition.ChatColor.Grey = "\b"` [L:36]
  - Modifiers: public, static, const
- `const string Sharp.Shared.Definition.ChatColor.Head = "\u0003"` [L:45]
  - Modifiers: public, static, const
- `const string Sharp.Shared.Definition.ChatColor.LightGreen = "\u0005"` [L:33]
  - Modifiers: public, static, const
- `const string Sharp.Shared.Definition.ChatColor.LightRed = "\u000f"` [L:43]
  - Modifiers: public, static, const
- `const string Sharp.Shared.Definition.ChatColor.Lime = "\u0006"` [L:34]
  - Modifiers: public, static, const
- `const string Sharp.Shared.Definition.ChatColor.Muted = "\n"` [L:44]
  - Modifiers: public, static, const
- `const string Sharp.Shared.Definition.ChatColor.Pink = "\u0003"` [L:31]
  - Modifiers: public, static, const
- `const string Sharp.Shared.Definition.ChatColor.Purple = "\u000e"` [L:42]
  - Modifiers: public, static, const
- `const string Sharp.Shared.Definition.ChatColor.Red = "\a"` [L:35]
  - Modifiers: public, static, const
- `const string Sharp.Shared.Definition.ChatColor.Silver = "\n"` [L:39]
  - Modifiers: public, static, const
- `const string Sharp.Shared.Definition.ChatColor.White = "\u0001"` [L:29]
  - Modifiers: public, static, const
- `const string Sharp.Shared.Definition.ChatColor.Yellow = "\t"` [L:37]
  - Modifiers: public, static, const

#### Methods
- `static string Sharp.Shared.Definition.ChatColor.GetColor(Sharp.Shared.Enums.CStrikeTeam team)` [L:49]
  - Modifiers: public, static, this


### class PreservedEntities

- FullName: `Sharp.Shared.Definition.PreservedEntities`
- Kind: class
- Modifiers: public, static
- Source: Sharp.Shared/Definition/PreservedEntities.cs:33
- Generated: false
- Summary: Persistent entities

Inheritance: object → **PreservedEntities**

#### Methods
- `static System.Collections.Frozen.FrozenSet<string> Sharp.Shared.Definition.PreservedEntities.GetPreservedEntities()` [L:136]
  - Modifiers: public, static
  - Summary: Gets the list of persistent entities
- `static bool Sharp.Shared.Definition.PreservedEntities.IsPreservedEntity(Sharp.Shared.GameEntities.IBaseEntity entity)` [L:124]
  - Modifiers: public, static, this
  - Summary: Determines whether the current entity is a persistent entity
- `static bool Sharp.Shared.Definition.PreservedEntities.IsPreservedEntity(string classname)` [L:130]
  - Modifiers: public, static
  - Summary: Determines whether this class is a persistent entity


### class UsefulInteractionLayers

- FullName: `Sharp.Shared.Definition.UsefulInteractionLayers`
- Kind: class
- Modifiers: public, static
- Source: Sharp.Shared/Definition/UsefulInteractionLayers.cs:24
- Generated: false

Inheritance: object → **UsefulInteractionLayers**

#### Fields
- `const Sharp.Shared.Enums.InteractionLayers Sharp.Shared.Definition.UsefulInteractionLayers.BrushOnly = Sharp.Shared.Enums.InteractionLayers.Solid | Sharp.Shared.Enums.InteractionLayers.HitBoxes | Sharp.Shared.Enums.InteractionLayers.Sky | Sharp.Shared.Enums.InteractionLayers.WorldGeometry | Sharp.Shared.Enums.InteractionLayers.Slime` [L:74]
  - Modifiers: public, static, const
  - Summary: Copy from Brush trace in game code
- `const Sharp.Shared.Enums.InteractionLayers Sharp.Shared.Definition.UsefulInteractionLayers.FireBullets = Sharp.Shared.Enums.InteractionLayers.Solid | Sharp.Shared.Enums.InteractionLayers.HitBoxes | Sharp.Shared.Enums.InteractionLayers.Sky | Sharp.Shared.Enums.InteractionLayers.Window | Sharp.Shared.Enums.InteractionLayers.PassBullets | Sharp.Shared.Enums.InteractionLayers.Player | Sharp.Shared.Enums.InteractionLayers.Npc | Sharp.Shared.Enums.InteractionLayers.Debris` [L:46]
  - Modifiers: public, static, const
  - Summary: Copy from FireBullets in game code
- `const Sharp.Shared.Enums.InteractionLayers Sharp.Shared.Definition.UsefulInteractionLayers.PlayerPing = Sharp.Shared.Enums.InteractionLayers.Solid | Sharp.Shared.Enums.InteractionLayers.HitBoxes | Sharp.Shared.Enums.InteractionLayers.Window | Sharp.Shared.Enums.InteractionLayers.Player | Sharp.Shared.Enums.InteractionLayers.Npc | Sharp.Shared.Enums.InteractionLayers.Debris` [L:62]
  - Modifiers: public, static, const
  - Summary: Copy from ping in game code
- `const Sharp.Shared.Enums.InteractionLayers Sharp.Shared.Definition.UsefulInteractionLayers.SwingOrStab = Sharp.Shared.Enums.InteractionLayers.Solid | Sharp.Shared.Enums.InteractionLayers.Window | Sharp.Shared.Enums.InteractionLayers.PassBullets | Sharp.Shared.Enums.InteractionLayers.Player | Sharp.Shared.Enums.InteractionLayers.Npc` [L:33]
  - Modifiers: public, static, const
  - Summary: Copy from SwingOrStab in game code


