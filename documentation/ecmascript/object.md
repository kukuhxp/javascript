# JAVASCRIPT OBJECTS

## 1. Built-in Objects

Ini adalah objek dasar yang sudah disediakan langsung oleh JavaScript, tidak tergantung browser.

Contoh:

- Object dasar: `Object, Function, Boolean, Symbol.`
- Number & Math: `Number, BigInt, Math.`
- String: `String>`
- Date & Time: `Date.`
- Error: `Error, TypeError, SyntaxError.`
- Collections: `Array, Set, Map, WeakSet, WeakMap.`
- Typed Arrays: `Int8Array, Float32Array.`
- JSON & RegExp: `JSON, RegExp.`

## 2. DOM Objects

Objek yang hanya ada di browser, digunakan untuk berinteraksi dengan halaman web.

Contoh:

- Global: `window.`
- Document Node: `document.`
- Element Node: `Element Node.`
- Collection: `HTMLCollection, NodeList.`
- Event: `Event, MouseEvent, KeyboardEvent.`
- Communication: `FormData, XMLHttpRequest, fetch.`
- Web Storage: `localStorage, sessionStorage.`

## 3. Web API Objects

Disediakan oleh browser modern sebagai bagian dari Web API.
   
Contoh:

- Geolocation API: `navigator.geolocation.`
- Canvas API `CanvasRenderingContext2D.`
- Web Audio API: `AudioContext, OscillatorNode.`
- Fetch API: `Request, Response, Headers.`
- File API: `File, FileList, Blob£.`
- WebSocket: `WebSocket.`
- Service Worker: `ServiceWorker, Cache.`

## 4. Object Literal

### Object Declaration

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

### Assigning The Key Value

```
// user is object
const user = {};

// name is key
// "Mazzy" is value
user.name = "Mazzy";
```

### Using The Object's Key

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

### This Keyword

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

### Object Index

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

### Nested Property

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

### Object Destructuring

## 5. Constructor Function

Membuat objek melalui constructor function.

`let object = new Object(value);`

## 6. Instance Class

Kamu juga bisa membuat tipe objek sendiri menggunakan class atau constructor function.

Contoh:

```
class Robot {
  constructor(name) {
    this.name = name;
  }
  greet() {
    console.log(`Halo, aku ${this.name}`);
  }
}

const r1 = new Robot("Astra");
r1.greet(); // "Halo, aku Astra"
```