# OBJECT-ORIENTED PROGRAMMING (OOP)

Object-oriented Programming (OOP) atau Pemrograman Berorientasi Objek adalah paradigma atau gaya berpikir dalam pemrograman yang berfokus pada objek, bukan sekadar fungsi atau logika.

## Encapsulation

Konsep encapsulation atau enkapsulasi, yaitu menyembunyikan detail internal dan hanya menampilkan hal penting. Properti dibuat private, hanya bisa diubah lewat method.

## Polymorphism

Konsep polymorphism memungkinkan method yang sama memiliki perilaku berbeda tergantung objek yang memanggilnya. Jenis-jenis polymorphism:

### 1. Overriding

Subclass mengubah method milik superclass agar perilakunya berbeda.

### 2. Overloading

Overloading artinya satu method bisa punya beberapa versi dengan parameter berbeda.

## Inheritance

Konsep inheritance atau pewarisan mengenal 2 jenis kelas, yaitu parent/super class sebagai kelas utama atau induk, dan child/subclass sebagai kelas pewaris atau anak. Dengan inheritance, kelas anak dapat mewarisi properti atau metode milik kelas induk.

## Abstraction

Konsep abstraction atau abstraksi, yaitu fokus pada inti fungsionalitas, tanpa peduli detail implementasi dari pembuatan properti atau metode. Yang terpenting adalah nama dari sebuah properti atau metode itu mudah dimengerti dan sederhana, agar kita tidak terlalu peduli dengan detail kodenya.

## Prototypal Inheritance

Prototypal inheritance adalah mekanisme pewarisan dalam JavaScript di mana objek bisa mewarisi properti dan metode dari objek lain melalui sesuatu yang disebut prototype.

Setiap objek secara otomatis mewarisi properti dan method dari prototype-nya.

Example:

```
let arr = [1, 2, 3];

console.log(arr.toString()); // Derived from Array.prototype
```