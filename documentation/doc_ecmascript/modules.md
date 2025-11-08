# JAVASCRIPT MODULES

Modules atau modul adalah cara memecah kode JavaScript menjadi file-file terpisah agar lebih mudah dibaca, bisa digunakan ulang, dan tidak saling bentrok (karena punya ruang lingkup sendiri.

Setiap file .js dianggap sebuah modul, yang bisa mengekspor variabel, fungsi, atau class agar bisa digunakan di file lain, dan mengimpor (import) ekspor dari modul lain.

Sebelum ada modul (jaman ES5 ke bawah), semua script disatukan dalam satu ruang global (window), sehingga nama variabel atau fungsi bisa saling bentrok, dan sulit memelihara kode besar.

Dengan ES Modules (ESM), setiap file punya scope sendiri, hanya apa yang di-export bisa diakses dari luar.

Syntax:

```
<script type="module" src="main.js"></script>
```

Browser otomatis menjalankan main.js sebagai ES Module,
yang artinya kita bisa pakai import dan export, dan program mempunyai strict mode aktif otomatis.

Contoh:

```
// math.js
export function tambah(a, b) {
  return a + b;
}

export const PI = 3.14159;

// main.js

import { tambah, PI } from './math.js';

console.log(tambah(2, 3)); // 5
console.log(PI);           // 3.14159
```


Penjelasan:

1. export = mengizinkan sesuatu dari file math.js agar bisa digunakan di file lain.
2. import = mengambil hasil export dari modul lain.

## Module Scope

Contoh:

```
// math.js
const rahasia = 42;
export const angka = 10;

// main.js
import { angka } from './math.js';

console.log(angka);    // ✅ 10
console.log(rahasia);  // ❌ Error: rahasia is not defined

// Variabel rahasia tidak bisa diakses dari luar karena tidak di-export.
```

## Export

1. Named Export

   ```
   // Export:
   export const name = 'Kukuh';
   export function hello() { console.log('Hai!'); }

   // Import:
   import { name, hello } from './modul.js';
   ```

2. Default Export

   Satu modul hanya boleh punya satu default export.

   ```
   // Export:
   export default function() {
     console.log('Ini default export!');
   }

   // Import:
   import myFunc from './modul.js';
   ```