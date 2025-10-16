---
title: Struktur Kontrol (if, switch, loop)
version: 1.0.0
header: Struktur Kontrol (if, switch, loop)
footer: https://github.com/fast-ibbi/jumat-iii-p1
paginate: true
marp: true
---

<!--
_class: lead
_paginate: skip
-->

# Struktur Kontrol (if, switch, loop)

---

### **Pengantar Logika Program**

Struktur kontrol memungkinkan program untuk **membuat keputusan** dan **mengulang proses**. Tanpa struktur kontrol, program hanya akan berjalan secara linear dari atas ke bawah. Dengan struktur kontrol, kita dapat membuat program yang lebih pintar dan efisien.[2][1]

---

**Contoh Konsep:**

```javascript
// Program tanpa struktur kontrol
let nilai = 85;
console.log("Nilai Anda: " + nilai);

// Program dengan struktur kontrol
let nilaiMahasiswa = 85;
if (nilaiMahasiswa >= 75) {
  console.log("Selamat, Anda lulus!");
} else {
  console.log("Maaf, Anda belum lulus.");
}
```

---

### **Kategori Struktur Kontrol**

Struktur kontrol dibagi menjadi 2 kategori utama:

1. **Percabangan (Conditional Statements):** Memungkinkan program memilih jalur eksekusi berdasarkan kondisi tertentu
2. **Perulangan (Loops):** Memungkinkan program mengeksekusi blok kode berulang kali selama kondisi terpenuhi[1][2]

---

### **Percabangan (Conditional)**

Percabangan memungkinkan program mengambil keputusan berdasarkan **evaluasi kondisi**. Kondisi adalah ekspresi yang menghasilkan nilai `true` atau `false`. JavaScript menyediakan beberapa cara untuk melakukan percabangan.[2][1]

**Jenis Percabangan:**

- `if` statement
- `if...else` statement
- `if...else if...else` statement
- `switch` statement

---

### **Sintaks If Dasar**

Statement `if` adalah bentuk paling sederhana dari percabangan. Kode di dalam blok `if` hanya akan dijalankan **jika kondisi bernilai true**.[1][2]

---

**Sintaks:**

```javascript
if (kondisi) {
  // kode yang dijalankan jika kondisi benar
}
```

**Contoh:**

```javascript
let suhu = 35;

if (suhu > 30) {
  console.log("Cuaca sangat panas!");
}
// Output: Cuaca sangat panas!
```

---

### **If dan Else If**

Ketika ada **lebih dari dua kemungkinan hasil**, gunakan `else if` untuk menambahkan kondisi tambahan di antara `if` dan `else`.[1][2]

---

**Sintaks:**

```javascript
if (kondisi1) {
  // kode jika kondisi1 benar
} else if (kondisi2) {
  // kode jika kondisi1 salah dan kondisi2 benar
} else if (kondisi3) {
  // kode jika kondisi1 dan kondisi2 salah, kondisi3 benar
} else {
  // kode jika semua kondisi salah
}
```

---

**Contoh:**

```javascript
let nilai = 82;

if (nilai >= 85) {
  console.log("Grade: A");
} else if (nilai >= 75) {
  console.log("Grade: B");
} else if (nilai >= 65) {
  console.log("Grade: C");
} else {
  console.log("Grade: D");
}
// Output: Grade: B
```

---

### **Aturan Eksekusi If-Else If**

JavaScript mengevaluasi kondisi **dari atas ke bawah** dan **berhenti ketika menemukan kondisi yang benar**. Blok kode lainnya akan diabaikan setelah satu kondisi terpenuhi.[2][1]

---

**Contoh:**

```javascript
let angka = 20;

if (angka > 10) {
  console.log("Angka lebih besar dari 10");
} else if (angka > 15) {
  console.log("Angka lebih besar dari 15");
} else if (angka > 18) {
  console.log("Angka lebih besar dari 18");
}
// Output: Angka lebih besar dari 10
// (kondisi berikutnya tidak dievaluasi)
```

