# P05 Perulangan: for, while, dan do-while

Pertemuan kelima mempelajari perulangan dengan jumlah putaran tertentu maupun kondisi berhenti. Gunakan flowchart yang ada di modul (Gambar 1–5) untuk mengikuti alur setiap latihan.

## Berkas latihan

| Berkas                   | Isi                                                                                                  |
| ------------------------ | ---------------------------------------------------------------------------------------------------- |
| `for_hitung.cpp`         | Perulangan `for` dengan batas yang diketahui; coba ubah `<=` menjadi `<`                             |
| `for_jumlah.cpp`         | Akumulator untuk menghitung total dan rata-rata dari sekumpulan nilai; uji juga saat jumlah data nol |
| `while_sentinel.cpp`     | `while` yang berakhir ketika menerima angka negatif sebagai sentinel                                 |
| `do_while_menu.cpp`      | Menu yang terus ditampilkan sampai pengguna memilih keluar; menggunakan `switch`                     |
| `sinilai_v04_awal.cpp`   | Kerangka SiNilai v0.4 untuk validasi jumlah mahasiswa, pemrosesan berulang, akumulator, dan rekap    |
| `contoh_masukan.txt`     | Tiga mahasiswa sebagai data uji                                                                      |
| `.vscode/`, `.gitignore` | Pengaturan VS Code dan berkas yang diabaikan seperti sebelumnya                                      |

## Data pembanding v0.4

Periksa dengan `./sinilai_v04 < contoh_masukan.txt`.

| Nama         | Komponen: kehadiran, mingguan, UTS, UAS | Nilai akhir | Huruf | Status      |
| ------------ | --------------------------------------- | ----------: | ----- | ----------- |
| Siti Aminah  | 100, 85.5, 78, 80                       |      83.975 | A     | Lulus       |
| Budi Santoso | 80, 70, 65, 60                          |       67.75 | C+    | Lulus       |
| Rina Wati    | 60, 50, 40, 55                          |        49.5 | D     | Belum lulus |

Rekap yang diharapkan: 3 mahasiswa, 2 lulus, 1 belum lulus, dan rata-rata kelas 67.075. Jumlah mahasiswa yang kurang dari satu perlu diminta ulang dengan `do-while`.

## Jika loop terus berjalan

Tekan `Ctrl+C` untuk menghentikan program. Selanjutnya periksa apakah variabel penghitung berubah dan apakah kondisi loop akhirnya dapat menjadi salah. Input huruf saat program meminta angka juga dapat membuat `cin` gagal; cara pemulihannya dibahas pada P07.

## Pengumpulan

Kumpulkan berkas `sinilai_v04.cpp` dalam folder `p05` di repositori `pt-NPM`. Lihat Modul Pertemuan 5 bagian E.

## Deklarasi AI

AI yang digunakan: GitHub Copilot.

Prompt: "Bagaimana memperbarui `total_nilai` dan `jumlah_lulus` selama loop mahasiswa agar rekap kelas v0.4 akurat?"

Umpan balik AI: Tambahkan setiap `nilai_akhir` ke `total_nilai` pada setiap iterasi. Tambah `jumlah_lulus` hanya jika mahasiswa memenuhi syarat kelulusan. Sesudah loop, bagi total nilai dengan jumlah mahasiswa untuk mendapatkan rata-rata kelas.
