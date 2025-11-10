# ERROR HANDLING

## Optional Chaining

Optional chaining adalah fitur yang memungkinkan kita mengakses properti atau memanggil fungsi dari sebuah objek tanpa menimbulkan error jika properti atau objek tersebut null atau undefined.

Example:

```
// Use in property
const user = { name: "Kukuh", address: { city: "Jakarta" } };

console.log(user.address?.city); // "Jakarta"
console.log(user.contact?.email); // undefined, no error

/**
 * user.address?.city - Access the city if address exists
 * user.contact?.email - contact does not exist, the result is undefined without error
 */
  
// Use in method
const user = {
  greet: () => "Hello"
};

console.log(user.greet?.()); // "Hello"
console.log(user.sayBye?.()); // undefined, no error

// Use in property
const arr = [1, 2, 3];

console.log(arr?.[0]); // 1
console.log(arr?.[10]); // undefined, no error

/**
 * Optional chaining makes code more error-safe.
 * Error like TypeError: Cannot read property 'x' of undefined.
 */
```