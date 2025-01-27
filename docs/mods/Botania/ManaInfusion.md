::requiredMod[Botania]{builtIn=true modLink=https://www.curseforge.com/minecraft/mc-mods/botania}

# Botania Mana Infusion

Mana Infusion is a type of [IRecipeManager](/vanilla/api/managers/IRecipeManager) and implements all the methods that are available to IRecipeManager's, such as `removeRecipe()` and `removeAll()`.

## Methods

#### Add Recipe

The following script will add two Mana Infusion recipes, the recipes will do the following:

1) When an Enchanted Golden Apple is given to a Mana Pool, a piece of Dirt will be given back.
2) When an Apple is given to a Mana Pool with a Diamond Block beneath it, a Diamond will be given back.

```zenscript
// <recipetype:botania:mana_infusion>.addRecipe(name as string, output as IItemStack, input as IIngredient, mana as int, catalystState as @Optional BlockState)

<recipetype:botania:mana_infusion>.addRecipe("mana_infusion_test", <item:minecraft:dirt>, <item:minecraft:enchanted_golden_apple>, 200);
<recipetype:botania:mana_infusion>.addRecipe("mana_infusion_test_catalyst", <item:minecraft:diamond>, <item:minecraft:apple>, 200, <blockstate:minecraft:diamond_block>);
```

#### Remove Recipes

The following script will remove all Mana Infusion recipes that output an Apple

```zenscript
// <recipetype:botania:mana_infusion>.removeRecipe(output as IItemStack);

<recipetype:botania:mana_infusion>.removeRecipe(<item:minecraft:apple>);
```
