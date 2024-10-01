# 1.3.3
Released: October 1st 2024

## Changes
- Reverted desert spawning changes from 1.3.2

## Bug Fixes
- Climate zones now correctly generate in oceanless worlds
- Village buildings can no longer generate over water
    - However, this causes an issue where village buildings can generate sliced up

# 1.3.2
Released: September 29th 2024

## Changes

### Blocks
- Enchantment table
    - Can now re-enchant items that already have enchantments
    - Re-enchanting an item adds levels to pre-existing enchantments and adds new enchantments that weren't already there
- Sapling
    - Jungle saplings now grow into palm trees in archipelagos

### Mobs
- Despawning
    - Animals now despawn in the default and hardcore presets
    - Animals will never despawn if they've been bred with or if they are products of breeding, regardless of settings

### Enchantments
- Bane of Arthropods
    - Now compatible with sharpness
    - Reduced effectiveness by 2/3
- Protection
    - Reduced damage reduction:
        | Level | Old | New |
        |---|---|---|
        | x | (6 + x^2) / 3 | x
        | 1 | 2 | 1 |
        | 2 | 3 | 2 |
        | 3 | 5 | 3 |
        | 4 | 7 | 4 |
    - Adjusted enchantability
- Smite
    - Now compatible with sharpness
    - Reduced effectiveness by 2/3
- Stamina
    - Adjusted enchantability
- Velocity
    - Increased effectiveness per level by 1%
    - Adjusted enchantability
- Enchantments no longer have caps on their maximum available enchantability per level
    - This means that lower level enchantments can be obtained from higher levels of enchanting

### Gameplay
- Sprint jumping no longer increases exhaustion with hunger set to sprint only, but sprinting in mid-air does

### Biomes
- Desert
    - Made slightly more common
- Frosted Birch Forest
    - Adjusted biome colors
- Parched Forest
    - Doubled chance of generating big trees
- Rainforest
    - Added a chance for regular big trees to generate
    - No longer generates with vines in beta worlds
- Seasonal Forest
    - Readded to world generation
    - Adjusted climate
- Snowcapped Forest
    - No longer generates with beaches
- Snowcapped Peaks
    - Replaced with taigas in world generation
    - Snowcapped Peaks will likely be replaced by a different biome in a later update
- Adjusted height of some biomes
- Fixed climate values for beaches and highlands edges being inconsistent with plains and highlands respectively

### World Generation
- Customized world type
    - Added a "Beta Terrain" option
    - Random biome selection with beta terrain results in beta biome distribution
    - The size of landmasses in beta terrain scales with biome size
- Crop generation in villages has been reduced by a half
- Adjusted branch generation in big trees
- Ores generate 4 blocks higher
- Increased the size of palm trees

### Other
- Reduced arm swing speed by 2 ticks
- Selecting a single biome in the world customization menu now displays "Biome Selection" as "Single"
- Clicking and dragging with items has been added
- Fixed texture alignment of diamonds
- Reduced FOV modifier with speed effects by 50%
- Tweaked block light color
- Reduced volume of level up sound
- Biome height is no longer displayed in the debug menu

## Bug Fixes
- Fixed legacy world generation option in customized worlds
- Fixed sword blocking being inverted
- Fixed air bubbles in the hotbar in the wrong position
- Fixed controller support on Linux maybe?

# 1.3.1
Released: May 28th 2024

## Additions
- Added sprint cooldown multiplier to custom gamemode settings

## Changes
- Gamemodes can now be assigned presets so that they update with the correct properties in later versions
- Increased default ambient occlusion strength to 95%

## Bug Fixes
- HUD icons now display correctly with various game settings
- Restored beta seed parity (will create chunk borders in default worlds)
- Gamemodes with missing properties can now be loaded
- Sprint cooldown from taking damage now works in multiplayer

# 1.3
Released: May 22nd 2024

## Additions

