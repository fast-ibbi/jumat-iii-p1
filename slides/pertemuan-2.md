---
title: Dasar JavaScript (variabel, tipe data, operator)
version: 1.0.0
header: Dasar JavaScript (variabel, tipe data, operator)
footer: https://github.com/fast-ibbi/jumat-iii-p1
paginate: true
marp: true
---

<!--
_class: lead
_paginate: skip
-->

# Dasar JavaScript (variabel, tipe data, operator)

---

## Pendahuluan

**Mengapa JavaScript penting untuk pemrograman web?**

- Bahasa utama untuk pembuatan web interaktif
- Digunakan di browser (client-side) & di server (server-side, misal dengan Node.js)

JavaScript memungkinkan menampilkan efek dinamis dalam halaman web modern.

---

## Variabel dalam JavaScript

**Variabel** adalah tempat menyimpan data yang nilainya bisa diubah selama program berjalan.

Contoh deklarasi:

```js
let nama = "Rani";
var umur = 20;
const PI = 3.14;
```

Di atas, `nama`, `umur`, dan `PI` adalah variabel dengan isi data yang berbeda-beda.

---

## Cara Deklarasi Variabel

Ada tiga cara mendeklarasikan variabel di JavaScript:

- `var` (lama)
- `let` (ES6, modern)
- `const` (nilai tetap)

Contoh:

```js
var kota = "Bandung";
let hari = "Senin";
const tahun = 2025;
```

Gunakan `let` atau `const` untuk penulisan modern.[2][3]

---

## Perbedaan var, let, dan const

| Keyword | Lingkup Scope | Bisa diubah? |
| ------- | ------------- | ------------ |
| var     | Function      | Ya           |
| let     | Block         | Ya           |
| const   | Block         | Tidak        |

`const` tidak dapat diubah nilainya setelah deklarasi.[2][3]

---

## Aturan Penulisan Variabel

1. Nama diawali huruf, \_ atau $
2. Tidak boleh ada spasi
3. Tidak boleh menggunakan kata kunci (reserved words)
4. Case-sensitive (huruf besar dan kecil beda)

---

Contoh penamaan:

```js
let hasilUjian = 90;
let _alamat = "Jakarta";
let $gaji = 2500000;
```

---

## Contoh Variabel yang Valid dan Tidak Valid

- Valid: `namaSiswa`, `_nilaiAkhir`, `$totalGaji`
- Tidak valid: `1nama`, `total nilai`, `var`

Cth (salah):

```js
let 1nama = "Budi"; // tidak valid
let my name = "Dina"; // tidak valid
let var = 10; // tidak valid
```

---

## Quiz

Keyword manakah yang digunakan untuk mendeklarasikan variabel dengan nilai yang tidak bisa diubah?

A. `var`
B. `let`
C. `const`
D. `final`

---

## Quiz

Manakah penulisan nama variabel yang TIDAK valid?

A. `namaSiswa`
B. `_nilaiAkhir`
C. `$totalGaji`
D. `1nama`

---

## Tipe Data Dasar JavaScript

- **String** ‒ kumpulan teks
- **Number** ‒ bilangan bulat/pecahan
- **Boolean** ‒ true/false
- **Undefined** ‒ belum diberi nilai
- **Null** ‒ kosong
- **Object** ‒ gabungan data
- **Symbol** (fitur baru ES6)

---

## Tipe Data String

Digunakan untuk menyimpan teks.

Contoh:

```js
let judul = "Belajar JavaScript";
let namaDepan = "Tina";
```

Baik tanda kutip tunggal ataupun ganda bisa digunakan.

---

## Tipe Data Number

Angka bulat atau desimal. JavaScript tidak membedakan antara integer dan float.

Contoh:

```js
let umur = 21;
let phi = 3.14;
```

Dapat digunakan pada operasi matematika langsung.

---

## Tipe Data Boolean

Hanya dua nilai: `true` atau `false`.

Contoh:

```js
let isLogin = true;
let isMember = false;
```

Sering digunakan pada logika seleksi atau perulangan.

---

## Tipe Data Undefined dan Null

- **Undefined**: Variabel dideklarasi tapi tidak ada isinya.
- **Null**: Variabel secara eksplisit diisi "kosong".

Contoh:

```js
let harga;
console.log(harga); // undefined
let diskon = null;
console.log(diskon); // null
```

---

## Tipe Data Object dan Array

- **Object:** Gabungan data berupa pasangan "key: value"
- **Array:** Kumpulan data (list), urut.

Contoh Object:

