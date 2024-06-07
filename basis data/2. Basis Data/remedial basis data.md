## Soal 1: Buat Tabel tabel_guru dan Simpan di dalam Database
Query
 ```sql
 CREATE DATABASE sekolah_adrian;

USE sekolah_adrian;

CREATE TABLE tabel_guru (
    id_guru INT PRIMARY KEY,
    nama_depan VARCHAR(50),
    nama_belakang VARCHAR(50),
    mapel VARCHAR(100),
    jabatan VARCHAR(100),
    usia INT,
    tanggal_lahir DATE
);
```
Analisis:
Membuat database sekolah_adrian dan tabel tabel_guru dengan kolom sesuai instruksi soal.

## Soal 2: Masukkan Data ke Tabel tabel_guru
Query:
```sql
INSERT INTO tabel_guru (id_guru, nama_depan, nama_belakang, mapel, jabatan, usia, tanggal_lahir)
VALUES 
(1, 'Adrianty', '', 'Pemrograman Web', 'Ketua Jurusan', 34, '1982-06-29'),
(2, 'Ibrahim', 'Mallombasang', 'Basis Data', 'Kepala Sekolah', 21, '2000-09-21'),
(3, 'Muhammad', 'Yusuf', 'Pemodelan Perangkat Lunak', 'Asisten Kepala Sekolah', 28, '1992-12-24'),
(4, 'Rusdyansyar', '', 'Pemrograman Berorientasi Objek', 'Asisten Kepala Sekolah', 25, '1996-01-21');
```
Analisis:
Memasukkan data yang diberikan ke dalam tabel tabel_guru.

## Soal 3: Tambahkan Data Berisi Nama Kalian dan Isi Data Lainnya
Query:
```sql
INSERT INTO tabel_guru (id_guru, nama_depan, nama_belakang, mapel, jabatan, usia, tanggal_lahir)
VALUES 
(5, 'NamaKalian', 'BelakangKalian', 'Matematika', 'Guru', 30, '1993-01-01');
```
analisis:
Menambahkan satu baris data baru sesuai dengan nama kalian dan data lainnya sesuai keinginan.

## Soal 4: Tampilkan Seluruh Data
Query:
```sql
SELECT * FROM tabel_guru;
```
Analisis:
Menampilkan semua data yang ada di tabel tabel_guru.

## Soal 5: Tampilkan Data dari Rusdyansyar Tanpa Guru Lain
Query:
```sql
SELECT * FROM tabel_guru WHERE nama_depan = 'Rusdyansyar';
```
Analisis:
Menampilkan hanya data dari Rusdyansyar sesuai permintaan soal.

## Soal 6: Ganti nama_belakang untuk id_guru = 2 Menjadi Ganteng
Query:
```sql
UPDATE tabel_guru SET nama_belakang = 'Ganteng' WHERE id_guru = 2;

SELECT * FROM tabel_guru WHERE id_guru = 2;
```
Analisis:
Mengubah nama_belakang untuk id_guru = 2 menjadi Ganteng dan menampilkan data tersebut.

## Soal 7: Hapus Data yang Dimasukkan pada Soal Nomor 3
Query:
```sql
DELETE FROM tabel_guru WHERE id_guru = 5;

SELECT * FROM tabel_guru;
```
Analisis:
Menghapus data yang dimasukkan pada soal nomor 3 dan menampilkan data tabel setelah penghapusan.

## Soal 8: Tampilkan Data Guru dengan Usia Kurang dari 30 Tahun
Query:
```sql
SELECT * FROM tabel_guru WHERE usia < 30;
SELECT * FROM tabel_guru WHERE mapel LIKE 'Pem%' ORDER BY usia ASC;
```
Analisis:
Menampilkan data guru yang berusia kurang dari 30 tahun.
Menampilkan data guru dengan mapel yang dimulai dengan "Pem" dan mengurutkannya berdasarkan usia.

## Soal 9: Tampilkan Nama Depan yang Mengandung Huruf 'r'
Query:
```sql
SELECT id_guru, nama_depan FROM tabel_guru WHERE nama_depan LIKE '%r%' OR nama_depan LIKE '%R%';
```
Analisis:
Menampilkan nama_depan yang mengandung huruf 'r' atau 'R'.

## Soal 10: Gabungkan nama_depan dan nama_belakang Menjadi nama_lengkap
Query:
```sql
SELECT CONCAT(nama_depan, ' ', nama_belakang) AS nama_lengkap FROM tabel_guru;
```
Analisis
Menggabungkan kolom nama_depan dan nama_belakang menjadi kolom baru nama_lengkap

## Soal 11: Tambahkan Kolom status dan Perbarui Nilainya
Query:
```sql
ALTER TABLE tabel_guru ADD status ENUM('PNS', 'PPPK', 'Honorer');

UPDATE tabel_guru SET status = 
    CASE 
        WHEN id_guru = 1 THEN 'PNS'
        WHEN id_guru = 2 THEN 'PPPK'
        WHEN id_guru = 3 THEN 'Honorer'
        WHEN id_guru = 4 THEN 'PNS'
        ELSE 'Honorer'
    END;

DESCRIBE tabel_guru;
```
Analisis:
Menambahkan kolom status dan mengisi nilainya sesuai kondisi yang diberikan.

## Soal 12: Tampilkan nama_depan dan usia Guru yang Paling Tua
Query:
```sql
SELECT nama_depan, usia FROM tabel_guru ORDER BY usia DESC LIMIT 1;
```
Analisis:
Menampilkan nama depan dan usia guru yang paling tua.