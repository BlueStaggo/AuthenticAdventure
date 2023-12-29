# 1.2.4
Released: December 29th 2023

## Additions
- New creative mode music from modern versions

## Changes
- Hunger bar no longer jitters when empty

## Bug Fixes
- Empty chunks are no longer prone to crashing
- Blocks now break correctly at maximum chunk height

# 1.2.3
Released: December 28th 2023

## Changes
- Adjusted the height of forests, taigas and birch forests
- Quit game button is now always visible on the title screen

# 1.2.2
Released: December 26th 2023

## Changes

### Gameplay
- Hardcore
    - Items are now deleted on death

## Bug Fixes
- The bottommost layer of the world now generates correctly
- The bottommost section of the world (lowest 16 blocks) now gets sent to the client

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
    - Animals spawn much more frequently and despawn in classic mode

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
- More blocks are pick blcoked correctly in creative mode
- Warning text for far render distance on 32 bit systems now renders correctly

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

- Stamina
    - Maximum level: III
    - Applies to leggings
    - Increases walking speed by 8% for each level
    - Cannot be used with Velocity

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