### Gameplay
- Customized game modes
    - Allows the player to change a variety of different options to play the game their own way
    - Allows for hardcore mode and classic mode to be played correctly in multiplayer
    - Added vanilla preset for a vanilla-style experience
    - Options that are new to the mod:
        - Hunger Type: readded vanilla hunger system but with Minecraft 1.11 exhaustion values and a saturation overlay over the hunger bar
        - Plank Variants: allow different wood types to be crafted into different plank types or restrict planks to oak only
        - End Portals: enabled by default excluding the classic preset

### Biomes
- Frosted Birch Forest
    - Snowy variant of the Birch Forest
- Snowcapped Forest
    - Generates inside Snowcapped Hills
    - Slightly taller elevation

### Settings
- Shading settings
    - Replaced shading style with more customisability
    - Moved colored water from video settings to shading settings
    - Colored Lighting: on by default, gives block light a slight orange tint and night light a blue shade
    - Non-Solid AO: on by default, allows for ambient occlusion to appear on transparent blocks like leaves
    - Ambient Occlusion: 90% by default, controls strength/darkness of ambient occlusion
    - Murky Swamps: off by default, gives swamps a dark look

## Changes

### Blocks
- Cobblestone
    - Changed texture
- Cobblestone Stairs
    - Renamed from Stone Stairs
- Mossy Cobblestone
    - Renamed from Moss Stone
    - Changed Texture
- Mushrooms
    - Can now be placed in lit areas
- Mushroom Block
    - Drops with the respective cap or stem texture on all sides when mined with silk touch
    - Can now be used with shears to obtain the variant with pores on all sides
- Vines
    - Reduced growth

### Items
- Golden Apple
    - Increased health/hunger given to 10
- Golden Tools
    - Increased durability to 250
    - Increased damage by 1
    - Reduced efficiency to x10
    - Reduced enchantability to 12
- Pigman Flesh
    - Increased length, reduced strength and reduced probability of hunger effect to match vanilla Rotten Flesh
- Raw Porkchop
    - No longer gives the hunger effect
- Shears
    - Increased durability to 250

### Mobs
- Creeper
    - Reverted to pre-1.2 AI
    - Can now move while exploding again
    - Consequently, creepers no longer run away from cats and ocelots
- Zombie
    - No longer drops rare loot
- Zombie Pigman
    - No longer drops golden helmets

### Enchantments
- Bane of Arthropods
    - Reduced effectiveness by 1/4
- Fortune
    - Reduced effectiveness on ore:
        | Level | Old Chances | New Chances |
        |---|---|---|
        | 1 | 67% x1<br>33% x2<br>**AVG 1.33** | 67% x1<br>33% x2<br>**AVG 1.33** |
        | 2 | 50% x1<br>25% x2<br>25% x3<br>**AVG 1.75** | 33% x1<br>67% x2<br><br>**AVG 1.67** |
        | 3 | 40% x1<br>20% x2<br>20% x3<br>20% x4<br>**AVG 2.20** | 33% x1<br>33% x2<br>33% x3<br><br>**AVG 2.00** |
- Protection (and other related enchantments):
    - Reduced effectiveness by 1/3
- Sharpness
    - Reduced effectiveness by 1/3
- Smite
    - Reduced effectiveness by 1/4
- Stamina
    - Increased max level to V
    - Half as effective with hunger type set to hungry
- Velocity
    - Increased max level to V
    - Reduced speed increase per level from 8% to 5%
- Increased rarity of higher level enchantments
- Removed enchantment buff in hardcore mode

### Gameplay
- Classic and Hardcore gamemodes are now only available as customization presets
- Animals respawn 400x as often, just like before Minecraft Beta 1.7 except animals do not despawn
    - This change does not apply to hardcore mode
- Changed game mode descriptions to be more accurate
- The classic AI option now reverts all vanilla 1.2 mob AI changes
- Increased length of sprint cooldown when taking damage (0.5 -> 2 seconds for easy, 1 -> 3 seconds for normal and 1.5 -> 4 seconds for hard)
- Removed +1 extra damage from classic mode

