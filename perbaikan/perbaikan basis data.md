# Rangkuman Basis Data

## Definisi Basis Data

Basis data adalah kumpulan data yang terorganisir dan disimpan secara sistematis sehingga dapat diakses, dikelola, dan diperbarui dengan mudah. Basis data biasanya dioperasikan oleh sistem manajemen basis data (DBMS).

### Peranan Basis Data

1. **Penyimpanan Data**: Menyimpan data dalam jumlah besar dengan cara yang efisien.
2. **Akses Data**: Memungkinkan akses data yang cepat dan mudah oleh pengguna.
3. **Manajemen Data**: Membantu dalam pengelolaan data termasuk penyimpanan, pengambilan, dan pembaruan data.
4. **Keamanan Data**: Menyediakan mekanisme untuk melindungi data dari akses yang tidak sah.
5. **Integritas Data**: Memastikan data yang disimpan akurat dan konsisten.

### Struktur Basis Data

1. **Skema Basis Data**: Deskripsi lengkap dari database, termasuk struktur tabel, relasi antar tabel, dan kendala-kendala yang ada.
2. **Tabel**: Kumpulan data yang terstruktur dalam baris dan kolom.
3. **Kolom (Atribut)**: Komponen dari tabel yang merepresentasikan kategori data.
4. **Baris (Record)**: Satu set data yang terdiri dari nilai-nilai dalam kolom yang berbeda.
5. **Indeks**: Struktur data yang meningkatkan kecepatan pengambilan data.

### Penjelasan Database

Database adalah tempat penyimpanan data yang terstruktur dengan menggunakan sistem manajemen basis data (DBMS). DBMS adalah perangkat lunak yang digunakan untuk membuat, mengelola, dan memanipulasi database. Contoh DBMS populer termasuk MySQL, PostgreSQL, Oracle, dan Microsoft SQL Server.

DBMS menyediakan berbagai fungsi penting seperti:

- **Definisi Data**: Mendefinisikan struktur data yang disimpan.
- **Manipulasi Data**: Memungkinkan pengguna untuk melakukan operasi seperti insert, update, delete, dan retrieve data.
- **Keamanan Data**: Memberikan kontrol akses terhadap data yang disimpan.
- **Transaksi**: Memastikan bahwa semua operasi pada data dilaksanakan dengan integritas penuh.

Basis data sangat penting dalam berbagai aplikasi modern, mulai dari sistem informasi perusahaan, situs web e-commerce, hingga aplikasi media sosial.

# Rangkuman MySQL

## Definisi MySQL
MySQL adalah sistem manajemen basis data relasional (RDBMS) yang menggunakan Structured Query Language (SQL) sebagai bahasa utamanya. MySQL adalah salah satu RDBMS yang paling populer dan banyak digunakan, terutama untuk aplikasi web, karena kecepatan, keandalan, dan kemudahan penggunaannya.

## Kelebihan MySQL
- Open Source: MySQL adalah perangkat lunak sumber terbuka yang dapat digunakan secara gratis.
- Performa Tinggi: MySQL dikenal memiliki kecepatan dan performa yang tinggi.
- Skalabilitas: MySQL dapat menangani database dengan ukuran besar dan dapat dioptimalkan untuk berbagai jenis aplikasi.
- Keamanan: Menyediakan berbagai fitur keamanan seperti otentikasi pengguna dan enkripsi data.
- Kompatibilitas: Mendukung berbagai platform seperti Windows, Linux, dan macOS.

# rangkuman database
## Penjelasan Database
Database adalah kumpulan data yang terorganisir sehingga dapat diakses, dikelola, dan diperbarui dengan mudah. Database dioperasikan oleh Sistem Manajemen Basis Data (DBMS), yang bertindak sebagai antarmuka antara pengguna dan data yang disimpan. DBMS populer meliputi MySQL, PostgreSQL, SQLite, Oracle, dan SQL Server.
## Struktur Dasar Database
- Tabel: Struktur dasar dalam database yang terdiri dari baris (records) dan kolom (fields).
- Baris: Satu set data yang terdiri dari beberapa kolom.
- Kolom: Atribut atau field dari tabel yang mendeskripsikan data.
## Cara Membuat Database
### Membuat Database
Gunakan perintah berikut untuk membuat database:

