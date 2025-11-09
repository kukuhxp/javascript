# STATEMENT

Statement atau pernyataan adalah instruksi lengkap yang memberi tahu mesin JavaScript untuk melakukan suatu tindakan tertentu.

Statement adalah satu baris perintah logis yang dijalankan oleh JavaScript.

Setiap statement biasanya diakhiri dengan titik koma (;), meskipun JavaScript memiliki fitur Automatic Semicolon Insertion (ASI) yang menambahkannya otomatis.


Contoh:

```
let x = 10;         // Statement deklarasi dan inisialisasi
x = x + 5;          // Statement penugasan
console.log(x);     // Statement pemanggilan fungsi
```

Masing-masing baris di atas adalah statement karena semuanya melakukan aksi.

Jenis:

1. Declaration Statement

   Digunakan untuk mendeklarasikan variabel, fungsi, atau class.
   
   Contoh:
   
   ```
   let name = "Kukuh";
   function greet() { console.log("Halo!"); }
   ```
2. Expression Statement

   Ekspresi yang menghasilkan nilai dan biasanya diakhiri titik koma.
   
   Contoh:
   
   ```
   x + y; // Ini statement
   x + y // Ini ekspresi
   ```
   
3. Conditional Statement

   Digunakan untuk pengambilan keputusan.
   
   Contoh:
   
   ```
   if (x > 10) {
      console.log("Lebih besar dari 10");
   } else {
      console.log("10 atau kurang");
   } 
   ```
4. Looping statement

   Mengulang blok kode berkali-kali.
   
   Contoh:

   ```
   for (let i = 0; i < 5; i++) {
     console.log(i);
   } 
   ```
   
5. Control Flow Statement

   Mengubah alur eksekusi program.

   Contoh: 

   ```
   break;
   continue;
   return;
   throw new Error("Terjadi kesalahan");
   ```
   
## Automatic Semicolon Insertion (ASI)

Automatic Semicolon Insertion (ASI) adalah fitur bawaan JavaScript yang secara otomatis menambahkan titik koma (;) di tempat yang dianggap perlu, jika kamu tidak menulisnya sendiri.

Tujuannya adalah agar kode JavaScript tetap bisa berjalan walau kamu lupa menulis ; di akhir statement.

Contoh:

```
let x = 5
let y = 10
console.log(x + y)
```

Tapi JavaScript menambahkan titik koma secara otomatis seperti ini:

```
let x = 5;
let y = 10;
console.log(x + y);
```

Sehingga tetap bisa berjalan normal ✅

Kapan ASI bekerja:

1. Saat interpreter membaca baris baru.
1. Baris sebelumnya adalah ekspresi yang bisa diakhiri dengan ;.
2. Tidak ada tanda yang membuat JavaScript menunggu kelanjutan ekspresi.

Contoh:

```
a = b + c
d = e + f
```

Setelah c, JavaScript melihat akhir ekspresi, jadi menambahkan ; otomatis. Tapi hati-hati, ASI bisa bikin bug!, karena JavaScript kadang salah menebak niat kamu.

Contoh:

```
return
{
  name: "Kukuh"
}
```
Kamu mungkin berharap return object, tapi yang terjadi adalah:
```
return; // ← ASI menambahkan titik koma di sini!
{
  name: "Kukuh"
}
```
Hasilnya adalah fungsi mengembalikan undefined, bukan objek. Jadi cara yang benar adalah

```
return {
  name: "Kukuh"
};
```

ASI tidak selalu aman saat menggunakan return, break, continue, throw, dan emulai baris baru dengan tanda (, [, /, +, atau -

Contoh bug lainnya:

```
let x = 10
let y = x
(x + 1).toString()
```

JavaScript menganggap:

```
let x = 10;
let y = x(x + 1).toString();
```

