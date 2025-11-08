# EVENT INTERFACE
 
## CustomEvent Constructor
 
- CustomEvent()

## Event Object

**Syntax:**

```
function functionName(e) {
 e.property, e.method;
}
```

# CONSTRUCTOR

## Event()

**Syntax:** `variable = new Event()`
 
# INSTANCE PROPERTIES

## type

**Status:** Read-only

**Value:** String

**Syntax:** Event.type

## target

**Status:** Read-only

**Value:** String

**Syntax:** Event.target

## currentTarget

**Status:** Read-only

**Value:** String

**Syntax:** Event.currenTarget

## key

## code

## clientX

## clientY

# INSTANCE METHODS

## preventDefault()

## stopPropagation()

## Callback Queue

Callback queue adalah bagian dari mekanisme event loop dalam JavaScript yang menyimpan fungsi-fungsi yang siap dijalankan setelah stack utama kosong.