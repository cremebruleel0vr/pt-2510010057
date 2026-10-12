# P04 Percabangan: if, if-else, switch, dan Operator Logika

Folder kode Pertemuan 4 Pemrograman Terstruktur. Setiap program di sini punya flowchart pasangannya
di modul (Gambar 2 sampai 7); baca gambarnya dulu, baru kodenya.

## Isi

| Berkas                   | Kegunaan                                                                              |
| ------------------------ | ------------------------------------------------------------------------------------- | --- | ------------------------------------------- |
| `if_dasar.cpp`           | if satu cabang: peringatan bila nilai di bawah 60                                     |
| `if_else.cpp`            | if-else: lulus atau belum lulus                                                       |
| `bertingkat.cpp`         | if-else bertingkat tiga syarat; coba tukar urutannya                                  |
| `logika.cpp`             | `&&`, `                                                                               |     | `, `!` dengan bool bernama; syarat ikut UAS |
| `switch_menu.cpp`        | switch dengan break dan default; coba hapus break-nya                                 |
| `sinilai_v03_awal.cpp`   | Starter SiNilai v0.3: bagian v0.2 sudah jadi, lengkapi huruf mutu, status, keterangan |
| `contoh_masukan.txt`     | Masukan uji yang sama dengan pertemuan sebelumnya                                     |
| `.vscode/`, `.gitignore` | Sama dengan pertemuan sebelumnya                                                      |

## Kasus uji SiNilai v0.3

| Empat komponen     | Nilai akhir | Huruf | Keterangan    | Status      |
| ------------------ | ----------- | ----- | ------------- | ----------- |
| contoh_masukan.txt | 83.975      | A     | Sangat baik   | Lulus       |
| 80 x4              | 80          | A     | Sangat baik   | Lulus       |
| 79.9 x4            | 79.9        | B+    | Baik          | Lulus       |
| 60 x4              | 60          | C     | Cukup         | Lulus       |
| 59.9 x4            | 59.9        | D     | Kurang        | Belum lulus |
| 30 x4              | 30          | E     | Sangat kurang | Belum lulus |

## Yang dikumpulkan mahasiswa

Folder `p04` di repository `pt-NPM` berisi `sinilai_v03.cpp` dan `README.md`. Lihat Modul Pertemuan 4 bagian E.

## Deklarasi AI

AI yang digunakan: GitHub Copilot.

Prompt: "Bagaimana `switch` pada karakter pertama `huruf_mutu` dapat memilih keterangan yang sesuai untuk nilai seperti B+ dan C+?"

Umpan balik AI: Baca `huruf_mutu[0]` lalu sediakan `case` untuk A, B, C, dan D; `default` dapat menangani E. Karena B+ diawali B dan C+ diawali C, keterangan untuk kelompoknya tetap tepat. Gunakan `break` agar tiap kasus tidak jatuh ke kasus berikutnya.
