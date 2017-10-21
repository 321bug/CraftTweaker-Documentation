
# Part

A Part is the form an item is in, for example a gear or an ore.

## Importing the package
It might be required for you to import the package if you encounter any issues, so better be safe than sorry and add the import.  
`import mods.contenttweaker.Part;` 

## Retrieving such an object
You can either retrieve an existing Part using the [MaterialSystem](/Mods/ContentTweaker/Materials/MaterialSystem) or create an entirely new one using the [Part Builder](/Mods/ContentTweaker/Materials/Parts/Part_Builder)


<details>
	<summary>Following types are pre-registered (Headlines are the [Part Types](PartType)):</summary>
	<h4>Items:</h4>
		<ul>
			<li>Beam ![beam icon](assets/beam.png)</li>
			<li>Bolt ![Bolt icon](assets/Bolt.png)</li>
			<li>Casing ![Casing icon](assets/Casing.png)</li>
			<li>Crystal ![Crystal icon](assets/Crystal.png)</li>
			<li>Dense Plate ![Dense Plate icon](assets/dense_plate.png)</li>
			<li>Dust ![Dust icon](assets/Dust.png)</li>
			<li>Gear ![Gear icon](assets/Gear.png)</li>
			<li>Ingot ![Ingot icon](assets/Ingot.png)</li>
			<li>Nugget ![Nugget icon](assets/Nugget.png)</li>
			<li>Plate ![Plate icon](assets/Plate.png)</li>
			<li>Rod ![Rod icon](assets/Rod.png)</li>
		</ul>
	<h4>Blocks:</h4>
		<ul>
			<li>Block</li>
		</ul>
	<h4>Ores:</h4>
		<ul>
			<li>Ore</li>
			<li>Dense Ore</li>
			<li>Poor Ore</li>
		</ul>
	<h4>Fluids:</h4>
		<ul>
			<li>Molten</li>
		</ul>	
	<h4>Armor:</h4>
		<ul>
			<li>Armor ![Helmet Icon](assets/armor_head.png)![Chest Plate Icon](assets/armor_chest.png)![Leggins Icon](assets/armor_legs.png)![Boots Icon](assets/armor_feet.png)</li>
		</ul>
</details>

## Fields
You can retrieve the following information from a Part:

| ZenMethod            | Return Type                            |
|----------------------|----------------------------------------|
| getName()            | String                                 |
| getUnlocalizedName() | String                                 |
| getPartType()        | [IPartType](IPartType)                 |
| getPartTypeName()    | String                                 |
| getOreDictPrefix()   | String                                 |
| getData()            | List<[IPartDataPiece](PartDataPiece)>  |

## Register to Material(s)
You can use this to register one or several Materials to this part
```
part.registerToMaterial(Material material);
part.registerToMaterials(Material[] materials);
```

The function will either return a single [MaterialPart](/Mods/ContentTweaker/Materials/Materials/MaterialPart) object or a List of them, depending on whether you registered one or multiple materials at once.