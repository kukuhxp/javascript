# ARRAY

## Empty Array Declaration

**Syntax:**

```
let variable = [ ]
let variable = new Array(length);
```

## Filled Array Declaration

**Syntax:**

```
const variable = [item, item n]
const variable = Array.of(item, item n);
const variable = new Array(item, item n);
// Copying array item with spread operator
let variable1 = [1, 2]
let variable2 = [...variable1, 3, 4]
// Creating an array from string object
const variable = Array.from("string");
// Creating an array with default items
const arr = Array(5).fill(0);
```

## Array Destructuriing

**Syntax:**

```
variable = ["Item 1", "Item 2"]
variable[variable 1, variable 2] = data;
```

## Prototype Object

**Syntax:**

`Array.prototype`

# INSTANCE METHODS

## copyWithin()

**Syntax:**

array.copyWithin(target, start, end)

**Parameters:**

- target: the position of copied index is placed
 
- start (optional): the start of copied part, the default is 0

- ended (optional): the end of copied part, the default is array length


## flatMap()

**Syntax:**

array.flatMap(callback(currentValue[, index[, array]])[, thisArg])
   