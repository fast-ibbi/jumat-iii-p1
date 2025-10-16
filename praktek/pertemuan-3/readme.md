# Praktek Pertemuan 3 - Struktur Kontrol (if, switch, loop)

## Petunjuk Umum

- Buat file JavaScript terpisah untuk setiap soal (misal: `soal1.js`, `soal2.js`, dst)
- Jalankan setiap file menggunakan Node.js: `node soal1.js`
- Pastikan output sesuai dengan yang diminta
- Tulis kode yang rapi dan mudah dibaca

---

## Soal 1: Penentu Grade Nilai

Buatlah program yang menentukan grade nilai mahasiswa berdasarkan kriteria berikut:

- Nilai >= 85: Grade A
- Nilai >= 75: Grade B
- Nilai >= 65: Grade C
- Nilai >= 55: Grade D
- Nilai < 55: Grade E

**Input:**

```javascript
let nilai = 78;
```

**Output yang diharapkan:**

```
Nilai: 78
Grade: B
```

**Catatan:** Gunakan struktur `if...else if...else`

---

## Soal 2: Kalkulator Sederhana dengan Switch

Buatlah program kalkulator sederhana yang dapat melakukan operasi dasar (tambah, kurang, kali, bagi) menggunakan `switch` statement.

**Input:**

```javascript
let angka1 = 10;
let angka2 = 5;
let operator = "+"; // bisa: +, -, *, /
```

**Output yang diharapkan:**

```
10 + 5 = 15
```

**Catatan:**

- Gunakan switch untuk memilih operasi
- Tambahkan case default untuk operator tidak valid
- Handle pembagian dengan 0

---

## Soal 3: Menampilkan Bilangan Ganjil

Buatlah program yang menampilkan semua bilangan ganjil dari 1 sampai 20 menggunakan loop `for` dan `continue`.

**Output yang diharapkan:**

```
1
3
5
7
9
11
13
15
17
19
```

**Catatan:** Gunakan operator modulo (%) untuk menentukan bilangan ganjil

---

## Soal 4: Tabel Perkalian

Buatlah program yang menampilkan tabel perkalian untuk angka tertentu (1-10) menggunakan loop `for`.

**Input:**

```javascript
let angka = 5;
```

**Output yang diharapkan:**

```
Tabel Perkalian 5:
5 x 1 = 5
5 x 2 = 10
5 x 3 = 15
5 x 4 = 20
5 x 5 = 25
5 x 6 = 30
5 x 7 = 35
5 x 8 = 40
5 x 9 = 45
5 x 10 = 50
```

---

## Soal 5: Validasi Login dengan Nested If

Buatlah program validasi login sederhana yang memeriksa username dan password.

**Input:**

```javascript
let inputUsername = "admin";
let inputPassword = "12345";

let validUsername = "admin";
let validPassword = "admin123";
```

**Output yang diharapkan:**

```
Username benar
Password salah!
```

**Atau jika username salah:**

```
Username tidak ditemukan
```

**Atau jika keduanya benar:**

```
Username benar
Password benar
Login berhasil!
```

**Catatan:** Gunakan nested if untuk memeriksa password hanya jika username benar

---

## Soal 6: Hitung Faktorial dengan While

Buatlah program yang menghitung faktorial dari suatu bilangan menggunakan loop `while`.

**Input:**

```javascript
let n = 5;
```

**Output yang diharapkan:**

```
Faktorial dari 5 adalah: 120
```

**Penjelasan:** 5! = 5 × 4 × 3 × 2 × 1 = 120

---

## Soal 7: Menu Minuman dengan Switch (Multiple Cases)

Buatlah program yang menampilkan kategori minuman berdasarkan pilihan menu. Beberapa minuman bisa memiliki kategori yang sama.

**Input:**

```javascript
let pilihanMenu = 2;
```

**Kategori:**

- 1, 2, 3: Minuman Dingin (Es Teh, Es Jeruk, Es Kopi)
- 4, 5, 6: Minuman Panas (Teh Panas, Kopi Panas, Coklat Panas)
- 7, 8: Minuman Spesial (Smoothie, Milkshake)

**Output yang diharapkan:**

```
Menu: 2
Kategori: Minuman Dingin
```

**Catatan:** Manfaatkan fall-through pada switch (case tanpa break untuk menggabungkan beberapa case)

---

## Soal 8: Pola Bintang dengan Nested Loop

Buatlah program yang menampilkan pola bintang segitiga menggunakan nested loop.

**Input:**

```javascript
let tinggi = 5;
```

**Output yang diharapkan:**

```
*
**
***
****
*****
```

**Catatan:** Gunakan dua loop `for` (outer loop untuk baris, inner loop untuk kolom)

---

## Soal 9: Cari Bilangan Prima

Buatlah program yang memeriksa apakah suatu bilangan adalah bilangan prima atau bukan.

**Input:**

```javascript
let angka = 17;
```

**Output yang diharapkan:**

```
17 adalah bilangan prima
```

**Penjelasan:**

- Bilangan prima adalah bilangan > 1 yang hanya bisa dibagi 1 dan dirinya sendiri
- Gunakan loop untuk memeriksa pembagi dari 2 sampai angka-1
- Gunakan `break` jika ditemukan pembagi

---

## Soal 10: Iterasi Array Mahasiswa dengan for...of

Buatlah program yang menampilkan daftar mahasiswa dan menghitung total mahasiswa menggunakan `for...of` loop.

**Input:**

```javascript
const mahasiswa = ["Budi", "Ani", "Citra", "Doni", "Eka"];
```

**Output yang diharapkan:**

```
Daftar Mahasiswa:
1. Budi
2. Ani
3. Citra
4. Doni
5. Eka

Total mahasiswa: 5
```

**Catatan:** Gunakan loop `for...of` dan variabel counter untuk penomoran

---

## Bonus Challenge 🌟

### Soal Bonus: Program ATM Sederhana

Buatlah program ATM sederhana yang memiliki menu:

1. Cek Saldo
2. Tarik Tunai
3. Setor Tunai
4. Keluar

**Input:**

```javascript
let saldo = 1000000;
let pilihan = 2; // pilihan menu
let nominal = 200000; // untuk tarik/setor
```

**Output yang diharapkan (untuk pilihan 2, tarik tunai 200000):**

```
=== ATM Sederhana ===
Saldo awal: Rp 1000000

Menu dipilih: Tarik Tunai
Nominal: Rp 200000
Transaksi berhasil!

Saldo akhir: Rp 800000
```

**Requirements:**

- Gunakan `switch` untuk menu
- Validasi saldo cukup untuk tarik tunai
- Validasi nominal > 0 untuk setor
- Tampilkan saldo awal dan akhir

---

## Tips Pengerjaan

1. **Baca soal dengan teliti** - Perhatikan input dan output yang diharapkan
2. **Gunakan struktur kontrol yang tepat** - if untuk kondisi kompleks, switch untuk nilai tetap
3. **Test dengan berbagai input** - Coba berbagai nilai untuk memastikan program bekerja
4. **Perhatikan edge cases** - Nilai negatif, 0, atau nilai ekstrim lainnya
5. **Komentar kode Anda** - Jelaskan logika yang digunakan
6. **Format output dengan rapi** - Gunakan template literal untuk string interpolation

---

## Kriteria Penilaian

| Aspek            | Bobot |
| ---------------- | ----- |
| Ketepatan Output | 40%   |
| Logika Program   | 30%   |
| Efisiensi Kode   | 15%   |
| Clean Code       | 10%   |
| Bonus Challenge  | 5%    |

---

**Selamat mengerjakan! 🚀**
