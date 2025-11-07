# FUNCTION

## Function Declaration

Function adalah sebuah object yang dapat menjalankan beberapa baris perintah. Function terdiri dari name, parameter dan body.

**Syntax:**

```
function functionName(parameter, parameter n) {
  functionBody
}
```

## Function Expression

Function expression adalah sebuah fungsi yang dideklarasikan di dalam sebuah variabel.

**Syntax:**

```
variable = function (parameter, parameter n) {
 statements;
}
```

## Named Function Expression (NFE)

Named function expression (NFE) adalah sebuah ekspresi fungsi yang memiliki nama.

**Syntax:**

```
variable = function functionName (parameter, parameter n) {
 statements;
}
```

## Invocation

Invocation adalah cara memanggil sebuah fungsi.

**Syntax:**

```
// Declaration
variable = function (parameter, parameter n) {
 statements;
}
// Invocation
variable();
```

**Syntax:**

```
function functionName(parameter, parameter n) {
 statements;
}
variable = functionName();
variable();
```

## Arrow Function

Arrow function adalah sebuah deklarasi fungsi terbaru dari ES6.

**Syntax:**

```
variable = (parameter, parameter n) => {
 statements;
}
```

**Syntax:**

`variable = parameter => statement:`

## Function Constructor

Function constructor sebuah fungsi yang dideklarasikan melalui constructor.

`variable = new Function(args, return);`

## Generator Function

Generator function adalah sebuah fungsi yang dapat menghentikan eksekusinya sementara dan melanjutkannya kembali.

**Syntax:**

```
function* nameFunction(parameter, parameter n) {
  yield value;
}

// Generator object
variable = nameFunction();

// next() is instance method
object.next();
```

## Immediately Invoked Function Expression (IIFE)

Immediately invoked function expression (IIFE) adalah sebuah fungsi yang langsung dijalankan setelah didefinisikan. Variabel di dalam IIFE bersifat lexical atau local.

**Syntax:**

```
(function(parameter, parameter n) {
  statements;
})();
```
**Syntax:**

```
((parameter, parameter n) => {
  statements;
})()
```

## Callback

Callback adalah sebuah function yang dikirim melalui argumen function atau method.

**Named Callback Syntax:**

 ```
// Function declaration 1
function functionName (parameter, callbackName) {
 callbackName();
}

// Function declaration 2 (Callback)
function functionName (parameter) {
 statements;
}

// Invocation
functionName(args, callbackName);

```

**Anonymous Callback Syntax**:

```
// Function declaration
function functionName (parameter, callbackName) {
 callbackName();
}

// Invocation
functionName(args, function (e) {
 statements;
});
```

## Closure

Closure adalah sebuah konsep di mana fungsi dapat mengakses scope bagian luar fungsi.

## Anonymous

Anonymous adalah istilah yang merujuk kepada function yang tidak memiliki nama.

## Asynchronous

Asynchronous adalah proses menjalankan program dibalik layar tanpa menghentikan eksekusi program utama.

# PARAMETERS

## General Parameter

General parameter adalah parameter yang umum digunakan saat mendeklarasikan sebuah fungsi. Perlu diingat bahwa pengiriman argumen ke parameter adalah berurutan. Jadi, jika kita mengirim argumen pertama ke sebuah fungsi, maka paramater yang akan menerima adalah parameter yang pertama.

## Optional Parameter

## Default Parameter

## Rest Parameter

## Object Parameter

## Array Parameter

## Callback Function