---

### **Switch Statement**

`switch` adalah alternatif untuk `if...else if...else` ketika kita perlu memeriksa **satu variabel terhadap banyak nilai tetap**. Statement ini lebih terstruktur dan mudah dibaca.[7][3]

---

### **Struktur Switch**

Switch mengevaluasi ekspresi sekali, lalu membandingkan hasilnya dengan nilai di setiap `case`. Jika cocok, blok kode tersebut dijalankan. Statement `break` menghentikan eksekusi, sementara `default` dijalankan jika tidak ada yang cocok.[3][7]

---

**Sintaks:**

```javascript
switch (ekspresi) {
  case nilai1:
    // kode
    break;
  case nilai2:
    // kode
    break;
  default:
  // jika tidak cocok
}
```

---

**Contoh:**

```javascript
let hari = 3;
let namaHari;

switch (hari) {
  case 1:
    namaHari = "Senin";
    break;
  case 2:
    namaHari = "Selasa";
    break;
  case 3:
    namaHari = "Rabu";
    break;
  ...
  default:
    namaHari = "Hari tidak valid";
}

console.log("Hari ini: " + namaHari);
// Output: Hari ini: Rabu
```

---

### **Kelebihan Switch**

Kelebihan menggunakan `switch` statement:[7][3]

1. **Lebih rapi dan mudah dibaca** dibanding banyak `if-else` berurutan
2. **Lebih efisien** untuk pembandingan nilai tetap
3. **Mudah di-maintain** ketika ada banyak kondisi
4. **Struktur lebih jelas** dengan case yang terorganisir

---

**Contoh Perbandingan:**

```javascript
// Menggunakan if-else (kurang rapi)
let menu = 2;
if (menu === 1) {
  console.log("Nasi Goreng");
} else if (menu === 2) {
  console.log("Mie Goreng");
} else if (menu === 3) {
  console.log("Ayam Goreng");
}
```

---

```javascript
// Menggunakan switch (lebih rapi)
switch (menu) {
  case 1:
    console.log("Nasi Goreng");
    break;
  case 2:
    console.log("Mie Goreng");
    break;
  case 3:
    console.log("Ayam Goreng");
    break;
}
```

---

**Contoh:**

```javascript
let kodeProdi = "TI";
let namaProdi;

switch (kodeProdi) {
  case "TI":
    namaProdi = "Teknik Informatika";
    break;
  case "SI":
    namaProdi = "Sistem Informasi";
    break;
  case "MI":
    namaProdi = "Manajemen Informatika";
    break;
  case "KA":
    namaProdi = "Komputerisasi Akuntansi";
    break;
  default:
    namaProdi = "Prodi tidak dikenali";
}

console.log("Program Studi: " + namaProdi);
// Output: Program Studi: Teknik Informatika
```

---

### **Perulangan (Loop)**

Perulangan (loop) adalah struktur kontrol yang memungkinkan **mengeksekusi blok kode berulang kali** selama kondisi tertentu terpenuhi. Loop menghemat waktu dan membuat kode lebih efisien.[8][4]

**Manfaat Loop:**

- Menghindari penulisan kode berulang (DRY principle)
- Memproses data dalam jumlah besar
- Iterasi melalui array atau koleksi data

---

### **Jenis Loop di JavaScript**

JavaScript menyediakan beberapa jenis loop:[4][8]

1. **for** - digunakan ketika jumlah iterasi sudah diketahui
2. **while** - digunakan ketika iterasi bergantung pada kondisi
3. **do...while** - mirip while, tapi minimal dijalankan 1 kali
4. **for...of** - untuk iterasi array dan iterable objects (modern)
5. **for...in** - untuk iterasi properti objek (modern)

---

### **Konsep Dasar Loop**

