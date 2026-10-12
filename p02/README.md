# P02 Tipe Data, Konstanta, dan Input

Pertemuan ini mengenalkan tipe data dasar, konstanta, serta cara membaca masukan pengguna. Buka folder `p02` di VS Code agar konfigurasi lokal `.vscode` dapat digunakan.

## Isi folder

| Berkas                   | Keterangan                                                                                                     |
| ------------------------ | -------------------------------------------------------------------------------------------------------------- |
| `tipe_dasar.cpp`         | Contoh `int`, `double`, `char`, `bool`, dan `string`; mulai materi ini kode menggunakan `using namespace std;` |
| `konstanta.cpp`          | Penggunaan `const` untuk bobot nilai; ada nilai yang dapat dicoba diubah                                       |
| `input_dasar.cpp`        | Membaca data menggunakan `cin`; uji nama satu kata dan nama yang terdiri dari dua kata                         |
| `sinilai_v01_awal.cpp`   | Kerangka program SiNilai v0.1 untuk membaca data dan mencetak kartu mahasiswa                                  |
| `contoh_masukan.txt`     | Data contoh untuk pengujian lewat `./sinilai_v01 < contoh_masukan.txt`                                         |
| `.vscode/`, `.gitignore` | Pengaturan editor/build dan pengecualian berkas hasil kompilasi dari pertemuan sebelumnya                      |

## Keluaran yang diharapkan

```text
=== SiNilai v0.1 ===
Nama      : Siti Aminah
NPM       : 2024010101
Kehadiran : 100
Mingguan  : 85.5
UTS       : 78
UAS       : 80

--- Kartu Data Mahasiswa ---
Nama      : Siti Aminah
NPM       : 2024010101
Kehadiran : 100
Mingguan  : 85.5
UTS       : 78
UAS       : 80
```

## Pengumpulan

Kumpulkan `sinilai_v01.cpp` dan `README.md` di folder `p02` repositori `pt-NPM`. Lihat Modul Pertemuan 2 bagian E.

## Deklarasi AI

AI yang digunakan: GitHub Copilot.

Prompt: "Pada SiNilai v0.1, kapan sebaiknya memakai `getline` untuk membaca nama dan mengapa NPM lebih tepat disimpan sebagai `string`?"

Umpan balik AI: `getline` membaca seluruh baris termasuk spasi, sehingga cocok untuk nama lengkap. NPM merupakan identitas, bukan nilai untuk operasi hitung, dan penggunaan `string` mempertahankan angka nol di depan. Saya mencobanya dengan nama dua kata dan NPM yang diawali nol.