```sql
CREATE DATABASE nama_database;
```
#### contoh
```sql
CREATE DATABASE siswa_rpl;
```

### Menampilkan Database
Untuk menampilkan semua database yang ada, gunakan perintah berikut:
#### contoh
```sql
SHOW DATABASES;
```

### Menggunakan Database
Untuk memilih dan menggunakan database tertentu, gunakan perintah berikut:

```sql
USE nama_database;
```
#### contoh
```sql
USE siswa_rpl
```

### Menghapus Database
Untuk menghapus database, gunakan perintah berikut:

```sql
DROP DATABASE nama_database;
```
#### Contoh
```sql
DROP DATABASE siswa_rpl;
```

Dengan memahami langkah-langkah dasar ini, Anda dapat mengelola database di berbagai sistem manajemen basis data

# Tipe Data pada Mysql
## angka

-  ==INT:== Untuk menyimpan nilai bilangan bulat (integer). Misalnya, INT dapat digunakan untuk menyimpan angka seperti 1, 100, -10, dan sebagainya. 

 - ==DECIMAL: ==Digunakan untuk menyimpan nilai desimal presisi tinggi, cocok untuk perhitungan finansial atau keuangan.
 - 
 - ==FLOAT dan DOUBLE: ==Digunakan untuk menyimpan nilai desimal dengan presisi floating-point. DOUBLE memiliki presisi lebih tinggi dibandingkan FLOAT.
 
 - ==TINYINT, SMALLINT,== ==MEDIUMINT==, dan ==BIGINT: ==Tipe data ini menyimpan bilangan bulat dengan ukuran yang berbeda-beda.
   Contoh : 

	```mysql
	CREATE TABLE contoh_tabel (
	    id INT,
	    harga DECIMAL(10, 2),
	    jumlah_barang TINYINT
	);
	```


Dalam contoh tersebut, id menggunakan tipe data INT, harga menggunakan tipe data `DECIMAL `dengan presisi 10 digit dan 2 angka di belakang koma, dan jumlah_barang menggunakan tipe data `TINYINT.
`
## teks

- ==CHAR(N) ==Menyimpan string karakter tetap dengan panjang N. Contoh: ==CHAR(10) ==akan menyimpan string dengan panjang tepat 10 karakter.

- ==VARCHAR(N):== Menyimpan string karakter dengan panjang variabel maksimal N. Misalnya, ==VARCHAR(255) ==dapat menyimpan string hingga 255 karakter, tetapi sebenarnya hanya menyimpan panjang yang diperlukan plus beberapa overhead.

- ==TEXT: ==Digunakan untuk menyimpan teks dengan panjang variabel, tanpa batasan panjang tertentu. Cocok untuk data teks yang panjangnya tidak terduga.

- ==ENUM: ==Memungkinkan Anda mendefinisikan set nilai yang mungkin dan membatasi kolom hanya dapat mengambil salah satu dari nilai tersebut.

- ==SET: ==Mirip dengan ENUM, namun dapat menyimpan satu atau lebih nilai dari himpunan yang telah ditentukan.

**Contoh :**
```mysql
CREATE TABLE contoh_tabel (
    nama CHAR(50),
    alamat VARCHAR(100),
    catatan TEXT,
    status ENUM('Aktif', 'Non-Aktif')
);
```

## tanggal

- ==DATE== :  Menyimpan nilai tanggal dengan format YYYY-MM-DD.
- ==TIME==: Menyimpan nilai waktu dengan format HH:MM:SS.

- ==DATETIME: ==Menggabungkan nilai tanggal dan waktu dengan format YYYY-MM-DD HH:MM:SS.

- ==TIMESTAMP: ==Sama seperti DATETIME, tetapi dengan kelebihan diatur secara otomatis saat data dimasukkan atau diubah.

```mysql
CREATE TABLE ContohTabel (
    tanggal DATE,
    waktu TIME,
    datetimekolom DATETIME,
    timestampkolom TIMESTAMP
);
```


Dalam contoh ini, kolom *==tanggal==* akan menyimpan nilai tanggal, *==waktu==* menyimpan nilai waktu, ==*datetimekolom== menyimpan kombinasi tanggal dan waktu, dan **==timestampkolom==* akan secara otomatis diatur saat data dimasukkan atau diubah.

## Boolean