Setiap loop terdiri dari 3 komponen utama:[8][4]

1. **Initialization (Inisialisasi):** Titik awal loop, biasanya variabel counter
2. **Condition (Kondisi):** Ekspresi boolean yang menentukan apakah loop berlanjut
3. **Increment/Decrement (Perubahan):** Mengubah nilai variabel setiap iterasi

---

**Contoh Konsep:**

```javascript
// Komponen loop
// 1. Initialization: let i = 0
// 2. Condition: i < 5
// 3. Increment: i++

for (let i = 0; i < 5; i++) {
  console.log("Iterasi ke-" + i);
}
```

---

### **Struktur Loop For**

Loop `for` adalah loop yang paling umum digunakan. Ketiga komponen (initialization, condition, increment) ditulis dalam satu baris.[4][8]

**Sintaks:**

```javascript
for (inisialisasi; kondisi; perubahan) {
  // kode yang diulang
}
```

---

**Contoh:**

```javascript
// Mencetak angka 1 sampai 5
for (let i = 1; i <= 5; i++) {
  console.log("Angka: " + i);
}
// Output:
// Angka: 1
// Angka: 2
// Angka: 3
// Angka: 4
// Angka: 5

// Menghitung jumlah deret
let jumlah = 0;
for (let i = 1; i <= 10; i++) {
  jumlah += i;
}
console.log("Jumlah 1-10: " + jumlah);
// Output: Jumlah 1-10: 55
```

---

### **Loop While**

Loop `while` menjalankan kode **selama kondisi bernilai true**. Kondisi diperiksa **sebelum** setiap iterasi. Jika kondisi false sejak awal, loop tidak akan pernah dijalankan.[9][4]

**Sintaks:**

```javascript
while (kondisi) {
  // kode
}
```

---

**Contoh:**

```javascript
let i = 1;

while (i <= 5) {
  console.log("Hitungan: " + i);
  i++;
}
// Output:
// Hitungan: 1
// Hitungan: 2
// Hitungan: 3
// Hitungan: 4
// Hitungan: 5

// Contoh: Input sampai user memasukkan angka negatif
let angka = 0;
let total = 0;

while (angka >= 0) {
  total += angka;
  // Misalkan user input (dalam praktik gunakan prompt)
  angka = parseInt(prompt("Masukkan angka (negatif untuk stop):"));
}
console.log("Total: " + total);
```

---

### **Loop Do...While**

Loop `do...while` mirip dengan `while`, tetapi kondisi diperiksa **setelah eksekusi pertama**. Artinya, kode **pasti dijalankan minimal 1 kali** meskipun kondisi false.[9][4]

**Sintaks:**

```javascript
do {
  // kode
} while (kondisi);
```

---

**Contoh:**

```javascript
let counter = 1;

do {
  console.log("Counter: " + counter);
  counter++;
} while (counter <= 5);
// Output:
// Counter: 1
// Counter: 2
// Counter: 3
// Counter: 4
// Counter: 5

// Contoh: Pasti dijalankan minimal 1x
let angka = 10;
do {
  console.log("Angka: " + angka);
  angka++;
} while (angka < 5);
// Output: Angka: 10
// (meskipun kondisi false, tetap jalan 1x)
```

---

### **Perbedaan While vs Do...While**

Perbedaan utama antara `while` dan `do...while`:[9][4]

| Aspek            | `while`                             | `do...while`                  |
| ---------------- | ----------------------------------- | ----------------------------- |
| Evaluasi kondisi | Sebelum eksekusi                    | Setelah eksekusi              |
| Eksekusi minimal | 0 kali (jika kondisi false)         | 1 kali (pasti)                |
| Penggunaan       | Ketika tidak yakin perlu dijalankan | Ketika harus jalan minimal 1x |

---

**Contoh Perbandingan:**

