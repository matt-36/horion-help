# Commands

{option/option} choose one of the listed options
<replace> replace the text with what it says

- .help
  - Lists all commands in the chat
  - Usage
    - .help
    - .help <moduel name>

- .path
  - Toggles the path module and walks towards a specified destination
  - Usage
    - .path {y/xz/xyz} <coordinates>
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
    - .nbt {load/write/save/read}
    - Load
      - Replaces anything in the active slot with the block listed in the nbt you copied if it was designed to be .nbt load
    - Write
      - Replaces the enchantments, occupants, and other data tags of the item being held if the nbt you copied was designed to be .nbt write
      - Can get the same effect with **.give <item> <amount> <tile id> 1** where the 1 means .nbt write
    - Save
      - Copies the nbt data of the item being held
    - Read
      - Copies the nbt data of an entity you are looking at while in a local or private world

- .toggle
  - Toggles a module without using the ClickGui
  - Usage
    - .toggle <module name>
  
- .bind
  - Connects a selected key and module together for quick and easy access
  - If you can't figure out the name of the key or module, [ask in the discord server](https://discord.gg/horion)
  - Usage
    - .bind <module name> <key>
  
- .unbind
  - Disconnects a module from its keybind for less accidental activation
  - If you can't figure out the name of the key or module, [ask in the discord server](https://discord.gg/horion)
  - If you accidentally unbind a module or did `.unbind all force` and don't know how to rebind it, see above
  - Usage
    - .unbind <module name>
    - .unbind all force
  
- .teleport
  - Teleports you to specific coords you input
  - Usage
    - .teleport <coords>
  
- .relativeteleport
  - Teleports you to a relative location with the specified coords you input
  - Usage
    - .relativeteleport <relative coords>

- .playertp (broken)
  - Teleports you to a player within your render distance
  - Usage
    - .playertp <username>

- .namespoof
  - Visually changes your name for everyone in the game
  - After doing the command, you have to leave the world and rejoin
  - Name does not reset back to normal when leaving and rejoining or switching to a different world, realm, or server
  - Usage
    - .namespoof {name/reset} <name>
  
- .cbe
  - Gives a block that will spawn a command block minecart, sometimes invisible, that will execute a command repeatedly while command blocks are enabled
  - Usage
    - .cbe {beehive/beenest/movingblock/invisible/spoof} <command>
