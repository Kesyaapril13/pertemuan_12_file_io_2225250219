
# Pertemuan 12 - File I/O dan Error Handling

**Nama:** Kesya Nur Aprilliani  
**NIM:** 2225250219  
**Kelas:** 3E  
**Program Studi:** Pendidikan Matematika  
**Mata Kuliah:** Algoritma dan Pemrograman

## 1. Tujuan

Mempelajari cara membaca, menulis, menambahkan, dan mengolah data menggunakan file teks Python. Program juga menerapkan penanganan error dasar agar tetap memberikan pesan yang jelas ketika terjadi kesalahan.

## 2. Struktur Proyek

- `data/`: menyimpan file input dan output.
- `latihan/`: menyimpan enam program latihan.
- `tugas/`: menyimpan program rekap nilai.
- `README.md`: dokumentasi proyek.
- `.gitignore`: menentukan file yang tidak disertakan dalam Git.

## 3. Format File Input

File `data/nilai.txt` menggunakan format:

NIM,nilai

Contoh:

```text
A001,85
A002,78
A003,92
A004,abc
A005,74
A006,88
```

Setiap baris berisi NIM dan nilai yang dipisahkan dengan koma.

## 4. Cara Menjalankan

Jalankan terminal dari folder utama proyek.

```bash
python latihan/01_tulis_file.py
python latihan/02_baca_file.py
python latihan/03_append_file.py
python latihan/04_proses_baris.py
python latihan/05_file_not_found.py
python latihan/06_value_error.py
python tugas/rekap_nilai_file.py
```

## 5. Error yang Ditangani

- `FileNotFoundError`: terjadi ketika file yang dibaca tidak tersedia.
- `ValueError`: terjadi ketika nilai tidak dapat dikonversi ke angka atau format record tidak sesuai.

Program melewati baris yang tidak valid agar data lainnya tetap dapat diproses.

## 6. Test Case

| Kondisi | Hasil yang Diharapkan |
|---|---|
| Data valid | Data dibaca dan dihitung |
| File hilang | Pesan kesalahan ditampilkan |
| Nilai tidak valid | Baris dilewati |
| Baris kosong | Baris diabaikan |
| Nilai 60 | Dihitung sebagai lulus |

Hasil aktual dan status pengujian dilengkapi setelah program dijalankan.

## 7. Kesimpulan

File I/O memungkinkan data disimpan dan dibaca kembali setelah program selesai. Penggunaan `with`, mode file yang tepat, validasi data, dan `try-except` membantu membuat program lebih terstruktur dan mampu menangani kesalahan dasar.

## 8. Refleksi

Kesalahan yang ditemukan pada latihan ini adalah nilai berbentuk teks yang tidak dapat dikonversi menjadi angka. Kesalahan tersebut ditangani menggunakan `ValueError`, sehingga baris yang bermasalah dapat dilewati dan data valid lainnya tetap diproses.

## 9. Sumber dan Bantuan

- Bahan Ajar Pertemuan 12: File Input-Output dan Penanganan Error Dasar, Algoritma dan Pemrograman, Universitas Sultan Ageng Tirtayasa, 2026/2027 Ganjil.
- Dokumentasi Python mengenai pembacaan file dan penanganan exception.
- Bantuan AI digunakan untuk membantu penyusunan dan penjelasan kode. Kode perlu diuji dan dipahami kembali oleh mahasiswa.
