# OPERATORS

## Increment / Decrement

1. Pre-increment / Pre-decrement

   ```
   let i = 5;
   let x = ++i;
   console.log(i); // 6
   console.log(x); // 6
   ```

2. Post-increment / Post-decrement

   ```
   let i = 5;
   let x = i++;
   console.log(i); // 6
   console.log(x); // 5  
   ```
   
## Nullish Coalescing

Nullish coalescing (??) adalah operator yang memberikan nilai default hanya jika nilai di sebelah kiri null atau undefined. Perbedaan dengan operator || adalah operator || menganggap semua falsy values (0, "", false) sama dengan false. ?? hanya memeriksa null atau undefined, sehingga 0 atau string kosong tidak diganti.

Sintaks:

`let result = value ?? defaultValue;`

Keterangan:

1. value = nilai yang ingin dicek
2. defaultValue = nilai yang diberikan jika value null atau undefined

Contoh:

```
let a = null;
let b = undefined;
let c = 0;
let d = "";

console.log(a ?? 10); // 10, karena a null
console.log(b ?? 20); // 20, karena b undefined
console.log(c ?? 30); // 0, bukan null/undefined, tapi hasilnya 0
console.log(d ?? "empty"); // "", bukan null/undefined, tapi hasilnya ""
```