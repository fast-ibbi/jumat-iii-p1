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

## Tujuan Pembelajaran

Memahami variabel, tipe data dasar, dan operator dalam JavaScript.

---

## Apa itu JavaScript?

JavaScript adalah bahasa pemrograman tingkat tinggi yang awalnya digunakan di browser untuk membuat halaman web menjadi interaktif.
Selain itu, dengan runtime Node.js, JavaScript juga dapat dijalankan di server.

---

## Variabel dalam JavaScript

Variabel adalah tempat untuk menyimpan data. Namanya digunakan untuk mengakses data tersebut di dalam program dan nilainya dapat berubah selama program berjalan.

---

## Menyatakan Variabel

JavaScript menggunakan kata kunci `var`, `let`, dan `const` untuk mendeklarasikan variabel.
`let` dan `const` adalah yang lebih modern dan direkomendasikan.
Contohnya:

```js
let nama = "Ani";
```

menyimpan string "Ani" ke variabel bernama nama.

---

## Perbedaan var, let, dan const

- **var**: variabel dengan cakupan fungsi (function scope) dan bersifat hoisting (diangkat ke atas saat eksekusi), tapi kurang direkomendasikan karena bisa menyebabkan bug.
- **let**: variabel dengan cakupan blok (block scope), tidak dihoisting secara sama, lebih aman digunakan.
- **const**: variabel dengan nilai konstan yang tidak bisa diubah setelah diberikan.

---

## Tipe Data Primitif

JavaScript memiliki tipe data dasar penting seperti:

- Number (angka)
- String (teks)
- Boolean (true/false)
- null (nilai kosong eksplisit)
- undefined (nilai belum didefinisikan)

---

## Number

Tipe data angka yang bisa berupa bilangan bulat maupun pecahan.
Contoh: 10, 3.14, -25.
Contoh deklarasi:

```js
let angka = 10;
```

Digunakan untuk operasi matematika.

---

## String

Tipe data teks yang dikelilingi oleh tanda kutip tunggal (' ') atau ganda (" ").
Contoh:

```js
let greeting = "Hello";
```

Digunakan untuk merepresentasikan kalimat atau kata.

---

## Boolean

Tipe data yang hanya memiliki dua nilai: true (benar) dan false (salah).
Umumnya digunakan dalam logika dan pengkondisian program.

---

## null dan undefined

- **null**: nilai kosong yang sengaja diberikan programmer untuk menyatakan tidak ada nilai.
- **undefined**: nilai default untuk variabel yang sudah dideklarasikan tapi belum diberikan nilai.

---

## Operator Aritmatika

Operator dasar matematika: `+ (tambah)`, `- (kurang)`, `* (kali)`, `/ (bagi)`, `% (modulus/sisa bagi)`, `++ (increment)`, `-- (decrement)`.
Digunakan untuk operasi hitung dalam program.

---

## Operator Penugasan

Operator yang digunakan untuk menetapkan nilai ke variabel.
Contohnya:

- = asignasi biasa
- += penambahan lalu penugasan
- -= pengurangan lalu penugasan
  Untuk menulis kode yang ringkas.

---

## Operator Perbandingan

Operator yang membandingkan dua nilai dan menghasilkan nilai boolean.
Contohnya:

- == (sama nilai)
- === (sama nilai dan tipe)
- != (tidak sama nilai)
- !== (tidak sama nilai atau tipe)
- `>` , `<`, `>=`, `<=` untuk perbandingan nilai.

---

## Operator Logika

Operator yang menggabungkan kondisi:

- && (AND): true jika kedua kondisi benar
- || (OR): true jika salah satu kondisi benar
- ! (NOT): membalik nilai boolean
  Berguna untuk membuat logika kompleks.

---

## Contoh Penggunaan Operator

Penjelasan contoh kode yang mengkombinasikan operator aritmatika dan logika:

```js
let a = 5;
let b = 10;
if (a < b && b > 0) {
  console.log("b lebih besar");
}
```

---

## Tips Menulis Kode JavaScript

- Gunakan nama variabel yang jelas dan deskriptif
- Tambahkan komentar jika perlu
- Hindari kode yang membingungkan

---

## Kesalahan Umum

- Salah tipe data saat operasi
- Menggunakan `var` tanpa sadar cakupannya
- Variabel tak terdefinisi

---

## Debugging Sederhana

Mengajari cara membaca pesan error
Menggunakan `console.log` supaya bisa menelusuri jalannya program dan nilai variabel.

---

<!-- ## Soal Praktik

---

## Soal 1: Variabel dan Tipe Data

Buatlah program JavaScript yang:

1. Mendeklarasikan variabel `nama` dengan tipe string berisi nama Anda
2. Mendeklarasikan variabel `umur` dengan tipe number berisi umur Anda
3. Mendeklarasikan variabel `mahasiswa` dengan tipe boolean bernilai `true`
4. Tampilkan ketiga variabel tersebut menggunakan `console.log`

---

## Soal 2: Operator Aritmatika

Buatlah program yang:

1. Deklarasikan dua variabel `angka1 = 15` dan `angka2 = 4`
2. Hitung dan tampilkan hasil dari:
   - Penjumlahan
   - Pengurangan
   - Perkalian
   - Pembagian
   - Modulus (sisa bagi)
3. Gunakan `console.log` untuk menampilkan setiap hasil operasi

---

## Soal 3: Operator Perbandingan

Diberikan dua variabel:

```js
let nilai1 = 85;
let nilai2 = "85";
```

Buatlah program yang menampilkan hasil perbandingan:

1. `nilai1 == nilai2`
2. `nilai1 === nilai2`
3. `nilai1 > 80`
4. `nilai2 >= 85`
   Jelaskan mengapa hasilnya berbeda pada poin 1 dan 2!

---

## Soal 4: Operator Logika

Buatlah program yang memeriksa kelulusan mahasiswa dengan kriteria:

1. Deklarasikan variabel `nilaiUTS = 75`, `nilaiUAS = 80`, `absensi = 90`
2. Mahasiswa lulus jika:
   - Nilai UTS >= 70 DAN nilai UAS >= 70 DAN absensi >= 80
3. Gunakan operator logika untuk memeriksa kondisi tersebut
4. Tampilkan "LULUS" atau "TIDAK LULUS" sesuai hasil

---

## Soal 5: Kombinasi Operator

Buatlah kalkulator sederhana yang:

1. Mendeklarasikan variabel `bilangan1 = 20` dan `bilangan2 = 8`
2. Hitung rata-rata dari kedua bilangan
3. Periksa apakah rata-rata tersebut:
   - Lebih dari 10 DAN kurang dari 20
   - Sama dengan 14
4. Tampilkan hasil perhitungan dan hasil pemeriksaan kondisi
5. Gunakan operator penugasan `+=` untuk menambah nilai `bilangan1` sebesar 5
 -->
