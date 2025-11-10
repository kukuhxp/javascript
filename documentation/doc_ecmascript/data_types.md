# JAVASCRIPT DATA TYPES

## Primitive Values

1. String
2. Number
3. Boolean
4. Null
5. Undefined

## Null

Null adalah nilai khusus yang menunjukkan bahwa suatu variabel dengan sengaja dikosongkan atau tidak memiliki nilai apa pun. Biasanya digunakan untuk menandai bahwa sebuah **variabel tidak berisi apa-apa secara sengaja.**

Example:

```
let data = null;

console.log(data); // null

// Null isn't 0 or ""
let a = null;
let b = 0;
let c = "";

console.log(a == null); // true
console.log(b == null); // false
console.log(c == null); // false
console.log(Boolean(a)); // false
console.log(Boolean(b)); // false
console.log(Boolean(c)); // false
```

## Bug of Null

Null is object adalah bug historis di JavaScript, seharusnya null bukan objek, tapi JavaScript sudah terlanjur mendeteksinya sejak awal hingga sekarang.

Contoh:

`typeof null; // "object"`

## Undefined

Undefined adalah nilai default yang menunjukkan bahwa sebuah variabel telah dideklarasikan tapi **belum diberi nilai secara tidak sengaja** atau sebuah properti/fungsi **tidak mengembalikan nilai**.

Contoh:

```
// Variable not filled in
let a;

console.log(a); // undefined

// Function does not return a value
function greet() {}

console.log(greet()); // undefined

// Object properties that do not exist
let obj = { name: "Alice" };

console.log(obj.age); // undefined
```

## Non-primitive Values

Secara umum, tipe objek di JavaScript bisa dibagi menjadi beberapa kategori utama:

### ECMAScript Objects

 Contoh:

- Array
- Function
- Object Literal.
- Constructor Function.
- Classes.

### Static Objects

Contoh:

- Math.
- JSON.
- RegExp.