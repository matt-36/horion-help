# NBT

## What is NBT?

NBT, or Named Binary Tag, is the data of a block or item that is changable using inventory editors, like Horion and MCEdit. A different way of explaining it is to say it is how minecraft stores item/block data. Using Horion, you need to copy text from either a message or a file downloaded from online containing the correct Horion NBT format.

## How do you identify an NBT type

First, lets explain what I mean by "NBT type". There are `.nbt load` and `.nbt write` NBTs. `.nbt load` NBTs are NBTs that create an item, which is specified in the text, and replace the current slot with it. `.nbt write` NBTs do NOT create an item, and simply overwrite the tags, like enchantments and names, of the item being held. This means that doing both `.nbt write` and `.nbt load` on the same nbt is useless, and will replace the first item with the second item anyways.
A simple example of the different nbt types are below

- `.nbt load` 
```
{Count:64b,Name:"wooden_sword",tag:{Unbreakable:1b}}
``` 

or 

- `.give wooden_sword 1`+`.nbt write` 
- `.give wooden_sword 1 0 1` (the 1 means the same as `.nbt write`)
```
{Unbreakable:1b}
```

The difference between how you can use these NBTs is kinda big. For `.nbt load`, you only get the wooden sword with the unbreakable tag, and thats it. Although, with `.nbt write`, you can give yourself any breakable item, do `.nbt write`, and then it will be indestructable. So, as a recap, an NBT that starts with a tag, like `{ench:[` is a `.nbt write` NBT, and an NBT that starts with an item, like `{Count:1b,Name:"` or `{{Items:[` (notice the extra bracket) is a `.nbt load` NBT.

## NBT tags
