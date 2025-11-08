# STRING TYPES

## String Literal

```
variable = "Let's begin!";
variable = 'He say "thank you"`;
```

## Template Literal

Template literal mendukung fitur multiple-line, sehingga kita dapat membuat string yang diikuti oleh garis baru.


```
variable = `I'm going to workplace,
but I need to buy a food first`
```

## Interpolation

```
let a = 50000;
let b = 50000;
let str = `My balance is = ${a + b}` // My balance is 100000
```

## HTML Literal

`document.body.innerHTML = "<p>JavaScript</p>";`

## Char Literal

```
variable = "JavaScript";
variable[0]
```

## String Concatenation

```
"a" + 7 = a7

a = 2;
b = "buy";
c = a.concat(b);
```

## Falsy String

`variable = "";`

## String Static Methods

### raw()

- Parameters: Strings, Sub N
- Return Value: String

## String Instance Properties

### constructor / String.prototype.constructor

- Status: Writable
- Value: Object


## String Instance Methods

### charAt() / String.prototype.charAt()

- Parameters: Index
- Return Type: String


### concat() / String.prototype.concat()

- Parameters: Object, String, Number
- Return Type: String


### endsWith() / String.prototype.endsWith()

- Parameters: String
- Return Type: Boolean 

### includes() / String.prototype.includes()

- Parameters: String
- Return Type: Boolean

### indexOf() / String.prototype.indexOf()

- Parameters: String
- Return Type: Number

### lastIndexOf() / String.prototype.lastIndexOf()

- Parameters: String
- Return Type: Number


### repeat() / String.prototype.repeat()

- Parameters: Numbers
- Return Type: String


### replace() / String.prototype.replace()

- Parameters: Old String/RegEx, New String
- Return Type: String
- Example:
   ```
   /*
    To avoid case sensitive of replace() method,
    you use the RegExp flag.
   */  
   string.replace("Some", "Replaced");
   
   // Using the insensitive flag of RegExp
   string.replace(/SOME/i, "Replaced");
   
   // Using the global match flag of RegExp
   string.replace(/some/g, "Replaced");
   ```

### search() / String.prototype.search()

- Parameters: Regex
- Return Type: Numbers

### slice() / String.prototype.slice()

- Parameters: Start, End
- Return Type: String

### split() / String.prototype.split()

- Parameters: Separator/Whitespace, Limit
- Return Type: Array of Strings

### startsWith() / String.prototype.startsWith()

- Parameters: String
- Return Type: Boolean 

### substring() / String.prototype.substring()

- Parameters: Start, End
- Return Type: String
- Example:
   ```
   /*
   If the one of index is negative, the index becomes zero (0)
   If the end index is negative, it swapped to start index
   */
   string.substring(-5, 3);
   
   /*
   If the start index > end index,
   the string is reversed. (3, -5) equivalent to (0, 3)
   */
   string.substring(3, -5);
   ```

### toLowerCase() / String.prototype.toLowerCase()

- Parameters: None
- Return Type: String

### toString() / String.prototype.toString()

- Parameters: None
- Return Type: String

### toUpperCase() / String.prototype.toUpperCase()

- Parameters: None
- Return Type: String

### trim() / String.prototype.trim

- Parameters: None
- Return Type: String