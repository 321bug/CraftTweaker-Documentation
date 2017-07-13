# Renaming

Always reading 'chest' is annoying, isn't it?  

That's why there's the possibility to rename stuff.

## Changing the display name

This is probably the easiest way to achieve a different item or block name.
You rename `item` to `newName`:
```
item.displayName = newName;

//Example
<minecraft:chest>.displayName = "Storage Box Deluxe";
```
`item` is an IItemStack.
`newName` is a String.

## Changing the localization

If some modded inventories still show the item's old name instead of the new one, you need to change the localization.
You can read what that means on the `game` entry.
```
game.setLocalization(languageCode,unlocalizedName,newName);

game.setLocalization(tile.chest.name,"StorageBox Deluxe")
```
`languageCode` is a string and optional. If you omit it, it will apply the localization regardless of the client's set language.  
`unlocaLizedName` is a string.  
`newName` is a string.


# Tooltips

Adding a tooltip is really easy:  
All you need is an item (or oreDict or similar).

## Normal Tooltips
This adds `tT` as tooltip to `item`.
```
item.addTooltip(tT);

<minecraft:chest>.addTooltip("Storage, what can I say more?");
```
`item` is a IIngredient
`tT` is a string

## Shift Tooltips
This adds a tooltip, that will only be visible when you hold shift.
```
item.addShiftTooltip(tT);

<minecraft:chest>.addShiftTooltip("STORAGE!!!");
```
`item` is a IIngredient
`tT` is a string

# Markup
The world is colorful, and so should be all of our tooltips.
You can also nest these options, should you with to (if you wanted a green text, that is strikethrough)

## Coloring a String

You can apply one of the 16 colors to your string
```
format.black
format.darkBlue
format.darkGreen
format.darkAqua
format.darkRed
format.darkPurple
format.gold
format.gray
format.darkGray
format.blue
format.green
format.aqua
format.red
format.lightPurple
format.yellow
format.white
```

```
<minecraft:stick>.addTooltip(format.green("This one wasn't ripe"));
```

## Formatting a String
You can apply different formats to your String should you wish to:
```
format.obfuscated
format.bold
format.strikethrough
format.underline
format.italic
```

```
<minecraft:stick>.addShiftTooltip(format.strikethrough("This is a bad tooltip"));
```