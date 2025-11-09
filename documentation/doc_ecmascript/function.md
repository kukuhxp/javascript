# FUNCTION

Function adalah sebuah object yang dapat menjalankan beberapa baris perintah. Function terdiri dari name, parameter dan body.

1. Declaration

   ```
   // Declaration
   function functionX(parameter, parameter n) {
     functionBody;
   }
   functionX() // Invocation
   ```

2. Arrow Function

   ```
   // Arrow Function 1
   let variable = (parameter, parameter n) => {
      functionBody;
      return;
   }
   variable(); // Invocation

   // Arrow Function 2: Tanpa Parameter
   let variable = () => functionBody;
   variable(); // Invocation

   // Arrow Function 3: Satu Parameter
   let variable = parameter => statement; // Parameter bokeh tidak menggunakan tanda kurung.
   variable(); // Invocation

   // Arrow Function 4: Dua Parameter atau Lebih
   const buatUser = (nama, umur) => ({ nama, umur });
   console.log(buatUser("Kukuh", 25)); // Invocation
   /* Harus dibungkus tanda kurung () agar tidak disangka blok kode. */
   ```

3. Function Expression

   ```
   let variable = function (parameter, parameter n) {
      functionBody;
   }
   variable(); // Invocation
   ```
4. Named Function Expression (NFE)

   ```
   let variable = function functionX (parameter, parameter n) {
      functionBody;
   }
   
   // Invocation
   variable(); ✅
   functionX(); ❌
   
   /*
     * Kenapa sayHello() tidak bisa dipanggil langsung?
     * Karena nama sayHello hanya berlaku di dalam function itu sendiri.
     * Kapan NFE berguna?
     * Untuk rekursi (memanggil dirinya sendiri) tanpa membuat nama global:
   */
   const factorial = function f(n) {
      return n === 0 ? 1 : n * f(n - 1);
   };
   console.log(factorial(5)); // 120
   ```
   
5. Higher-order Function (HOF)

   Higher-order Function (HOF) adalah function yang menerima function sebagai argumen, atau mengembalikan function lain.

   ```
   function functionX() {
     // Anonymous Function
     return function() {
       functionBody
     };
   }
   const variable = functionX();
   sayHello(); // Function Variable
   ```

6. Function Constructor

   ```
   let variable = new Function(args, return);
   ```

7. Generator Function

   ```
   function* functionX(parameter, parameter n) {
     yield value;
   }
   let object = functionName(); // Generator object
   object.next(); // next() is instance method
   ```

8. Immediately Invoked Function Expression (IIFE)

   ```
   // IIFE
   (function(parameter, parameter n) {
     functionBody;
   })();

   // IIFE Arrow Function
   ((parameter, parameter n) => {
     functionBody;
   })()
   ```

9. Callback

   Callback adalah fungsi yang dikirim sebagai argumen ke fungsi lain, dan akan dipanggil kembali (callback) di dalamnya.
   
   Contoh:
   ```
   // Named Callback Function
   function functionX(parameter, callback) {
      callback();
   }
   function callback(parameter) { // Callback
      functionBody;
   }
   functionX(args, callback); // Invocation

   // Anonymous Callback 1: Function Declaration
   function functionX(parameter, callback) {
      callback();
   }
   functionName(args, function(e) {    // Invocation
      functionBody;
   });
   
   // Anonymous Callback 2: setTimeout. Function
   setTimeout(function() {
      console.log("Jalan setelah 2 detik");
   }, 2000);
   
   // Anonymous Callback 3: addEventListener() Method
   document.addEventListener("click", function() {
      console.log("Kamu mengklik dokumen!");
   })
   
   // Anonymous Callback 4: forEach() Method
   const angka = [1, 2, 3];
   angka.forEach(function(item) {
      console.log(item);
   });
   
   // Anonymous Callback 4: map() Method
   const kuadrat = [1, 2, 3].map(function(num) {
      return num * num;
   });
   console.log(kuadrat); // [1, 4, 9]
   ```
   
## Function as First-Class Citizen

Function di JavaScript adalah nilai yang bisa disimpan di variabel, dikirim sebagai argumen, atau dikembalikan dari function lain.

Contoh:

```
function greet() { console.log("Hi"); }
const say = greet; // simpan di variabel
say(); // Hi
```

## Function vs Arrow Function

Perbedaan penting dengan function biasa adalah arrow function tidak punya this sendiri, ia mewarisi this dari scope di atasnya. Kalau pakai function() biasa di dalam setTimeout, this akan berubah dan tidak lagi mengacu ke obj.

```
const obj = {
  nama: "Kukuh",
  sayHi: function() {
    setTimeout(() => {
      console.log("Hai " + this.nama);
    }, 1000);
  }
};
obj.sayHi(); // Output: Hai Kukuh
```

## Callback

Callback adalah sebuah function yang dikirim melalui argumen function atau method.

## Closure

Closure adalah sebuah konsep di mana fungsi dapat mengakses scope bagian luar fungsi.

Contoh:

```
function outer() {
  let count = 0;
  return function() {
    count++;
    console.log(count);
  };
}

const counter = outer();
counter(); // 1
counter(); // 2
```
## Anonymous

Anonymous adalah istilah yang merujuk kepada function yang tidak memiliki nama.

## Asynchronous

Asynchronous adalah proses menjalankan program dibalik layar tanpa menghentikan eksekusi program utama. JavaScript hanya punya 1 thread utama, tapi bisa menangani asynchronous task lewat event loop.

Contoh:

```
console.log("Mulai");
setTimeout(() => console.log("Tunggu 1 detik"), 1000);
console.log("Selesai");

// Output:
Mulai
Selesai
Tunggu 1 detik
```
## Parameters

1. General Parameter

   General parameter adalah parameter yang umum digunakan saat mendeklarasikan sebuah fungsi. Perlu diingat bahwa pengiriman argumen ke parameter adalah berurutan. Jadi, jika kita mengirim argumen pertama ke sebuah fungsi, maka paramater yang akan menerima adalah parameter yang pertama.

2. Optional Parameter

3. Default Parameter

4. Rest Parameter

5. Object Parameter

6. Array Parameter