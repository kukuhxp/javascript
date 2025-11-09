# CONTROL ABSTRACTION

Control abstraction atau abstraksi kontrol adalah konsep dalam pemrograman yang menyembunyikan detail bagaimana suatu kontrol alur bekerja, sehingga programmer cukup fokus pada apa yang dilakukan, bukan bagaimana cara melakukannya.

Control abstraction memungkinkan kita mengelompokkan pola kontrol seperti looping, kondisi, atau pemanggilan fungsi menjadi bentuk yang lebih umum dan mudah digunakan, tanpa menulis ulang logika detail setiap kali.

Dengan kata lain, kita menyembunyikan mekanisme kontrol di balik nama fungsi, prosedur, atau konstruk khusus.


Contoh:

```
// Tanpa abstraksi kontrol, kamu mengatur detail bagaimana loop berjalan inisialisasi, kondisi, increment.
let arr = [1, 2, 3];
for (let i = 0; i < arr.length; i++) {
  console.log(arr[i]);
}

// Dengan abstraksi kontrol, kamu hanya memberi tahu apa yang harus dilakukan, bukan bagaimana melakukannya.
forEach sudah menyembunyikan mekanisme loop, itulah control abstraction.
arr.forEach(item => console.log(item));
```

Konsep:

1. Meningkatkan Keterbacaan Kode
   
   Programmer fokus pada tujuan alih-alih detail teknis.


2. Mengurangi Duplikasi

   Logika kontrol umum ditulis sekali, lalu dipakai berulang.

3. Memudahkan Pemeliharaan

   Jika cara kerja internal berubah, cukup ubah di satu tempat.