- ==BOOL / BOOLEAN / TINYINT(1):== Digunakan untuk menyimpan nilai boolean, yang dapat mewakili kebenaran atau kesalahan. Representasi nilai benar adalah 1, sedangkan nilai salah direpresentasikan sebagai 0. Meskipun nilai selain 0 dianggap benar, secara umum, ketiganya seringkali digunakan secara bergantian. Seringkali, ketika Anda mendeklarasikan kolom sebagai BOOL atau BOOLEAN, MySQL mengonversinya secara otomatis menjadi TINYINT(1), yang juga dapat digunakan untuk menyimpan nilai boolean dengan 0 untuk false dan 1 untuk true.

1. Menggunakan BOOLEAN
```mysql
CREATE TABLE contohTabel (
    title VARCHAR(255),
    completed BOOLEAN
);
```
Dalam contoh diatas, kita mendefinisikan kolom completed sebagai tipe data BOOLEAN. Ini merupakan cara yang sah dan umum digunakan di MySQL. Nilai yang dapat disimpan dalam kolom ini adalah TRUE atau FALSE, atau dalam representasi angka, 1 atau 0.

2. Menggunakan BOOL
```mysql
CREATE TABLE contohTabel (
    title VARCHAR(255),
    completed BOOL
);
```

Dalam contoh ini, kita menggunakan BOOL sebagai tipe data untuk kolom completed. Perlu dicatat bahwa MySQL secara otomatis mengonversi BOOL menjadi TINYINT(1). Oleh karena itu, pada dasarnya, ini setara dengan contoh pertama. Namun, beberapa pengembang lebih suka menggunakan BOOLEAN untuk kejelasan.

3. Menggunakan TINYINT(1)
```mysql
CREATE TABLE contohTabel (
    title VARCHAR(255),
    completed TINYINT(1)
);
```

Dalam contoh ini, kita menggunakan TINYINT(1) sebagai tipe data untuk kolom completed. Ini adalah pendekatan yang valid karena MySQL mengonversi BOOL menjadi TINYINT(1) secara otomatis. Dalam hal ini, nilai yang dapat disimpan adalah 1 untuk TRUE dan 0 untuk FALSE.

## rangkuman Tentang Table
setelah kita membuat database selanjutnya kita membuat tabel untuk tempat menyimpan data data yg akan disimpan.

### pembuatan tabel

Untuk membuat tabel baru, gunakan perintah `CREATE TABLE` dengan mendefinisikan kolom dan tipe datanya

```sql
CREATE TABLE nama_tabel (
    nama_kolom1 tipe_data1 [constraints],
    nama_kolom2 tipe_data2 [constraints],
    ...
);
```
#### contoh
```sql
CREATE TABLE guru (
    id INT PRIMARY KEY AUTO_INCREMENT,
    nig INT NOT NULL,
    nama VARCHAR(100) NOT NULL,
    umur INT,
    gaji DECIMAL(10, 2),
    tanggal_lahir DATE
);
```

#### penjelasan

- `id`: Kolom dengan tipe data integer, sebagai primary key, dan auto-increment.
- `nig`: Kolom ini menyimpan Nomor Induk Guru dan diatur sebagai NOT NULL, yang berarti kolom ini harus memiliki nilai.
- `nama`: Kolom dengan tipe data varchar dengan panjang maksimal 100 karakter, dan tidak boleh null.
- `umur`: Kolom dengan tipe data integer.
- `gaji`: Kolom dengan tipe data desimal dengan 10 digit total dan 2 digit desimal.
- `tanggal_lahir`: Kolom dengan tipe data date

### Menampilkan Struktur Tabel
Untuk menampilkan struktur tabel (kolom, tipe data, constraints, dll.), gunakan perintah DESCRIBE.

```sql
DESCRIBE nama_tabel;
```
#### contoh
```sql
DESCRIBE guru;
```
#### penjelasan 
Perintah ini akan menampilkan informasi tentang kolom dalam tabel `guru`.

### Menampilkan Daftar Tabel
Untuk menampilkan daftar semua tabel dalam database yang sedang digunakan, gunakan perintah `SHOW TABLES`.
#### contoh
```sql
SHOW TABLES;
```
#### penjelasan 
Perintah ini akan menampilkan semua tabel yang ada dalam database yang sedang aktif.

