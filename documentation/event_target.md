# EVENT TARGET INTERFACE

## Event Target Objects

- Window Interface
- Document Node
- Element Node

# CONSTRUCTOR

## EventTarget()

**Syntax:** `variable = new EventTarget()`

# INSTANCE METHODS

## addEventListener()

Method yang digunakan untuk menambahkan event dan function pada element node.

## removeEventListener()

Method yang digunakan untuk menghilangkan event dan function pada element node.

## dispatchEvent()

# EVENT TARGET

## Event Expression

**Syntax:**

`element.event = function() { statements; }`

**Syntax:**
    
`element.event = functionName;`

## Event Listener

**Syntax:**
```
element.eventListener("event", function() {
 callback, statements;
});
```

**Syntax:**

```
element.eventListener("event", () => {
 callback, statements;
});
```
 
**Syntax:**

`element.eventListener("event", callback);`

## Event Bubbling

Event bubbling adalah ketika user melakukan trigger pada child element, lalu event pada parent element juga ikut tereksekusi.

`parentElement.addEventListener("event", callback);`

`childElement.addEventListener("event", callback);`


## Event Delegation

Event delegation adalah sebuah teknik yang digunakan untuk menangani seluruh event pada child element hanya dengan menggunakan event bubbling. Cukup menggunakan event listener pada parent element untuk menangani seluruh event pada child element.

**Syntax:**

```
parentElement.eventListener("click" function(e) {
  if (e.target.tagName === "child element") {
    statements;
  }
});
```

## Capture Option

Capture adalah sebuah argumen opsional yang digunakan untuk melakukan event capturing.

**Syntax:**

```
element.eventListener("event", function() {
 callback;
}, {capture: true});
```

**Syntax:**

```
element.eventListener("event", function() {
 callback;
}, true);
```

**Syntax:**

`element.EventListener("event", functionName, {capture: true});`

`element.EventListener("event", functionName, true);`

## Once Option

Once adalah sebuah argumen opsional yang digunakan untuk menjalankan function hanya satu kali pada event listener.

**Syntax:**

```
element.eventListener("event", function() {
 callback;
}, {once: true});
```
**Syntax:**

`element.eventListener("event", callback, {once:true});`

## HTML Event Attributes

HTML event attribute adalah attribute yang digunakan untuk memanggil JavaScript function di dalam dokumen HTML.

**Mouse Event:** `onclick, ondblclick`