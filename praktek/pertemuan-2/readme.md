## Soal 1: Deklarasi Variabel

Buatlah file `soal1.js` dan deklarasikan variabel-variabel berikut:

- Gunakan `let` untuk menyimpan nama lengkap Anda
- Gunakan `const` untuk menyimpan tahun lahir Anda
- Gunakan `let` untuk menyimpan hobi favorit Anda

Tampilkan semua variabel tersebut ke console menggunakan `console.log()`.

**Contoh Output:**

```
Nama: Ahmad Fauzi
Tahun Lahir: 2005
Hobi: Membaca
```

---

## Soal 2: Perbedaan var, let, dan const

Buatlah file `soal2.js` dan coba praktekan perbedaan `var`, `let`, dan `const`:

1. Buat variabel dengan `let` bernama `nilai` isi dengan 80, lalu ubah menjadi 90
2. Buat variabel dengan `const` bernama `namaSekolah` isi dengan nama sekolah Anda
3. Coba ubah nilai `namaSekolah` (perhatikan apa yang terjadi!)
4. Buat variabel dengan `var` bernama `kelas` isi dengan "XII RPL"

Amati dan catat perbedaannya!

---

## Soal 3: Tipe Data String dan Number

Buatlah file `soal3.js` untuk menghitung dan menampilkan:

1. Buat variabel `namaProduk` (string) dengan nilai "Laptop Gaming"
2. Buat variabel `harga` (number) dengan nilai 15000000
3. Buat variabel `diskon` (number) dengan nilai 10 (persen)
4. Hitung harga setelah diskon
5. Tampilkan hasil dengan format: "Produk [nama] seharga Rp [harga setelah diskon]"

**Contoh Output:**

```
Produk Laptop Gaming seharga Rp 13500000
```

---

## Soal 4: Tipe Data Boolean

Buatlah file `soal4.js` yang berisi:

1. Buat variabel `umur` dengan nilai umur Anda
2. Buat variabel `sudahDewasa` (boolean) yang berisi hasil perbandingan apakah umur >= 17
3. Buat variabel `punyaSIM` (boolean) dengan nilai sesuai kondisi Anda
4. Tampilkan semua variabel tersebut

**Contoh Output:**

```
Umur: 18
Sudah Dewasa: true
Punya SIM: false
```

---

## Soal 5: Object dan Array

Buatlah file `soal5.js` dengan struktur data berikut:

1. Buat object `mahasiswa` dengan properti:
   - nama (string)
   - nim (string)
   - jurusan (string)
   - semester (number)
2. Buat array `mataKuliah` berisi minimal 5 nama mata kuliah
3. Tampilkan nama mahasiswa dan daftar mata kuliah

**Contoh Output:**

```
Nama: Siti Aminah
NIM: 2023010123
Jurusan: Teknik Informatika
Mata Kuliah:
- Algoritma Pemrograman
- Basis Data
- Pemrograman Web
- Jaringan Komputer
- Matematika Diskrit
```

---

## Soal 6: Operator Arithmetic

Buatlah file `soal6.js` untuk kalkulator sederhana:

1. Buat variabel `angka1` dengan nilai 25
2. Buat variabel `angka2` dengan nilai 7
3. Hitung dan tampilkan:
   - Penjumlahan
   - Pengurangan
   - Perkalian
   - Pembagian
   - Sisa bagi (modulus)

**Contoh Output:**

```
25 + 7 = 32
25 - 7 = 18
25 * 7 = 175
25 / 7 = 3.571428571428571
25 % 7 = 4
```

---

## Soal 7: Operator Comparison

Buatlah file `soal7.js` untuk membandingkan nilai:

1. Buat variabel `nilaiUjian` dengan nilai 85
2. Buat variabel `nilaiMinimal` dengan nilai 75
3. Bandingkan dan tampilkan:
   - Apakah nilaiUjian > nilaiMinimal?
   - Apakah nilaiUjian >= 80?
   - Apakah nilaiUjian === 85?
   - Apakah nilaiUjian == "85"?
   - Apakah nilaiUjian === "85"?

**Contoh Output:**

```
Nilai Ujian > Nilai Minimal: true
Nilai Ujian >= 80: true
Nilai Ujian === 85: true
Nilai Ujian == "85": true
Nilai Ujian === "85": false
```

---

## Soal 8: Operator Logical

Buatlah file `soal8.js` untuk menentukan status kelulusan:

1. Buat variabel `nilaiTugas` = 80
2. Buat variabel `nilaiUTS` = 75
3. Buat variabel `nilaiUAS` = 85
4. Buat variabel `kehadiran` = 90 (persen)
5. Tentukan status lulus jika:
   - Semua nilai >= 70 DAN kehadiran >= 75
6. Gunakan operator logical `&&` untuk mengecek
7. Tampilkan hasilnya

**Contoh Output:**

```
Nilai Tugas: 80
Nilai UTS: 75
Nilai UAS: 85
Kehadiran: 90%
Status Lulus: true
```

---

## Soal 9: Operator Ternary

Buatlah file `soal9.js` untuk menentukan grade nilai:

1. Buat variabel `nilai` dengan nilai antara 0-100
2. Gunakan operator ternary untuk menentukan grade:
   - > = 85: "A"
   - > = 70: "B"
   - > = 60: "C"
   - < 60: "D"
3. Tampilkan nilai dan grade

**Petunjuk:** Gunakan nested ternary operator

**Contoh Output:**

```
Nilai: 87
Grade: A
```

---

## Soal 10: Program Gabungan

Buatlah file `soal10.js` untuk sistem data siswa lengkap:

1. Buat object `siswa` berisi:
   - nama (string)
   - kelas (string)
   - nilaiMatematika (number)
   - nilaiFisika (number)
   - nilaiKimia (number)
2. Hitung rata-rata nilai
3. Tentukan status kelulusan (rata-rata >= 70)
4. Tentukan predikat menggunakan ternary:
   - > = 85: "Sangat Baik"
   - > = 70: "Baik"
   - > = 60: "Cukup"
   - < 60: "Kurang"
5. Tampilkan semua informasi dengan format yang rapi

**Contoh Output:**

```
=== Data Siswa ===
Nama: Rizki Pratama
Kelas: XII RPL 1

=== Nilai ===
Matematika: 85
Fisika: 78
Kimia: 90

=== Hasil ===
Rata-rata: 84.33
Status: Lulus
Predikat: Baik
```

---

## Panduan Pengerjaan

1. Buat file JavaScript untuk setiap soal (soal1.js, soal2.js, dst.)
2. Simpan semua file di folder `praktek/pertemuan-2/`
3. Jalankan setiap file dengan perintah: `node namafile.js`
4. Pastikan output sesuai dengan contoh yang diberikan
5. Jika ada error, perbaiki dan jalankan ulang

## Tips Pengerjaan

- Gunakan `console.log()` untuk menampilkan output
- Perhatikan perbedaan `==` dan `===`
- Gunakan template literal (backtick) untuk format string yang kompleks: `` `Nama: ${nama}` ``
- Test setiap kode sebelum melanjutkan ke soal berikutnya

---

**Selamat Mengerjakan!** 🚀
