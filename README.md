# Pertemuan 03 Seleksi Python

**Nama:** Aulia Nurrizqi
**NIM:** 2225250160
**Kelas:** 3A

## Tujuan

Mempelajari dan menerapkan struktur seleksi dalam Python, yaitu `if`, `if-else`, kondisi majemuk, dan `nested if`. Program dibuat dan diuji menggunakan Visual Studio Code, kemudian dikumpulkan melalui GitHub.

## Struktur Folder

```text
pertemuan-03-seleksi-NIM/
├── README.md
├── .gitignore
├── latihan/
│   ├── 01_genap_ganjil.py
│   ├── 02_bandingkan_dua_bilangan.py
│   ├── 03_kelulusan_bersyarat.py
│   └── 04_jenis_segitiga.py
└── tugas/
    └── analisis_persamaan_kuadrat.py
```

## Latihan

### 1. Genap atau Ganjil

Program menerima sebuah bilangan bulat. Jika bilangan habis dibagi 2, maka program menampilkan bahwa bilangan tersebut genap. Jika tidak, program menampilkan bahwa bilangan tersebut ganjil.

**Algoritma:**

1. Masukkan bilangan bulat.
2. Hitung sisa pembagian bilangan dengan 2.
3. Jika sisa pembagian sama dengan 0, tampilkan "Genap".
4. Jika tidak, tampilkan "Ganjil".

### 2. Membandingkan Dua Bilangan

Program menerima dua bilangan dan membandingkan keduanya menggunakan `nested if`.

**Algoritma:**

1. Masukkan bilangan pertama dan kedua.
2. Periksa apakah bilangan pertama lebih besar atau sama dengan bilangan kedua.
3. Jika sama, tampilkan bahwa kedua bilangan sama.
4. Jika tidak sama, tampilkan bahwa bilangan pertama lebih besar.
5. Jika kondisi pertama tidak terpenuhi, tampilkan bahwa bilangan pertama lebih kecil.

### 3. Kelulusan Bersyarat

Mahasiswa dinyatakan lulus jika nilai akhir minimal 60 dan kehadiran minimal 80%.

**Algoritma:**

1. Masukkan nilai akhir.
2. Masukkan persentase kehadiran.
3. Periksa kondisi `nilai >= 60 and kehadiran >= 80`.
4. Jika kedua kondisi terpenuhi, tampilkan "Lulus".
5. Jika salah satu kondisi tidak terpenuhi, tampilkan "Belum lulus".

### 4. Jenis Segitiga

Program menerima tiga panjang sisi dan menentukan jenis segitiga menggunakan kondisi majemuk dan `nested if`.

**Algoritma:**

1. Masukkan panjang sisi a, b, dan c.
2. Periksa apakah ketiga sisi dapat membentuk segitiga.
3. Jika valid, periksa apakah ketiga sisi sama.
4. Jika ketiga sisi sama, tampilkan "Segitiga sama sisi".
5. Jika ada dua sisi yang sama, tampilkan "Segitiga sama kaki".
6. Jika semua sisi berbeda, tampilkan "Segitiga sembarang".
7. Jika tidak memenuhi syarat segitiga, tampilkan bahwa ketiga sisi tidak membentuk segitiga.

## Tugas 2: Analisis Persamaan Kuadrat

Program digunakan untuk menganalisis persamaan kuadrat:

**ax² + bx + c = 0**

Jenis akar ditentukan berdasarkan nilai diskriminan:

**D = b² - 4ac**

### Algoritma

1. Masukkan nilai koefisien `a`, `b`, dan `c`.
2. Periksa apakah `a = 0`.
3. Jika `a = 0`, tampilkan bahwa input bukan persamaan kuadrat.
4. Jika `a ≠ 0`, hitung diskriminan dengan rumus `D = b² - 4ac`.
5. Jika `D > 0`, hitung dan tampilkan dua akar real yang berbeda.
6. Jika `D = 0`, hitung dan tampilkan satu akar real kembar.
7. Jika `D < 0`, tampilkan bahwa tidak ada akar real.
8. Tampilkan hasil numerik dengan dua angka di belakang koma.

## Cara Menjalankan

Pastikan Python 3 sudah terpasang dan interpreter Python sudah dipilih di Visual Studio Code.

Untuk menjalankan tugas utama, buka terminal pada folder utama proyek lalu gunakan perintah:

```bash
python tugas/analisis_persamaan_kuadrat.py
```

Jika menggunakan `python3`, gunakan:

```bash
python3 tugas/analisis_persamaan_kuadrat.py
```

## Hasil Pengujian

| No | Input (a, b, c) | Diskriminan | Hasil yang Diharapkan   | Status   |
| -- | --------------- | ----------: | ----------------------- | -------- |
| 1  | (1, -5, 6)      |           1 | Dua akar real: 3 dan 2  | Berhasil |
| 2  | (1, 2, 1)       |           0 | Akar real kembar: -1    | Berhasil |
| 3  | (1, 0, 1)       |          -4 | Tidak ada akar real     | Berhasil |
| 4  | (0, 2, 3)       |           - | Bukan persamaan kuadrat | Berhasil |

### Penjelasan Hasil Pengujian

* Pada input `(1, -5, 6)`, diskriminan bernilai 1 sehingga menghasilkan dua akar real yang berbeda, yaitu 3 dan 2.
* Pada input `(1, 2, 1)`, diskriminan bernilai 0 sehingga menghasilkan akar real kembar, yaitu -1.
* Pada input `(1, 0, 1)`, diskriminan bernilai -4 sehingga tidak memiliki akar real.
* Pada input `(0, 2, 3)`, nilai `a` sama dengan 0 sehingga bukan merupakan persamaan kuadrat.

## Refleksi

Dalam pengerjaan tugas ini, saya mempelajari penggunaan struktur `if`, `if-else`, kondisi majemuk, dan `nested if` dalam Python. Saya juga memahami bahwa pengujian perlu dilakukan pada setiap cabang kondisi, termasuk nilai batas.

Salah satu kesalahan logika yang perlu diperhatikan adalah penggunaan kondisi yang tidak sesuai dengan aturan. Pada persamaan kuadrat, pemeriksaan `a == 0` harus dilakukan terlebih dahulu sebelum menghitung diskriminan dan akar karena jika `a = 0`, bentuk tersebut bukan persamaan kuadrat.

Melalui tugas ini, saya juga belajar menjalankan program menggunakan Visual Studio Code serta mengunggah hasil pekerjaan ke GitHub menggunakan Git.

## Kesimpulan

Struktur seleksi dalam Python dapat digunakan untuk membuat program mengambil keputusan berdasarkan kondisi tertentu. Penggunaan `if`, `if-else`, kondisi majemuk, dan `nested if` memungkinkan program menangani berbagai kemungkinan input. Pengujian dengan beberapa test case membantu memastikan setiap kondisi dan hasil program berjalan dengan benar.

## Sumber dan Bantuan

* Bahan Ajar Algoritma dan Pemrograman Pertemuan 03, Program Studi S1 Pendidikan Matematika FKIP Untirta.
* Python Documentation.
* Visual Studio Code Documentation.
* GitHub Documentation.
* Bantuan ChatGPT digunakan untuk membantu memahami konsep dan penyusunan dokumentasi tugas.
