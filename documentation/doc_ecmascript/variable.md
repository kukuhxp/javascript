# VARIABLE

## Variable

JavaScript menggunakan fitur loosely type, sehingga ketika membuat sebuah variabel, JavaScript tidak menyediakan keyword untuk mendeklarasikan tipe data dari variabel tersebut

Jenis:

1. Let

   ```
   // Unassigned Variable
   let variable;
   
   // Assigned Variable
   let variable = value`
   
   // Assigning Variable
   let variable;
   variable = value;
   
   // Reassigning Variable
   let variableX;
   variableX= value;
   variablX = newValue;
   let variableY = value;
   let variableY= = newValue;
   ```

2. Const
   ```
   // Constant Variable
   const a = 8;
   a = 10; // Error

   // Constant Array
   const b = [10, 9];
   b = [2, 5]; // Error
   
   // Constant Object
   const c = {age: 20};
   c = {age: 23}; // Error
   ```

3. Var

## Variable Scope

```
global variable
{
  lexical variable
}
```

## Auto-boxing, Boxing & Unboxing

1. Auto-boxing

   ```
   let variable = value;
   variable.method();
   ```

2. Boxing & Unboxing

   ```
   // Boxing
   let object = new Object(value);
   
   // Unboxing  
   let object = Object.method();
   ```

## Casting

1. Implicit Casting

   Casting yang dilakukan secara otomatis tanpa menggunakan method apapun.
   
2. Explicit Casting

   Casting yang dilakukan secara manual dengan menggunakan method.

## Type Coercion

JavaScript bisa mengubah tipe data secara otomatis saat dibutuhkan. Kadang type coercion itu berguna, tapi juga sebagai sumber bug, karena JavaScript ingin menjadi terlalu pintar.

Contoh:

```
console.log("5" - 2); // 3, string "5" diubah jadi number
console.log("5" + 2); // "52", karena ada +, maka 2 diubah jadi string
```

## Hoisting

Hoisting adalah mekanisme dalam JavaScript di mana deklarasi variabel dan fungsi diangkat ke atas scope-nya sebelum kode dijalankan.

Contoh:

```
sayHi(); // ✅ Berjalan
function sayHi() { console.log("Hai!"); }

// Tapi hati-hati dengan let atau const
console.log(x); // ❌ ReferenceError
let x = 10;
```

## Global Object Binding

Jika kamu membuat variabel tanpa let, const, atau var,
JavaScript secara otomatis menambahkannya ke objek global.

Contoh:

```
x = 10; // ❌ Buruk, tapi valid
console.log(window.x); // 10
```
## Loosely Typed

Loosely typed atau dynamically typed adalah karakteristik dari bahasa pemrograman di mana variabel tidak perlu dideklarasikan dengan tipe data tertentu secara eksplisit. Tipe data akan ditentukan secara otomatis saat program dijalankan, berdasarkan nilai yang diberikan.

## Dynamic Typing

Variabel bisa berganti tipe data kapan saja, karena JavaScript bukan bahasa statis, tipe data tidak dikunci.

Contoh:

```
let value = 42;      // number
value = "Hello";     // string
value = true;        // boolean
```