### Biomes
- Desert
    - Removed desert wells
- Forest
    - Slightly increased temperature
- Jungle
    - Reduced amount of vines
    - Adjusted tree distribution
    - Tall trees are slightly taller
    - Big trees have a different shape
- Rainforest
    - Added underground vines
    - Replaced small trees with tall swamp trees
    - Big trees have a different shape
- River
    - No longer generates as a biome
- Savanna
    - Slightly increased temperature
    - Slightly reduced humidity
- Wooded Hills
    - Climate now matches extreme hills

### World Generation
- Big trees
    - Grown trees now have the same shape as naturally generated trees
    - Reduced leaf decay by moving branch positions
- Villages
    - Now generate at surface level in superflat worlds
- Slightly changed biome distribution
- Temperate biomes are now more common
- Adjusted height of some biomes
- Biomes now use different seeds for noise values

### Structures
- Village
    - Cobblestone placed below village buildings has been changed to mossy cobblestone
    - Can spawn in more biomes

### Other
- The texture of the hunger bar has been changed to feathers when hunger is set to sprint only
- Reworked biome blending to no longer depend on world seed
- Server world seeds are no longer shared to clients
- Slightly reduced default ambient occlusion strength
- Made light slightly brighter (fixes a visual error with smooth lighting disabled)
- Reduced humidity in superflat worlds
- Torches now glow up regardless of shading style
- Pressing start and select at the same time on a controller toggles debug info
- The creative inventory can now be scrolled using the right stick on a controller

## Removals
- Deprecated the Small Biomes, Large Biomes, AMPLIFIED and Legacy world types as they can easily be recreated with the Customized world type
- Shading style removed from options in favour of more customizable style settings
- Obsolete biomes (e.g. hills variants) are no longer shown on the custom world type menu 

## Bug Fixes
- Night time is now dark with shading style set to beta
- Swamp trees can now grow above Y 128
- Screenshotting at lower resolutions no longer prevents screenshotting at larger resolutions under 3x the size of the original resolution
- Quitting settings menus now correctly saves options
- Removed the "Already decorating!" crash
- Pick block now works correctly for bookshelves and glowstone blocks
- Fixed upside-down slab lighting bug
- Exhaustion is no longer applied when taking damage with hunger type set to sprint only
- Some mobs in multiplayer are now correctly affected by the health multiplier
- Sprint cooldown for attacking mobs now works correctly in multiplayer
- Picking up experience orbs now play the same popping sound in multiplayer as it does in singleplayer

---

# 1.2.5
Released: March 17th 2024

## Additions
- Beta world type
- Controller support

## Changes

### Biomes
- Readjusted the height of forests, taigas and birch forests
- Increased the frequency of ice mountains
- Removed plains from inside of forests
- Removed birch trees from rainforests

### Gameplay
- Classic Mode
    - Cows, chickens and sheep no longer drop meat
    - Zombies drop feathers instead of rotten flesh
    - Zombie Pigmen drop cooked pork instead of pigman flesh
- Made the sprint cooldown vignette slightly darker

## Bug Fixes
- Blocks now update correctly in multiplayer
- Cursor now correctly centers onto the screen when the inventory is opened

---

# 1.2.4
Released: December 29th 2023

## Additions
- New creative mode music from modern versions

## Changes
- Hunger bar no longer jitters when empty

## Bug Fixes
- Empty chunks are no longer prone to crashing
- Blocks now break correctly at maximum chunk height

---

# 1.2.3
Released: December 28th 2023

## Changes
- Adjusted the height of forests, taigas and birch forests
- Quit game button is now always visible on the title screen

---

# 1.2.2
Released: December 26th 2023

## Changes

### Gameplay
- Hardcore
    - Items are now deleted on death

## Bug Fixes
- The bottommost layer of the world now generates correctly
- The bottommost section of the world (lowest 16 blocks) now gets sent to the client

---

