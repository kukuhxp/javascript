# NULL & UNDEFINED

Null adalah nilai khusus yang menunjukkan bahwa suatu variabel dengan sengaja dikosongkan atau tidak memiliki nilai apa pun. Biasanya digunakan untuk menandai bahwa sebuah **variabel tidak berisi apa-apa secara sengaja.**

undefined adalah nilai default yang menunjukkan bahwa sebuah variabel telah dideklarasikan tapi **belum diberi nilai secara tidak sengaja** atau sebuah properti/fungsi **tidak mengembalikan nilai**.

Contoh:

```
// Null
let data = null;
console.log(data); // null

// Undefined
// Variabel belum diisi
let a;
console.log(a); // undefined

// Fungsi tidak mengembalikan nilai
function greet() {}
console.log(greet()); // undefined

// Properti objek yang tidak ada
let obj = { name: "Alice" };
console.log(obj.age); // undefined

```

## Null isn't 0 or ""

```
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

```
typeof null; // "object"
```

Ini adalah bug historis di JavaScript — seharusnya null bukan objek, tapi JavaScript sudah terlanjur mendeteksinya begitu sejak awal (dan tidak diubah demi kompatibilitas).