```js
let user = { nama: "Bayu", umur: 23 };
```

Contoh Array:

```js
let buah = ["apel", "jeruk", "anggur"];
```

---

## Contoh Object dan Array

**Object:**

```js
let buku = {
  judul: "Algoritma",
  penulis: "Eko",
};
```

**Array:**

```js
let nilai = [80, 75, 92];
```

Bisa diakses menggunakan `buku.judul` atau `nilai[0]`.

---

## Quiz

Tipe data apakah `true` dan `false`?

A. String
B. Number
C. Boolean
D. Undefined

---

## Operator dalam JavaScript

Operator digunakan untuk operasi data.
Jenis utama:

- Assignment
- Arithmetic (Aritmatika)
- Comparison (Perbandingan)
- Logical (Logika)

---

## Operator Assignment

Digunakan untuk memberi atau mengubah nilai variabel.
Simbol umum: `=`, `+=`, `-=`, `*=`, `/=`

Contoh:

```js
let x = 10; // assignment
x += 5; // x = x + 5 => x = 15
```

---

## Contoh Operator Assignment

```js
let nilai = 7;
nilai *= 2; // nilai = 14
nilai -= 4; // nilai = 10
console.log(nilai);
```

---

## Quiz

Apa hasil dari kode berikut?

```js
let x = 10;
x += 5;
console.log(x);
```

A. 10
B. 15
C. 5
D. Error

---

## Operator Arithmetic

Untuk perhitungan matematika:

- Penjumlahan: `+`
- Pengurangan: `-`
- Perkalian: `*`
- Pembagian: `/`
- Sisa bagi: `%`

---

Contoh:

```js
let hasil = 9 + 5; // 14
let sisa = 10 % 3; // 1
```

---

## Contoh Operator Arithmetic

```js
let a = 6,
  b = 4;
let tambah = a + b; // 10
let kurang = a - b; // 2
let kali = a * b; // 24
let bagi = a / b; // 1.5
let sisa = a % b; // 2
console.log(tambah, kurang, kali, bagi, sisa);
```

---

## Quiz

Apa hasil dari `10 % 3`?

A. 3
B. 3.33
C. 1
D. 0

---

## Operator Comparison

Digunakan untuk membandingkan dua nilai:

- `==`, `===` : sama dengan
- `!=`, `!==` : tidak sama dengan
- `>`, `<`, `>=`, `<=` : lebih/kurang dari

Contoh:

```js
console.log(5 > 3); // true
console.log(5 == "5"); // true
```

---

## Perbedaan == dan ===

- `==` membandingkan nilai saja (lewat konversi tipe)
- `===` membandingkan tipe dan nilai sekaligus

Contoh:

```js
console.log(4 == "4"); // true
console.log(4 === "4"); // false
```

---

## Operator Logical

Untuk menggabung/negasikan kondisi:

- AND `&&`
- OR `||`
- NOT `!`

Contoh:

```js
let umur = 22;
let siswa = true;
console.log(umur > 18 && siswa); // true
console.log(umur < 18 || siswa); // true
console.log(!siswa); // false
```

---

## Quiz

Operator logika manakah yang menghasilkan `true` jika KEDUA kondisi bernilai `true`?

A. `||`
B. `&&`
C. `!`
D. `==`

---

## Contoh Operator Logical

```js
let lulus = true;
let nilaiA = 85;
if (lulus && nilaiA > 80) {
  console.log("Dapat beasiswa");
}
```

---

## Quiz

Apa perbedaan antara `==` dan `===`?

A. Tidak ada perbedaan
B. `==` membandingkan nilai, `===` membandingkan tipe dan nilai
C. `===` lebih cepat dari `==`
D. `==` hanya untuk number, `===` untuk semua tipe

---

## Contoh Program Sederhana

Program untuk menentukan kelulusan:

```js
let nilai = 70;
let status = nilai >= 60 ? "Lulus" : "Tidak Lulus";
console.log(status);
```

Menggunakan operator ternary `? :`.[11]

---

## Operator String

Digunakan untuk menggabungkan string dengan `+`.
Contoh:

```js
let depan = "Halo ";
let belakang = "Dunia";
let hasil = depan + belakang; // "Halo Dunia"
console.log(hasil);
"Belajar" + " JavaScript"; // "Belajar JavaScript"
```

---

## Quiz

Bagaimana cara menggabungkan dua string "Hello" dan "World"?

A. `"Hello" - "World"`
B. `"Hello" + "World"`
C. `"Hello" * "World"`
D. `"Hello" & "World"`