## Insert dan Select
Setelah mempelajari cara untuk membuat, melihat struktur dan menampilkan daftar table sekarang kita akan mempelajari cara memasukan data pada table serta menampilkan hasil dari table tersebut, untuk melakukannya kita akan membaginya menjadi dua bagian yaitu *Insert* dan *Select*.

### Insert
query satu ini memiliki fungsi untuk memasukkan sebuah nilai pada table yang telah kita buat dan kita akan mempelajari insert data 1 baris dan lebih dari satu baris.

### Insert 1 baris
Perintah `INSERT` digunakan untuk menambahkan satu baris data ke dalam tabel dalam database. Berikut adalah penjelasan

#### Penjelasan:
Perintah `INSERT` memungkinkan Anda untuk menambahkan data baru ke dalam tabel. Dalam kasus satu baris, Anda menentukan nilai untuk setiap kolom yang ingin Anda masukkan.

```sql
INSERT INTO nama_tabel (kolom1, kolom2, kolom3, ...)
VALUES (nilai1, nilai2, nilai3, ...);
```
#### analisis
- `nama_tabel`: Nama tabel tempat Anda ingin memasukkan data.
- `kolom1, kolom2, kolom3, ...`: Nama kolom yang akan Anda isi dengan nilai.
- `nilai1, nilai2, nilai3, ...`: Nilai yang akan dimasukkan ke dalam kolom tersebut.
### insert Lebih dari 1 Baris
Anda juga dapat menambahkan lebih dari satu baris data sekaligus menggunakan perintah INSERT. Berikut adalah penjelasan 
#### Penjelasan:
Dengan menambahkan beberapa baris sekaligus, Anda menyediakan beberapa set nilai untuk dimasukkan ke dalam tabel.

```sql
INSERT INTO nama_tabel (kolom1, kolom2, kolom3, ...)
VALUES
  (nilai1a, nilai2a, nilai3a, ...),
  (nilai1b, nilai2b, nilai3b, ...),
  (nilai1c, nilai2c, nilai3c, ...);
```
#### analisis
- `nama_tabel`: Nama tabel tempat Anda ingin memasukkan data.
- `kolom1, kolom2, kolom3, ...`: Nama kolom yang akan Anda isi dengan nilai.
- `(nilai1a, nilai2a, nilai3a, ...)`, `(nilai1b, nilai2b, nilai3b, ...)`, `(nilai1c, nilai2c, nilai3c, ...)`: Set nilai untuk setiap baris yang akan dimasukkan.
### Select
Selanjutnya query ini memiliki fungsi untuk menampilkan hasil dari table yang telah di inputkan (Insert) data kedalam tabel tersebut, berbeda dengan `desc` yang hanya menampilkan struktur dari table query ini menampilkan hasil dari table. 
#### select all table (Memilih Semua Kolom dari Tabel)

```sql
SELECT * FROM nama_tabel;
```
#### penjelasan 
Ini akan mengambil semua kolom dan semua baris dari tabel `nama_tabel`.
#### Select field spesifik(Memilih Kolom Tertentu)

```sql
SELECT kolom1, kolom2 FROM nama_tabel;
```
#### penjelasan 
Ini akan mengambil hanya kolom `kolom1` dan `kolom2` dari tabel `nama_tabel`.
### Select kondisi where (Memilih dengan Kondisi WHERE)

```sql
SELECT * FROM nama_tabel WHERE kondisi;
```
#### penjelasan 
Ini akan mengambil semua kolom dan baris yang memenuhi kondisi tertentu dari tabel `nama_tabel`.

### Update
Selanjutnya jika ingin mengganti nilai dari sebuah kolom tertentu  kita bisa menggunakan *Query* **Update** lalu formatnya seperti dibawah ini :

```sql
Format :
UPDATE [Nama_Table] SET [Nama_Kolom]="Nilai_Pengganti" WHERE kondisi;

Contoh :
UPDATE PELANGGAN SET No_Telp="083135219096" WHERE Id_Pelanggan=1;
```

### Delete
Kita juga dapat menghapus baris pada table dengan *Query* **Delete**, untuk menghapus keseluruhan baris kita dapat menggunakan format seperti ini :

```sql
Format :
DELETE FROM [Nama_Table] WHERE [Nama_Kolom];

Contoh :
DELETE FROM PELANGGAN WHERE Id_Pelanggan=6;
```