# OBJECT LITERAL

## Object Declaration

```
// Empty Object
let object = {}

// Assigned Object
let obj = {
  // Property
  key: value,
  
  // Method
  key: function() {
    statements;
  }
}
```

## Assigning The Key Value

```
// user is object
const user = {};

// name is key
// "Mazzy" is value
user.name = "Mazzy";
```

## Using The Object's Key

```
object = {
  key: value,
  key: function () {
    statements;
  }
}

variable = object.property;
variable = object.method();

function(object.property);
function(object.method());
```

# This Keyword

Operator this pada object merupakan cara mengakses property atau method milik object. Penggunaan this harus berada di dalam object.

Contoh:

```
let object = {
  key: value,
  key: function() {
    this.key;
  }
}
```

## Object Index

```
let object = {
  name: "John",
  country: "U.S.A",
  0: "I like it",
  1: "Disklike it"
}

variable = person["name"];
variable = person["country"];

function(person["name"]);
function(person["country"]);
```

## Nested Property

```
let object = {
  key: key {
    key: function() {
      statements;
    }
  }
}

function(object.object.method());
```

## Object Destructuring