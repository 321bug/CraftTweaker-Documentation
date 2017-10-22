# Saw

The Saw ONLY takes _Blocks_ as inputs, all IItemStack input MUST be that of a place-able _Block_.

## Addition

``` 
mods.betterwithmods.Saw.add(IItemStack[] output, IItemStack input);
mods.betterwithmods.Saw.add(IItemStack[] output, IIngredient input);
 
mods.betterwithmods.Saw.add([<minecraft:stick>,<minecraft:stick>], <minecraft:fence>);
//Only use Ingredients that contain items!
mods.betterwithmods.Saw.add([<minecraft:stick>,<minecraft:stick>], <ore:plankWood>);
```

## Removal

``` 
mods.betterwithmods.Saw.remove(IItemStack input);
 
mods.betterwithmods.Saw.remove(<minecraft:oak_plank>);
```
