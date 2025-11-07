# OBJECT LITERAL

## Declaration

**Empty Object:**

`variable = {}`

**Assigned Object:**

```
variable = {
  // Property
  key: value,
  // Method
  key: function() {
    statements;
  }
}
```

**Object via Constructor:**

`variable = new Object(value);`

## Assigning The Key Value

```
const user = {};
// User is object, name is key and "Mazzy" is value
user.name = "Mazzy";
```

## Using The Object

```
variable = {
  key: value,
  key: function () {
    statements;
  }
}
variable = object.property;
variable = object.method();
function(object.key);
function(object.method());
```

## This Keyword

Operator this pada object merupakan cara mengakses property atau method milik object. Penggunaan this harus berada di dalam object.

```
variable = {
  key: value,
  key: function() {
    this.key;
  }
}
```

## Object Index

```
variable= {
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
variable = {
  key: key {
    key: function() {
      statements;
    }
  }
}
function(object.object.method());
```

## Object Destructuring