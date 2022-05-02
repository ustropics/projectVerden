# Reely SpecTackleLure

## Fishing skill, craftable gear, fishing tweaks, and ... danger?

**Now with craftable, upgradeable fishing rod and craftable bait!**

You've fished...and fished...and fished. And you have little to show for all your effort. 

Reely SpecTackleLure adds a Fishing skill that improves your ability to hook fish as your skill increases.

- Fish within range will begin to splash the surface when you cast your line to give you an idea if you've found a good location
- Fish are excited by your bait and will converge on your float faster & from farther away
- Fish won't spend as much time milling around or bottom feeding while you're fishing; they'll go after your bait more often
- Upgrading your fishing rod works in addition to your fishing skill to increase your chance of hooking fish
- Adjustable float size to make it larger and more visible in the water
- Option to remove fish spawn restrictions near player created objects such as crafting stations and fires.

**And a word of caution when deep-sea fishing ... the ocean can be a dangerous place. Be careful what you _fish_ for!**

## Version 0.1.7

- Fixed issue checking ocean depth before spawning deep sea creatures.

### Previous Updates

- Externalized rod and bait recipes for crafting-oriented servers to control recipes.
	- To change the recipes, modify the RSTLrecipes.json file in the mod directory. _Note: Don't change the name of the recipe_
- Added an option to override fish spawn restrictions around player created objects.
	- This will allow a chance for fish to spawn near structures and bases. _See note below_
- Fixed bug where rod durability would increase when containers with rods inside were opened
- Reduced initial durability to match basic merchant purchased rod
- Increased maximum craftable item quality to 4
- Updated to work with Auga UI
- Fixed rods not showing level or wear in containers
- Revised spawn mechanics to remove cast spamming
- Added craftable rod and bait. Rod can be upgradced to improve your fishing chance. 
    - Note that upgraded rods only add to the hook chance if you're using Reely SpecTackleLure's fishing skill. See note below on how to use RSTL's fishing skill while still using MoreSkills for other skills.
- Added configuration to allow other mods (e.g., More Skills) to manage the fishing skill, with RSTL still providing its craftable gear, fishing tweaks and deep-sea danger.
- Abbreviated the chat command to /rstl
- Added a _small_ chance of spawning a level 3 (2 star) serpent in the ocean. You'll need a longboat and probably a friend for this one.

## Configuration

### General

- **UseFishingSkill**: Set to false to allow another mod to manage the fishing skill. RSTL will sill provide its fishing tweaks, craftable items and deep-sea danger. Default is true (RSTL fishing skill enabled)
- **DetectionRadius**: The maximum distance from the fishing float to search for fish. Default is 25. Can be set from 10 to 50
- **FloatSize**: The size of the float. Increase to make the float larger and more visible in the water. Valheim default size is 1. Can be set from 1 to 3
- **NoBaseRestrictedSpawn**: Removes the restriction from fish spawning due to proximity to player created objects such as crafting stations and fires. _See note below_

### Utility

- **LogLevel**: Controls the level of information in the log
- **FishingSkillID**: The numeric identifier for the Fishing skill. Only change this if you have a conflict with another custom skill using ID 879. Can be set from 200 to 900. _Note that changing this value will reset your Fishing skill_

### In-game reconfiguration

You can use Configuration Manager (or similar) mod to change the configuration without exiting the game, and force Reely SpecTackleLure to update its configuration from the chat window (press Enter) then type:

    /rstl config 

You can also modify the detection radius and float size directly from the chat window using this syntax:

    /rstl detectionradius=40


## Compatibility issues & defects

- If you find a compatibility issue you can post it on NexusMods. Be sure to include the mod name and version you think may be incompatible.
- If you have a bug please report it on NexusMods. If you do post a bug report, please make sure to include the following:
    - Your version of this mod
    - What you were doing, or attempting to do when it happened
    - If it's repeatable - i.e., can you duplicate it?
    - The exact behavior you observed (or didn't observe)
    - If possible, a capture of the log file with errors (errors always begin with this mod's name ...")

## Notes

- Reely SpecTackleLure won't spawn additional fish or radically change fishing mechanics. You still have to catch fish, although it gets easier as your skill increases.
- With every advantage there's a cost; your fishing rod now has wear and tear and needs to be repaired occasionally.
- To use RSTL's fishing skill with MoreSkills installed, you need to set _Enable Fishing Skill = false_ in the MoreSkills _FishingConfig_ file.
- There are number of factors that restrict spawning other than proximity to player created objects. Fish spawning at a particular location is not guaranteed, even if _NoBaseRestrictedSpawn_ set to true.

- Shameless plugs for other mods:
    - WolfPack: Control all your tame creatures at once! https://www.nexusmods.com/valheim/mods/1549/
    - RequipMe: Instantly re-equip your best gear from your tombstone! https://www.nexusmods.com/valheim/mods/1615
    - UnRemove: Restore your destroyed pieces without rebuilding them... https://www.nexusmods.com/valheim/mods/1676
	
- Your comments and feedback are always welcome. Please feel free to post or send a note on NexusMods.