# 1.2.1
Released: December 25th 2023

## Changes

### Gameplay
- Hardcore
    - Text mentions that items get deleted on death

### Biomes
- Highlands
    - Increased temperature and rainfall
- Reduced the height of a few biomes
- Screwed over the height of forests, taigas and birch forests
- Removed beaches from a few biomes

## Bug Fixes
- Blocks above Y 2048 are now saved
- Picking gravel now correctly gives the player gravel
- XP no longer appears in creative mode while sneaking
- The world creation screen and game over screen no longer suggests that hardcore mode prevents respawning

---

# 1.2
Released: December 25th 2023

## Additions

### World Generation
- Customized world type
    - Repurposed from the Single Biome world type
    - Biome size can be changed
- Legacy world type
    - Restores randomised biome distribution without climate zones

### Biomes
- Birch Forest
    - A forest filled with tall birch trees
- Extreme Hills
    - Restored from Beta 1.8
    - Slightly more tall grass
- Mega Taiga
    - Features tall spruce trees
- Mushroom Valley
    - Variant of Rainforest featuring mycelium and large mushrooms
- Seasonal Forest
    - Unused biome left in the code
    - Unable to generate even in customized worlds
    - Forest variant with less trees
- Snowcapped Hills
    - Resembles Extreme Hills from release 1.7
- Snowcapped Peaks
    - Features spiky, mountainous terrain
    - Stone mountains with grassy lowlands
    - Generates with oak and spruce trees
- Wooded Hills
    - Variant of Extreme Hills with more trees (oak and spruce)

### Settings
- Shading style
    - Beta makes all light grayscale

## Changes

### Blocks
- Grass Block
    - Reverted top texture to aa1.0
- Sapling
    - Oak saplings generate swamp trees in swamplands
- Snow Layer
    - Added to the creative inventory
- Tall Grass
    - Increased brightness
    - Reduced height

### Mobs
- Spawning
    - Animals in classic mode spawn much more frequently and are able to despawn

### World Generation
- Changed the shape of the land
- Biomes now generate within five climate zones: snowy, cool, temperate, warm and hot
- The player can spawn in any biome
- Adjusted height of several biomes
- Superflat
    - Increased temperature and humidity
- Villages
    - Generate with mossy cobblestone
    - No longer generate with villagers
- Large mushrooms now generate after trees again

### Biomes
- Beaches
    - No longer generate next to highlands
- Gravel Beach
    - Increased size and rarity
- Ice Plains, Ice Mountains and Frosty Highlands
    - No longer generates with tall grass, flowers or mushrooms
- Parched Forest
    - Renamed from Extreme Hills
- Plains
    - Reduced amount of tall grass
- Rainforest
    - Removed large mushrooms
- River
    - Increased width and decreased depth
- Savanna
    - No longer generates with tall grass or flowers
    - Now generate with spots of desert
    - Adjusted climate
- Swampland
    - Increased amount of large mushrooms
    - No longer generate with rivers embedded inside

### Gameplay
- Flying
    - Sneaking no longer slows down flying
    - The player can now sprint in any direction while flying
    - No longer affected underwater
- Hardcore
    - Respawning is now allowed

### Lighting
- Made ambient occlusion darker
- Adjusted color of block light
- Adjusted block lighting in the inventory
- Made skylight at sunrises and sunsets darker

### Settings
- Lighting fixes
    - Changed to three options:
        - Off: completely disable lighting fixes
        - Minimal: maximum of 20 lighting fixes every second
        - Maximum: fix lighting of every new chunk per tick

### Other
- Replaced all panoramas with 8 new panoramas
- The main menu panorama starts at a random rotation every time
- Positive world height limit has been removed
- Reduced spread of biome color blending
- Increased chunk updates while the game is paused
- Debug menu contains information on world height, temperature, rainfall and biome height
- Made sky color vary more between biomes

## Removals

### World Generation
- Single Biome world type
    - Removed in favor of Customized
