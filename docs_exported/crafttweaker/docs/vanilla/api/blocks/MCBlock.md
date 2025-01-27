# MCBlock

## Importing the class

It might be required for you to import the package if you encounter any issues (like casting an Array), so better be safe than sorry and add the import at the very top of the file.
```zenscript
import crafttweaker.api.blocks.MCBlock;
```


## Casters

| Result type | Is Implicit |
|-------------|-------------|
| string | false |

## Methods

:::group{name=canSpawnInBlock}

Return Type: boolean

```zenscript
// MCBlock.canSpawnInBlock() as boolean

myMCBlock.canSpawnInBlock();
```

:::

:::group{name=getDefaultState}

Return Type: [MCBlockState](/vanilla/api/blocks/MCBlockState)

```zenscript
// MCBlock.getDefaultState() as MCBlockState

myMCBlock.getDefaultState();
```

:::

:::group{name=getValidStates}

Return Type: stdlib.List&lt;[MCBlockState](/vanilla/api/blocks/MCBlockState)&gt;

```zenscript
// MCBlock.getValidStates() as stdlib.List<MCBlockState>

myMCBlock.getValidStates();
```

:::


## Properties

| Name | Type | Has Getter | Has Setter | Description |
|------|------|------------|------------|-------------|
| commandString | string | true | false | No Description Provided |
| lootTable | string | true | false | No Description Provided |
| translationKey | string | true | false | No Description Provided |

