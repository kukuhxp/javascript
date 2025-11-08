# JAVASCRIPT OBJECTS

## Temporary Object

Temporary object adalah objek yang dibuat secara otomatis dan hanya digunakan sementara waktu oleh JavaScript, lalu dihapus setelah tugasnya selesai.

## Autoboxing

Ketika kamu menggunakan nilai primitif seperti string, number, atau boolean) dan memanggil method di atasnya, JavaScript membuat temporary object agar method itu bisa dipanggil.

```
// String variable
const text = "Halo";
console.log(text.toUpperCase());

// Equivalent
const temp = new String("Halo");
const result = temp.toUpperCase();
delete temp; // hapus (tidak disimpan)
```