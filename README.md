Nama: Muhamad Fahri Hidayat

NPM: 4525210041

Program Studi: Teknik Informatika

Fakultas: Teknik

Mata Kuliah: Praktikum Basis Data B

Dosen Pengampu: Prof. Dr. Dra. Andiani, M.Kom.

Tahun Akademik: 2026/2027

📚 Ringkasan Materi & Implementasi

Praktikum ini membahas eksekusi perintah SQL melalui CLI (Command Line Interface / CMD) XAMPP MariaDB untuk pengujian constraint berikut:

1. Dasar Pembuatan Database & Tabel

Pembuatan database fahri_biodata dan tabel fahri.

Manipulasi struktur tabel menggunakan perintah ALTER TABLE (menambah kolom email, menghapus kolom no_telpn).

Menghapus tabel dengan DROP TABLE.

2. Constraint NOT NULL

Pembuatan database fahri_praktikum dan tabel fahri_mahasiswa.

Penerapan atribut NOT NULL pada kolom nama dan npm.

Pengisian data (insertion) serta pengecekan struktur tabel dengan DESC.

3. Constraint UNIQUE

Single Column Unique: Pengujian UNIQUE pada kolom nidn tabel fahri_dosen. Menunjukkan error Duplicate entry ketika memasukkan NIDN yang sama.

Composite Unique: Pembuatan CONSTRAINT uk_produk UNIQUE (kode, nama_produk) pada tabel fahri_produk. Menjelaskan bahwa kombinasi data harus bersifat unik.

4. Constraint PRIMARY KEY

Single Primary Key: Tabel fahri_makanan dengan id_makanan sebagai Primary Key.

Composite Primary Key: Tabel fahri_table dengan CONSTRAINT pk_pesanan PRIMARY KEY (id_pesanan, tgl_pesanan).

5. Constraint FOREIGN KEY

Pembuatan relasi antar tabel fahri_penonton (Parent Table) dan fahri_tiket (Child Table).

Pengujian Integritas Referensial (Referential Integrity): Penolakan baris baru jika referensi id_penonton tidak terdaftar.

6. Constraint CHECK

Single Condition Check: Tabel fahri_menu dengan syarat CHECK (harga >= 1000).

Composite Condition Check: Tabel fahri_anggota dengan syarat CONSTRAINT chk_anggota CHECK (umur >= 19 AND kota = 'Yogya').

7. Constraint DEFAULT

Tabel fahri_dokter dengan nilai awal status VARCHAR(20) DEFAULT 'Aktif'.

Pembuktian bahwa data yang di-insert tanpa kolom status akan otomatis berstatus 'Aktif'.

8. Atribut AUTO_INCREMENT

Tabel fahri_bioskop dengan id_tiket INT PRIMARY KEY AUTO_INCREMENT.

Pengubahan nilai awal index menggunakan ALTER TABLE fahri_bioskop AUTO_INCREMENT = 30;.