```javascript
// WHILE: bisa 0 kali
let x = 10;
while (x < 5) {
  console.log("While: " + x);
  x++;
}
// Output: (tidak ada output)

// DO-WHILE: minimal 1 kali
let y = 10;
do {
  console.log("Do-While: " + y);
  y++;
} while (y < 5);
// Output: Do-While: 10
```

---

### **Infinite Loop (Waspada)**

**Infinite loop** terjadi ketika kondisi **tidak pernah menjadi false**, sehingga loop berjalan terus-menerus dan program hang/crash. Pastikan selalu ada mekanisme penghentian.[4][8]

---

**Contoh SALAH (Infinite Loop):**

```javascript
// JANGAN LAKUKAN INI!
let i = 0;
while (i < 10) {
  console.log(i);
  // LUPA increment i++
  // Loop tidak akan pernah berhenti!
}

// JANGAN LAKUKAN INI!
for (let j = 0; j < 10; ) {
  console.log(j);
  // LUPA j++
}
```

---

**Contoh BENAR:**

```javascript
// BENAR
let i = 0;
while (i < 10) {
  console.log(i);
  i++; // Ada increment
}

// BENAR dengan safety mechanism
let counter = 0;
while (true) {
  console.log(counter);
  counter++;
  if (counter >= 10) break; // Ada break untuk keluar
}
```

---

### **Break dan Continue**

JavaScript menyediakan 2 keyword untuk mengontrol alur loop:[10][11]

1. **break:** Menghentikan loop **sepenuhnya** dan keluar dari loop
2. **continue:** Melewati iterasi saat ini dan **langsung ke iterasi berikutnya**

**Contoh Break:**

```javascript
for (let i = 1; i <= 10; i++) {
  if (i === 5) {
    break; // Stop di angka 5
  }
  console.log(i);
}
// Output: 1, 2, 3, 4
```

---

**Contoh Continue:**

```javascript
for (let i = 1; i <= 10; i++) {
  if (i % 2 === 0) {
    continue; // Skip angka genap
  }
  console.log(i);
}
// Output: 1, 3, 5, 7, 9
```

---

### **For...of Loop**

`for...of` adalah cara modern (ES6) untuk **iterasi array dan iterable objects**. Lebih sederhana dan mudah dibaca dibanding `for` tradisional.[12][5]

**Sintaks:**

```javascript
for (const item of iterable) {
  // kode
}
```

---

**Contoh:**

```javascript
// Iterasi array
const buah = ["Apel", "Jeruk", "Mangga", "Pisang"];

for (const item of buah) {
  console.log(item);
}
// Output:
// Apel
// Jeruk
// Mangga
// Pisang
```

---

```javascript
// Iterasi string
const kata = "JavaScript";
for (const huruf of kata) {
  console.log(huruf);
}
// Output: J, a, v, a, S, c, r, i, p, t (satu per satu)
```

---

```javascript
// Dengan index (jika diperlukan)
const warna = ["Merah", "Hijau", "Biru"];
let index = 0;
for (const w of warna) {
  console.log(`${index}: ${w}`);
  index++;
}
// Output:
// 0: Merah
// 1: Hijau
// 2: Biru
```

---

### **For...in Loop**

`for...in` digunakan untuk **iterasi properti/key objek**. Berbeda dengan `for...of` yang iterasi nilai, `for...in` iterasi nama properti (key).[6][13]

**Sintaks:**

```javascript
for (const key in object) {
  // kode
}
```

---

**Contoh:**

```javascript
// Iterasi properti objek
const mahasiswa = {
  nama: "Budi Santoso",
  nim: "12345678",
  jurusan: "Teknik Informatika",
  semester: 3,
};
```

---

```javascript
for (const key in mahasiswa) {
  console.log(`${key}: ${mahasiswa[key]}`);
}
// Output:
// nama: Budi Santoso
// nim: 12345678
// jurusan: Teknik Informatika
// semester: 3
```

---

