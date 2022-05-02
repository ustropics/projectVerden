
# This is a RE-UPLOAD with the most up-to-date H&H version from nexus, **aedenthorn** is the author of this mod.

* Original Author of this mod is **aedenthorn** from nexus mods
* [Original Mod](https://www.nexusmods.com/valheim/mods/1162)

## Permissions as of 23/01/2022, Upload permission.
![Permissions](https://i.imgur.com/iZd10IE.png)

## Mod Information (Below is the original information from nexus):

This mod lets you edit various stats for individual armor pieces and has two global armor multipliers as well. It also adds the possibility for new resistance types, and implements a new Water resistance against the Wet status effect.

This mod also fixes a bug in the vanilla game that makes it not recognize frost immunity for environmental cold.


## Setting Armor Stats

Custom armor stats are stored in json files in **BepInEx\plugins\CustomArmorStats**. To create a template json file for a specific armor piece, type the following command in the console (F5):

**customarmorstats save <ItemSpawnName>**

E.g. **customarmorstats save ArmorBronzeLegs** will create a file called ArmorBronzeLegs.json with the default values for Bronze leggings.  Edit that file as you
like, save it, then type the following command in the console:

**customarmorstats reload**

This will reload the file, applying the new values when an item is created or moved to a new inventory.

The variables are mostly self-explanatory.

Damage modifiers are a list of colon-separated pairs, e.g. for the Wolf Chest armor:

**"damageModifiers":["Frost:Resistant"]**

The first value is the damage type, the second value is the resistance level.

Valid damage types include:

Blunt
Slash
Pierce
Chop
Pickaxe
Physical
Fire
Frost
Lightning
Elemental
Poison
Spirit
Water (this is a new type, affecting the Wet status)

Valid resistence levels include:

Normal
Resistant
Weak
Immune
Ignore
VeryResistant
VeryWeak


You can also dump these lists using

**customarmorstats damagetypes**

**customarmorstats damagemods**


## Water Resistance

Water resistance provides the following modifiers, depending on the resistance level:

Normal - no change
Resistant - increases Wet status countdown speed by 100%
Weak - decreases Wet status countdown speed by 1/3
Immune - prevents Wet status effect
Ignore - prevents Wet status effect
VeryResistant - prevent wet status effect application except when swimming, increases Wet status countdown speed by 100%
VeryWeak - decreases Wet status countdown speed by 2/3


## Global Multipliers

The mod also provides the following global armor modifiers via the config file:

**GlobalArmorDurabilityLossMult**

**GlobalArmorMovementModMult**


## Config

A config file **BepInEx/config/aedenthorn.CustomArmorStats.cfg** is created after running the game once with this mod.

You can adjust the config values by editing this file using a text editor or in-game using the Config Manager﻿.

To reload the config from the config file, type **customarmorstats reset** into the game's console (F5).
## Technical

To install manually, place the dll file in the BepInEx/plugins folder. You will need BepInEx.

Code is at https://github.com/aedenthorn/ValheimMods.

﻿﻿If you want to complain or ask for help or help me test my mods, you can visit my Discord server. ﻿https://www.discord.com/invite/bs6zHuj

[Click here for a list of all my mods for Valheim.](https://www.nexusmods.com/valheim/articles/104)