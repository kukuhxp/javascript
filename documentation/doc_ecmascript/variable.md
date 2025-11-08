# VARIABLE

## Variable

JavaScript menggunakan fitur loosely type, sehingga ketika membuat sebuah variabel, JavaScript tidak menyediakan keyword untuk mendeklarasikan tipe data dari variabel tersebut

Jenis:

1. Let

   ```
   // Unassigned variable
   let variable;
   
   // Assigning variable
   let variable;
   variable = value;
   
   // Assigned variable
   let variable = value`
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

## Hoisting

Hoisting adalah mekanisme dalam JavaScript di mana deklarasi variabel dan fungsi diangkat ke atas scope-nya sebelum kode dijalankan.