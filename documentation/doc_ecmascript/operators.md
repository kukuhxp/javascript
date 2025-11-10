# OPERATORS

## Increment / Decrement

### 1. Pre-increment / Pre-decrement Operators

Example:

```
let i = 5;
let x = ++i;

console.log(i); // 6
console.log(x); // 6
```

## 2. Post-increment / Post-decrement Operators
```
let i = 5;
let x = i++;
console.log(i); // 6
console.log(x); // 5  
```
   
## Nullish Coalescing

Nullish coalescing (??) adalah operator yang memberikan nilai default hanya jika nilai di sebelah kiri null atau undefined. Perbedaan dengan operator || adalah operator || menganggap semua falsy values (0, "", false) sama dengan false. ?? hanya memeriksa null atau undefined, sehingga 0 atau string kosong tidak diganti.

Syntax:

`let result = value ?? defaultValue;`

Explanation:

1. `value`

   Nilai yang ingin dicek.
   
2. `defaultValue`

   Nilai yang diberikan jika value null atau undefined.

Example:

```
let a = null;
let b = undefined;
let c = 0;
let d = "";

console.log(a ?? 10); // 10, because the a is null
console.log(b ?? 20); // 20, because the b is undefined
console.log(c ?? 30); // 0, not the null/undefined, but the result is 0
console.log(d ?? "empty"); // "", not the null/undefined, but the result is ""
```