- Hill biomes
    - Now built into regular biomes

### Biomes
- Shrubland
    - Removed from generation
- Biomes no longer have strange variants
    
## Bug Fixes
- Rendering no longer completely breaks down on old graphics drivers
- Chests are now held correctly
- More blocks are pick blocked correctly in creative mode
- Warning text for far render distance on 32 bit systems now renders correctly

---

# 1.1
Released: July 1st 2023

## Additions

### Blocks
- Wood Slab
    - Not made out of stone
    - Comes in the four wood varieties
- Wood Stairs
    - Other wood variations added
- Fence
    - Other wood variations added
- Nether Brick Slab
- Sandstone Stairs

### World Generation
- Amplified world type
    - Tall terrain generates up to the top of the world
- Small Biomes world type
    - Biomes are half the size
- Single Biome world type
    - Generate a single biome of the player's choice
    - Oceans, ocean biomes, beaches, rivers and hills can be turned on or off
    - Amplified world generation can be turned on
    - Strange biomes do not generate
- Strange Biomes
    - Some biomes have "strange" variants that have a 1 in 3 chance of replacing that biome
    - Added strange variants for Jungle, Extreme Hills, Plains and Swampland

### Biomes
- Rainforest
    - Strange variant of the Jungle biome
    - Like the pre-Beta 1.8 biome of the same name
- Taiga
    - A variant of the Snowy Taiga without snow
- Frozen Beach
    - A beach with snow and ice
- Frosty Highlands
    - Snowy variant of the Highlands
- Frosty Highlands Edge
    - Snowy variant of Highlands Edge
- Gravel Beach
    - Variant of the Beach with gravel
- Windswept Crags
    - Strange variant of the Extreme Hills biome
    - Reminiscent of the pre-Authentic Adventure Extreme Hills biome
    - Very tall hills featuring crags
- Shrubland
    - Strange variant of the Swampland biome
    - Features many shrubs
- Savanna
    - Strange variant of the Plains biome
    - Features dry grass and tall plateaus

## Changes

### Blocks
- Textures
    - Reverted some texture changes
    - Grass texture changed to hybrid between beta and release
    - Ore and end stone textures have been updated
- Soul Sand
    - Prevents swimming
- Stairs
    - Added corner stairs
- End Portal Frame
    - Now available in the creative menu
- Mushroom Blocks
    - Now available in the creative menu
    - Player placed blocks have proper textures
- Water
    - Tinted based on the current biome
    - Colored water can be disabled in the settings
- Leaves
    - Increased decay radius
- Fence
    - Recipe changed from 6 sticks to 4 planks and 2 sticks
    - Crafting fences now gives 3 at a time instead of 2
- Button
    - Now only requires 1 stone to craft instead of 2

### Items
- Realigned a few textures
- Food
    - Stack size increased from 16 to 64
    - All raw meat and fish now have a 50% chance to give 20 seconds of Hunger II
    - Updated meat textures
- Rotten Flesh
    - Chance of poison increased from 80% to 100%
- Pigman Flesh
    - Heal amount increased from 4 to 6
    - No longer grants poison
    - Now has a 100% chance to give 20 seconds of Hunger III
- Mushroom Stew
    - Stack limit increased to to 4
- Boat
    - No longer breaks on collision
    - Now drops itself when attacked
- Bottle o' Enchanting
    - No longer drops experience orbs in classic mode
- Fermented Spider Eye
    - Changed texture

### Mobs
- Snow Golem
    - Can now place snow at higher temperatures

### Gameplay
- Items can now be dropped as a stack while holding left control
- Experience
    - Picking up experience orbs now plays a plop sound
    - Levelling up now plays a ding sound 
    - Enchanting is now properly scaled with the 30 level cap
- Sprinting
    - Left Control can now be used for sprinting
    - Disabled when attacking mobs and getting hurt
    - Cooldown is scaled with difficulty
- Spawn Location
    - Can be in any biome in hardcore mode