```javascript
// Contoh lain
const nilai = {
  matematika: 85,
  fisika: 78,
  kimia: 92,
};

let totalNilai = 0;
let jumlahMataKuliah = 0;

for (const mk in nilai) {
  console.log(`Nilai ${mk}: ${nilai[mk]}`);
  totalNilai += nilai[mk];
  jumlahMataKuliah++;
}

let rataRata = totalNilai / jumlahMataKuliah;
console.log(`Rata-rata: ${rataRata.toFixed(2)}`);
// Output:
// Nilai matematika: 85
// Nilai fisika: 78
// Nilai kimia: 92
// Rata-rata: 85.00
```

**Catatan Penting:**
`for...in` **tidak direkomendasikan untuk array**, gunakan `for...of` untuk array.[13][6]

---

## Quiz - Struktur Kontrol

---

### **Soal 1**

Apa output dari kode berikut?

```javascript
let nilai = 80;
if (nilai >= 75) {
  console.log("Lulus");
}
console.log("Selesai");
```

**A.** Lulus  
**B.** Selesai  
**C.** Lulus<br>Selesai  
**D.** Tidak ada output

---

### **Soal 2**

Manakah pernyataan yang BENAR tentang switch statement?

**A.** Switch dapat digunakan untuk kondisi range seperti `x > 10`  
**B.** Switch hanya membandingkan nilai dengan operator `===`  
**C.** Switch tidak memerlukan statement `break`  
**D.** Switch lebih lambat dibanding if-else

---

### **Soal 3**

Apa yang akan terjadi jika `break` tidak ditambahkan dalam case switch?

**A.** Program akan error  
**B.** Terjadi fall-through ke case berikutnya  
**C.** Loop akan berhenti otomatis  
**D.** Tidak ada pengaruh

---

### **Soal 4**

Berapa kali kode di dalam loop akan dijalankan?

```javascript
for (let i = 0; i < 5; i++) {
  console.log(i);
}
```

**A.** 4 kali  
**B.** 5 kali  
**C.** 6 kali  
**D.** Infinite loop

---

### **Soal 5**

Apa perbedaan utama antara `while` dan `do...while`?

**A.** `while` lebih cepat dari `do...while`  
**B.** `do...while` pasti dijalankan minimal 1 kali  
**C.** `while` tidak bisa menggunakan kondisi boolean  
**D.** `do...while` hanya untuk array

---

### **Soal 6**

Apa output dari kode berikut?

```javascript
let x = 10;
while (x < 5) {
  console.log(x);
  x++;
}
console.log("Done");
```

**A.** 10<br>Done  
**B.** Done  
**C.** 10 11 12 13 14<br>Done  
**D.** Infinite loop

---

### **Soal 7**

Apa fungsi dari keyword `continue` dalam loop?

**A.** Menghentikan loop sepenuhnya  
**B.** Melewati iterasi saat ini dan lanjut ke iterasi berikutnya  
**C.** Mengulang loop dari awal  
**D.** Keluar dari program

---

### **Soal 8**

Loop mana yang PALING TEPAT untuk iterasi array di JavaScript modern?

**A.** `for` tradisional  
**B.** `while`  
**C.** `for...of`  
**D.** `for...in`

---

### **Soal 9**

Apa output dari kode berikut?

```javascript
for (let i = 1; i <= 5; i++) {
  if (i === 3) {
    break;
  }
  console.log(i);
}
```

**A.** 1 2 3 4 5  
**B.** 1 2 3  
**C.** 1 2  
**D.** 1 2 4 5

---

### **Soal 10**

Kapan sebaiknya menggunakan nested if dibanding else if?

**A.** Ketika ada kondisi bertingkat yang perlu diperiksa secara berurutan  
**B.** Ketika semua kondisi setara dan saling eksklusif  
**C.** Nested if selalu lebih baik dari else if  
**D.** Tidak ada perbedaan keduanya sama saja
