# ERROR HANDLING

## Optional Chaining

Optional chaining adalah fitur yang memungkinkan kita mengakses properti atau memanggil fungsi dari sebuah objek tanpa menimbulkan error jika properti atau objek tersebut null atau undefined.

Contoh:

```
// Penggunaan di property
const user = { name: "Kukuh", address: { city: "Jakarta" } };
console.log(user.address?.city); // "Jakarta"
console.log(user.contact?.email); // undefined, tidak error

/**
  * user.address?.city → mengakses city jika address ada
  * user.contact?.email → contact tidak ada → hasilnya undefined tanpa error
  */
  
// Penggunaan di method
const user = {
  greet: () => "Hello"
};
console.log(user.greet?.()); // "Hello"
console.log(user.sayBye?.()); // undefined, tidak error

//  Penggunaan di array
const arr = [1, 2, 3];
console.log(arr?.[0]); // 1
console.log(arr?.[10]); // undefined, tidak error
```

Kesimpulan:

Optional chaining membuat kode lebih aman dari error seperti TypeError: Cannot read property 'x' of undefined