- Creative Mode
    - A few blocks are no longer pickable
    - Mobs can now be picked as spawn eggs
    - Shift clicking items in the hotbar now quickly deletes them
    - Pressing F4 toggles no-clip
- Classic Mode
    - Getting hurt now plays the old oof sound
    - Damage caused by the player deals 1 extra damage

### Lighting
- Adjusted color of block light
- Block light no longer flickers
- Sky light at night slightly adjusted
- Light now comes sooner at sunrise, so new worlds start bright

### World Generation
- Changed shape to be more like 1.7-1.17 world generation with smaller oceans
- Adjusted height and climate values of some biomes
- Mushroom Islands and Ice Plains generate again
- Hill biomes are less common (reduced chance of spawning from 2/3 to 1/2)
- Reduced ore generation in Hardcore mode by 25%
- Gravel now generates under water
- Terrain can now generate up to 256 blocks
- Large mushrooms
    - Removed from most biomes
    - Now generate before trees

### Biomes
- Highlands
    - Reduced temperature and rainfall
- Snowy Taiga
    - Renamed from Taiga
- Jungle
    - Vines now generate underground
- Extreme Hills
    - Increased large mushrooms
- Swampland
    - Increased large mushrooms
- Plains
    - Reduced trees
- Beach
    - Made larger
- Desert
    - No longer generates lakes
- Mushroom Island
- Mushroom Island Shore
- Ice Plains
- Ice Mountains
- Frozen Ocean
    - Can generate in worlds again

### Structures
- Strongholds
    - No longer generates in ocean biomes
    - A few more rooms no longer generate above ground

### Settings
- Reworked biome blending
    - Biome colors now spread much further between biomes
    - Removed the biome blending slider
- Reworked fast lighting
    - Fast lighting is now a slider called "Light Fix Speed"
    - Default value is 10%
    - 0% is fast lighting off, 100% is fancy lighting on
    - Percentage determines how much light population occurs every tick
- Added an option for colored water

### Other
- End Poem & Credits
    - Holding down space speeds up the credits
    - Added the Authentic Adventure subtitle to the logo
    - Added BlueStaggo to the credits
- Main Menu
    - Replaced all panoramas and added an additional 2 panoramas
    - Holding down left shift speeds up the panorama animation
    - Pressing P cycles through panoramas
    - Removed Authentic Adventure splashes
- Autosaving occurs every minute instead of every two seconds
- Chunks are now updated in a spiral pattern
- Fixed world conversion to Anvil
- The world seed is now shown on servers

## Bug Fixes
- Strongholds no longer generate in oceans
- Experience level is no longer shown when sneaking in classic mode
- Armor and air bars are now shown in their old positions in classic mode
- Big trees now always have height variation
- Crags now turn grass below them into dirt
- Block breaking delay removed from servers

---

# 1.0.1
Released: May 19th 2023

## Additions
- Large Biomes world type

## Changes

### Items
- Food
    - Changed stack size from 64 to 16
- Rotten Flesh and Pigman Flesh
    - Now grants poison instead of hunger
- Bottle o' Enchanting
    - Dropped experience no longer scales with difficulty

### Mobs
- Cow
    - Reduced Raw Beef drops from 1-3 to 0-2
- Chicken
    - Reduced Raw Chicken drops from 1-3 to 0-2

### Biomes
- Plains
    - Reduced large mushrooms

### Settings
- Fancy lighting has been renamed to fast lighting and its effect is inversed

## Bug Fixes
- Slimes, Magma Cubes and Blazes no longer move very fast in mid air
- Slimes have +50% health on hardcore mode instead of classic mode

---

# 1.0
Released: May 17th 2023

## Additions

### Items
- Raw and Cooked Mutton
- Pigman Flesh

### Enchantments
- Stamina
    - Maximum level: III
    - Applies to leggings
    - Reduces exhaustion by 10% for each level
    - Cannot be used with Velocity
