# Random

## 导入相关包

It might be required for you to import the package if you encounter any issues (like casting an Array), so better be safe than sorry and add the import at the very top of the file.
```zenscript
import crafttweaker.api.util.Random;
```


## 方法

### getRandomUUID

Return Type: string

```zenscript
Random.getRandomUUID() as string
myRandom.getRandomUUID();
```

### nextBoolean

Return Type: boolean

```zenscript
Random.nextBoolean() as boolean
myRandom.nextBoolean();
```

### nextDouble

Returns the next pseudorandom, uniformly distributed double value between 0.0 and 1.0 from this random number generator's sequence.

Return Type: double

```zenscript
Random.nextDouble() as double
myRandom.nextDouble();
```

Returns the next pseudorandom double. Its range is [min, max]

Return Type: double

```zenscript
Random.nextDouble(min as double, max as double) as double
```

| 参数  | 类型     | 描述                      |
| --- | ------ | ----------------------- |
| min | double | No Description Provided |
| max | double | No Description Provided |


### nextFloat

Returns the next pseudorandom, uniformly distributed float value between 0.0f and 1.0f from this random number generator's sequence.

Return Type: float

```zenscript
Random.nextFloat() as float
myRandom.nextFloat();
```

Returns the next pseudorandom float. Its range is [min, max]

Return Type: float

```zenscript
Random.nextFloat(min as float, max as float) as float
```

| 参数  | 类型    | 描述                      |
| --- | ----- | ----------------------- |
| min | float | No Description Provided |
| max | float | No Description Provided |


### nextInt

Returns the next pseudorandom, uniformly distributed int value from this random number generator's sequence.

Return Type: int

```zenscript
Random.nextInt() as int
myRandom.nextInt();
```

Returns the next pseudorandom, uniformly distributed int value between zero (inclusive) and bound (exclusive) from this random number generator's sequence

Return Type: int

```zenscript
Random.nextInt(bound as int) as int
```

| 参数    | 类型  | 描述                                             |
| ----- | --- | ---------------------------------------------- |
| bound | int | the upper bound (exclusive). Must be positive. |


Returns the next pseudorandom int. Its range is [min, max]

Return Type: int

```zenscript
Random.nextInt(min as int, max as int) as int
```

| 参数  | 类型  | 描述                      |
| --- | --- | ----------------------- |
| min | int | No Description Provided |
| max | int | No Description Provided |


