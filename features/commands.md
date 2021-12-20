# Commands

`{option/option}` choose one of the listed options

`<replace>` replace the text with what it says

`{option-1/option-2} <replace(option-1)>` the replacable text only works with the listed option or the text in the paranthesis are a note
  
- .help
  - Lists all commands in the chat
  - Usage
    - `.help`
    - `.help <module name>`

- .path
  - Toggles the path module and walks towards a specified destination
  - Usage
    - `.path {y/xz/xyz} <coordinates>`
    - Y
      - Creates a path to the Y coordinate you listed
    - XZ
      - Creates a path to the X and Z coordinates you listed
    - XYZ
      - Creates a path to the X, Y, and Z coordinates you listed
  
- .nbt
  - Changes Item data of an item in the active inventory slot
  - You have to copy the nbt from a text file you downloaded or typed, then use the corresponding command. Ask the creator or someone who knows the nbt what the command is if you don't know
  - If you get an error when trying to use this command, check the [issues page](issues.md)
  - Usage
    - `.nbt {load/write/save/read}`
    - Load
      - Replaces anything in the active slot with the block listed in the nbt you copied if it was designed to be .nbt load
    - Write
      - Replaces the enchantments, occupants, and other data tags of the item being held if the nbt you copied was designed to be .nbt write
      - Can get the same effect with `.give <item> <amount> <tile id> 1` where the 1 means .nbt write
    - Save
      - Copies the nbt data of the item being held
    - Read
      - Copies the nbt data of an entity you are looking at while in a local or private world

- .toggle
  - Toggles a module without using the ClickGui
  - Usage
    - `.toggle <module name>`
  
- .bind
  - Connects a selected key and module together for quick and easy access
  - If you can't figure out the name of the key or module, [ask in the discord server](https://discord.gg/horion)
  - Usage
    - `.bind <module name> <key>`
  
- .unbind
  - Disconnects a module from its keybind for less accidental activation
  - If you can't figure out the name of the key or module, [ask in the discord server](https://discord.gg/horion)
  - If you accidentally unbind a module or did `.unbind all force` and don't know how to rebind it, see above
  - Usage
    - `.unbind <module name>`
    - `.unbind all force`
  
- .teleport
  - Teleports you to specific coords you input
  - Usage
    - `.teleport <coords>`
  
- .relativeteleport
  - Teleports you to a relative location with the specified coords you input
  - Usage
    - `.relativeteleport <relative coords>`

- .playertp (broken)
  - Teleports you to a player within your render distance
  - Usage
    - `.playertp <username>`

- .namespoof
  - Visually changes your name for everyone in the game
  - After doing the command, you have to leave the world and rejoin
  - Name does not reset back to normal when leaving and rejoining or switching to a different world, realm, or server
  - Usage
    - `.namespoof {name/reset} <name(name)>`
  
- .cbe
  - Gives a block that will spawn a command block minecart, sometimes invisible, that will execute a command repeatedly while command blocks are enabled
  - Usage
    - `.cbe {beehive/beenest/movingblock/invisible/spoof} <command>`

- .eject
  - Removes horion from your minecraft game
  - Usage
    - `.eject`

- .gamemode (broken)
  - Changes your gamemode
  - Usage
    - `.gamemode {0/1/2}`

- .friend (broken)
  - Friends users so you don't hurt them
  - has a module to do it as well, midclick
  - Usage
    - `.friend <username>`

- .enchant
  - Enchants an item that you are holding, can do any enchantment on any item and any level from 1 to 32767
  - Usage
    - `.enchant <enchantment name> <level>`

- .panic
  - Disables all modules
  - Usage
    - `.panic`

- .hide
  - Hides horion but doesn't disable anything or eject
  - Usage
    - `.hide`

- .give
  - Gives you any item you want using the namespace or decimal id
  - Usage
    - `.give <namespace id/decimal id> <amount> <tile id> <1(.nbt write)/0(nothing)>`

- .bruh
  - Sends a local message, or a message only visible to you, saying "bruh"
  - Usage
    - `.bruh`

- .server
  - Gives you information about a server or realm you are currently on, for example, the ip and port
  - Usage
    - `.server`

- .setoffhand
  - Sets the item you are holding to your offhand instead of a totem of undying or shield
  - Usage
    - `.setoffhand`

- .coords
  - Says your coords in the chat as a local message, or a message only visible to you
  - Usage
    - `.coords`

- .say
  - Sends a message in the chat
  - Usage
    - `.say`

- .spammer
  - Allows you to set up the spammer module
  - Usage
    - `.spammer {message/delay/bypass/manual} <message(message)/delay(delay)> {true/false}(bypass)`

- .dupe
  - Duplicates the item you are currently holding
  - Usage
    - `.dupe`

- .damage (broken)
  - Damages you using fall damage
  - Usage
    - `.damage <amount>`

- .config
  - Allows you to save your current active modules and settings
  - Usage
    - `.config {save/load/new} <name>`
    - `.config save`

- .setprefix
  - Changes the command prefix for horion
  - / is disabled
  - Usage
    - `.setprefix <key>`

- .waypoint
  - Allows you to create waypoints for remembering locations
  - Only shows waypoints when the waypoint module is active
  - Usage
    - ## `.waypoint (((((Unknown)))))` 

- .top
  - Teleports you to the top of any area, useful underwater or in the nether
  - Usage
    - `.top`

- .xp
  - Gives you xp points and levels
  - Usage
    - `.xp <amount>`
    - `.xp <amount>L`

- .modules
  - Lists all modules
  - Usage
    - `.modules`
- .rename
  - Rename's your item in hand
  - Usage
    - `.rename <name>`
- .repair
  - Repair's your item in hand
  - Usage
    - `.repair`