- Velocity
    - Maximum level: III
    - Applies to leggings
    - Increases walking speed by 8% for each level
    - Cannot be used with Stamina

### Biomes
- Highlands
    - Tall biome with oak and spruce trees
- Highlands Edge
    - Lower variant of the highlands
- Sea Crags
    - An ocean biome with stone spikes
- Archipelago
    - An ocean biome consisting of islands with jungle trees

### Gamemodes
- Classic
    - Brings back old health mechanics
    - Food does not stack
    - Increased sword damage
    - Disabled critical hits
    - Disabled sprinting
    - Disabled experience and enchanting

### Splashes
- Also try:
    - NSSS
    - Better than Adventure
    - New Frontier Craft
    - Mango Pack
    - Back in Time
    - Classicube
    - Betacraft
    - Adventure+
    - Minecraft Diverge
        - Another Minecraft mod made by BlueStaggo
- Real Minecrafters never eat!
    - References Minecraft Youtuber Grian ("Real Minecrafters age their copper like this!") as well as hunger mechanics before Beta 1.8 (eating was not required to survive)
- Famine simulator!
- Actually features adventure!
- Careful? Where's the fun in that?
    - Quote from Sonic the Hedgehog in Sonic Frontiers

### Settings
- Biome blend distance can now be changed and is set to 5x5 by default
- Turning off fancy lighting disables the "populate lighting" step in the new lighting engine

## Changes

### Blocks
- Textures
    - Reverted texture changes from 1.0
    - New cobblestone texture
    - Inventory lighting changed to look like Beta 1.8
- Enchantment Table
    - Maximum level decreased from 50 to 30 outside hardcore mode
- Stairs
    - Crafting recipes yield 8 stairs instead of 4
- Ladder
    - Crafting yields 3 ladders instead of 2

### Items
- Textures
    - Realigned some textures
    - Charcoal now has a unique texture
- Food
    - Takes longer to eat
    - Eaten instantly in classic mode
    - Unstackable in classic mode

### Gameplay
- Hunger
    - Only decreases with sprinting
    - Disabled in hardcore mode and classic mode
- Exhaustion
    - Exhaustion added from sprinting increased from 0.1 per metre to 0.2
    - Exhaustion added from sprint jumping increased from 0.8 to 1.0
    - Halved in easy mode, doubled in hard mode
    - Removed saturation
- Health
    - No longer regenerated from hunger
    - Now directly healed by food
- Sprinting
    - Disabled in hardcore mode and classic mode
- Experience
    - Adjusted level requirements to post-1.3 levels
    - Sneaking now shows the exact XP value and level requirement
- Hardcore Mode
    - Monsters now have 50% more health
    - Doubled experience drops
- Creative Mode
    - Added access to the survival inventory to creative menu
    - Pick block now picks the exact same block
    - Sprinting while flying is now faster

### World Generation
- Ocean distribution slightly adjusted
- Many biomes had their height and temperature adjusted
- Large mushrooms now generate occasionally in some biomes

### Biomes
- Plains
    - Now generates with more trees 
- Swampland
    - No longer has dark grass and foliage
- Extreme Hills
    - Now generates with trees

### Structures
- Stronghold
    - Generates much more frequently
    - Now generates above ground in any biome
    - Added spawners to the prison and library rooms
    - The End portal only generates with a 20% chance

### Lighting
- Backported the release 1.8 lighting engine
- Block light has been desaturated

### Main Menu
- Four panoramas are chosen at random
- Added an "Authentic Adventure" subtitle to the logo

### Other
- The pie chart and lagometer are now only shown when the player presses F3 while sneaking
- Speed effects now work properly in mid air
- Removed the 5 tick delay between mining blocks

## Removals

### Biomes
- Mushroom Island
- Mushroom Shore
- Ice Plains
- Ice Mountains
- Frozen Ocean
    - These biomes are still in the code, but they do not generate naturally

## Bugs
- Slimes, Magma Cubes and Blazes move very fast in mid air
