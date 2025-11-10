# OBJECT-ORIENTED PROGRAMMING (OOP)

## Prototypal Inheritance

Prototypal inheritance adalah mekanisme pewarisan dalam JavaScript di mana objek bisa mewarisi properti dan metode dari objek lain melalui sesuatu yang disebut prototype.

Setiap objek secara otomatis mewarisi properti dan method dari prototype-nya.

Example:

```
let arr = [1, 2, 3];

console.log(arr.toString()); // Derived from Array.prototype
```