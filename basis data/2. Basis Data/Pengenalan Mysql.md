##### Pertemuan 1
# Basis Data
## Definisi Basis Data
Basis data merupakan kumpulan informasi yang terorganisir, sedangkan sistem basis data menyediakan cara untuk menyimpan, mengelola, dan mengakses data tersebut. Kesimpulannya, basis data penting dalam menyediakan struktur yang teratur untuk mengelola informasi secara efisien.


> [! info]- *Basis* dan *data*
>> Basis : Wadah atau tempat berkumpul
>> Data : Kumpulan fakta dari sebuah objek

## Peranan Basis Data 
layanan transportasi berbasis aplikasi : layanan ini memberikan kemudahan kepada pengguna untuk mendapatkan kendaraan yang di butuhkan.pengguna dapat memesan layanan dengan cara memasukkan lokasi tujuan,lokasi keberangkatan,kemudian aplikasi akan menghitung biaya lalu memilih dan mengirim kan kendaraan bagi pemilik kendaraan

## Struktur Basis Sata
basis data umumnya di gambarkan sebagai tabung yang berisi data yang di nama data tersebut berbentuk tabel contohnya pada gambar di bawa ini
![Gambar1](Aset/IMG1/IMG1(1).jpg)

## Contoh Table
berikut ialah contoh table  simpel yang berisikan item Nama,Hoby dan umur :

| Nama   | Hoby       | Umur |
| ------ | ---------- | ---- |
| Fachri | Makan      | 16   |
| Hayril | Minum      | 16   |
| Rahmat | Membaca | 17   |
| Rahman | Bermain | 17   |
| Juli   | Tidur      | 16   |

## Penjelasan Database
Database ialah tempat disimpan nya data data yang digambarkan sebagai bentuk tabung, lalu berisikan data atau sebuah file dalam bentuk tabel. lalu dalam tabel dibagi dalam beberapa bagian yaitu : 
- ==Field== : kumpulan karakter yang membentuk sebuah arti disebut sebagai field.
- ==Record== : kumpulan field dalam bentuk yang kompleks 
- ==item data== : Sebuah nilai data yang berada pada kolom
- ==karakter== : sebuah nilai yang terletak pada sebuah kolom by
### Pertemuan 2
# Mysql
**Mysql** ialah software yang digunakan untuk membuat sebuah *database*. dan berikut ialah tahapan cara mendownload serta penggunaan awal dari mysql mulai dari pembuatan database dan pembuatan table.
## cara menginstal Mysql
untuk menginstal mysql pertama tama kita harus memingstal **xampp** dan untuk mendapatkannya kita dapat mendownload software tersebut pada browser. dan setelah menginstal ikuti tahap berikut ini :
1. Buka **XAMPP** lalu tunggu proses instaling selesai. dan setelah itu klik icon yang bertuliskan "FInish"
	![Gambar2](Aset/IMG2/IMG2(1).png) 
2. Setelah terlihat tampilan seperti ini klik icon "Start" pada baris **Mysql** dan klik icon yang bertuliskan "Shell".
	![Gambar3](Aset/IMG2/IMG2(2).png)
3. Dan setelah itu kita akan langsung di arahkan ke dalam **Mysql** dan tahap penginstalan telah selesai.
# Tentang Database
setelah melakukan tahap "menginstal Mysql" selanjutnya ada tahap *membuat*, *menghapus*, *melihat* dan *menggunakan* data base.
## 1) membuat database
untuk membuat database kita menggunakan query `CREATE DATABASE [nama_database]` setelah mengetikkan query tersebut akan terbuat sebuah databse dan hasilnya akan seperti dibawah ini :
![Gambar4](Aset/IMG2/IMG2(3).png)
## 2) menampilkan database
untuk menampilkan *data base* kita bisa menggunakan `SHOW DATABASES;` untuk menampilkan data base yang telah digunakan seperti pada contoh di atas kita telah membuat *database* dengan nama "RENTAL_NERO" dan hasilnya tampil pada daftar database yang telah kita buat, hasilnya akan terlihat seperti dibawah ini :
![Gambar5](Aset/IMG2/IMG2(4).png)
## 3) menghapus database
adapun untuk menghapus *database* kita menggunakan query `DROP DATABASE [nama_database]`dan *database* yang ditentukan akan terhapus lalu untuk memastikannya kita dapat melihatnya di `SHOW DATABASES`, setelah menuliskan query `DROP` hasilnya akan seperti dibawah ini :
![Gambar6](Aset/IMG2/IMG2(5).png)
## 4) menggunakan database 
lalu yang terakhir untuk menggunakan *database* yang telah kita buat di langkah langkah sebelumnya, kita dapat menggunakan query `USE [nama_database]`, lalu setelah mengetikkan query diatas kita akan langsung masuk kedalam *database* yang kita inginkan. Hasilnya akan terlihat seperti dibawah ini :
![Gambar7](Aset/IMG2/IMG2(6).png)

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
# Tentang Table 
setelah kita membuat *database* selanjutnya kita membuat *tabel* untuk tempat menyimpan data data yg akan disimpan.
## 1) pembuatan tabel
untuk pembuatan table kita menggunakan format seperti di bawah ini :
```mysql
CREATE TABLE [nama_table] (
    -> id_pelanggan INT (4) PRIMARY KEY NOT NULL,
    -> nama_depan VARCHAR(20) NOT NULL,
    -> nama_belakang VARCHAR(20) NOT NULL,
    -> no_telp VARCHAR (12) UNIQUE 
     );
```
Dan hasilnya akan seperti berikut :
![Gambar8](Aset/IMG2/IMG2(7).png)
>[!info]- Analisis
>> id_pelanggan,nama_depan,nama_belakang dan no_telp : Menjadi field dari sebuah table
>> INT :  tipe data untuk menampung nilai angka
>> VARCHAR : tipe data untuk menampung nilai huruf
>> ( ) : untuk menentukan nilai dari tipe data
>> PRIMARY KEY : menjadi sebuah penanda karna hanya ada satu di sebuah kolom
>> NOT NULL : berarti kolom harus di isi
>> UNIQUE : memiliki sistem yang mirip dengan primary key.

**Kesimpulan :**
kata pertama (id_pelanggan) ialah nama dari kolomnya lalu kata keduanya (INT) ialah nama tipe datanya lalu kata ketiga (NOT NULL) ialah untuk memastikan agar colomnya harus di isi atau tidak.


## 2) menampilkan struktur tabel
lalu setelah membuat tabel kita dapat menampilkan struktur dari table yang telah kita buat dengan cara mengetik `DESC [nama_tabel]` dan hasil kodenya akan seperti berikut :
```mysql
DESC PELANGGAN;
```
Dan hasilnya akan seperti berikut :
![Gambar9](Aset/IMG2/IMG2(8).png)
>[!info]- Analisis
>> DESC : berfungsi untuk mendeskripsikan hasil atau struktur tabel yang telah dibuat

**Kesmipulan :**
setelah membuat table kita dapat menampilkan struktur dari table tersebut dengan mengetikkan query `DESC PELANGGAN` dan hasilnya akan tampil.


## 3) menampilkan daftar tabel
untuk menampilkan daftar tabel yang ada dalam *database* kita menggunakan query `SHOW TABLES;`dan hasil yang akan tampil ialah seperti berikut : 
![Gambar10](Aset/IMG2/IMG2(9).png)

 > [!info]- Analisis 
 >>- `SHOW TABLES` ialah query yang berfungsi untuk menampilkan table table yang terdapat pada databse yang kita gunakan.
>>- `DESC TABLES` ialah query yang berfungsi untuk menampilkan struktur table yang telah dibuat. 
>>- Kita dapat membuat table dalam sebuah database dengan mengetik format pada nomor 1.

**Kesimpulan :**



# Sesi QNA
### **pertanyaan :**
1) Mengapa hanya kolom id_pelanggan yang menggunakan constraint PRIMARY KEY?
2) Mengapa pada kolom no_telp yang menggunakan data CHAR bukan VARCHAR?
3)  Mengapa hanya kolom no_telp yang menggunakan constraint UNIQUE?
4)  Mengapa kolom no_telp tidak memakai constraint NOT NULL sementara kolom lainnya menggunakan constraint tersebut?
5) Tuliskan perbedaan antara PRIMARY KEY dengan UNIQUE?

### **Jawaban :** 
1) Untuk membedakan id Pelanggan  yang sama, mencegah duplikasi, dan mempermudah pencarian data.
2) Tipe data char menyimpan data dalam karakter panjang lebih efisien. pencarian pada kolom tipe data `CHAR` dapat lebih cepat.
3) Karna no_telp tidak ada yang sama semua pasti berbeda dan nilainya unik maka menggunakan constrains unique artinya data dalam tabel id_telpon berbeda tidak ada yang sama. 
4) Nomor telpon dianggap opsional. nomor telepon hanya menjadi wajib saat pengguna melakukan langkah-langkah tertentu, Anda mungkin tidak ingin mengharuskan pengguna mengisinya pada tahap awal.
5) PRIMERY KEY untuk membedakan data yang sama dan hanya boleh 1 dan tidak boleh tidak ada. 
	Kalau UNiQUE sebuah kolom yang memiliki data yang berbeda atau tidak sama unique boleh 1,2,3 Dan seterusnya dan boleh tidak ada.
## Pertemuan 3
# Insert dan Select
Setelah mempelajari cara untuk membuat, melihat struktur dan menampilkan daftar table sekarang kita akan mempelajari cara memasukan data pada table serta menampilkan hasil dari table tersebut, untuk melakukannya kita akan membaginya menjadi dua bagian yaitu *Insert* dan *Select*.

## ==Insert==
query satu ini memiliki fungsi untuk memasukkan sebuah nilai pada table yang telah kita buat dan kita akan mempelajari insert data 1 baris dan lebih dari satu baris.

### Insert 1 baris
untuk menginput data satu baris kita menggunakan format seperti berikut :
```mysql
INSERT INTO [NAMA_TABLE]
 VALUES (DATA_1, DATA_2, DATA_3, DATA_4);
```
atau untuk pengaplikasiannya seperti berikut :
![Gambar11](Aset/IMG3/IMG3(1).png)

### Insert lebih 1 baris
Sedangkan untuk menginput nilai yang lebih dari satu baris kita menggunakan foramt seperti dibawah ini :
```mysql
INSERT INTO [NAMA_TABLE]
 VALUES (DATA_1, DATA_2, DATA_3, DATA_4),
(DATA_1, DATA_2, DATA_3, DATA_4),
(DATA_1, DATA_2, DATA_3, DATA_4);
```
atau untuk pengaplikasiannya seperti berikut :
![Gambar12](Aset/IMG3/IMG3(2).png)


## ==Select== 
Selanjutnya query ini memiliki fungsi untuk menampilkan hasil dari table yang telah di inputkan (Insert) data kedalam tabel tersebut, berbeda dengan `desc` yang hanya menampilkan struktur dari table query ini menampilkan hasil dari table. 

### Select all table
untuk menampilkan hasil dari seluruh table yang telah dibuat/menampilkan seluruh baris dan kolom kita menggunakan format seperti dibawah ini :
```mysql
SELECT * FROM [NAMA_TABLE];
```
Dan hasilnya akan tampil seperti ini :
![Gambar13](Aset/IMG3/IMG3(3).png)


### Select field spesifik
lalu untuk menampilkan beberapa kolom yang spesifik kita dapat menggunakan format yang sedikit berbeda dengan format all table, yaitu seperti dibawah ini :
```mysql
SELECT NAMA_KOLOM_1, NAMA_KOLOM_2, NAMA_KOLOM_N FROM PELANGGAN;
```
Dan hasil yang akan tampil ialah kolom kolom yang di minta saja contoh dan hasilnya akan seperti ini :
![Gambar14](Aset/IMG3/IMG3(4).png)

### Select kondisi "where"
lalu kondisi yang saat satu ini berfungsi untuk mengambil data yang lebih spesifik dari sebuah field dengan simbol simbol aritmatika mulai dari "+", "-", "/", "%",">","<". Misalnya kita meminta untuk menampilkan field "Nama_Depan" pada "Id_Pelanggan" ke 2, kita dapat menggunakan simbol aritmatika seperti berikut :
```mysql
SELECT Nama_Kolom FROM Nama_Table WHERE Id_Pelanggan=2; 
```
Dan contoh serta hasilnya akan terlihat seperti berikut ini :
![Gambar15](Aset/IMG3/IMG3(5).png)

> [!info]- Analisis
>> - Insert ialah query yang berfungsi untuk memasukkan data pada table yang telah kita buat.
>> - Select ialah query yang berfungsi untuk menampilkan hasil table dan select ini terbagi menjadi 3 bagian.
>> - 3 Jenis Select ialah Select All Table, Select Field Spesifik dan Select kondisi atau "Where". 
>> - Where ini berisikan simbol simbol aritamtika mulai dari "+", "-", "/", "%",">","<".
>> - "`*`"simbol bintang ini memiliki makna "all" atau "semua" 


### Kesimpulan
Kesimpulannya ialah **insert** bertugas untuk memasukkan nilai pada table yang telah dibuat dan **Select** berfungsi untuk menampilkan hasil dari table yang telah dibuat dan di input datanya dari *Query* sebelumnya, lalu **Select** ini dapat menampilkan semua sesuai dengan yang kita menggunakan misalnya jika ingin menampilkan seluruh table kita menggunakan simbol "`*`" atau All lalu jika ingin menampilkan beberapa field kita dapat menggunakan format hanya perlu memanggil nama fieldnya.

Lalu yang terakhir ialah kondisi "Where" dimana kita dapat memanggil nama field dengan menggunakan simbol aritmatika, misalnya kita ingin memanggil field "Nama_Pelanggan" tapi hanya ''Id_Pelanggan" 2 kita dapat menggunkan format seperti ini `SELECT Nama_Kolom FROM Nama_Table WHERE Id_Pelanggan=2;`


## ==Update==
Selanjutnya jika ingin mengganti nilai dari sebuah kolom tertentu  kita bisa menggunakan *Query* **Update** lalu formatnya seperti dibawah ini :
```mysql
Format :
UPDATE [Nama_Table] SET [Nama_Kolom]="Nilai_Pengganti" WHERE kondisi;

Contoh :
UPDATE PELANGGAN SET No_Telp="083135219096" WHERE Id_Pelanggan=1;
```

Berikut ialah contoh pengaplikasian dan hasil dari penggunaan **Update** :
![Gambar16](Aset/IMG3/IMG3(6).png)

## ==Delete==
Kita juga dapat menghapus baris pada table dengan *Query* **Delete**, untuk menghapus keseluruhan baris kita dapat menggunakan format seperti ini :
```mysql
Format :
DELETE FROM [Nama_Table] WHERE [Nama_Kolom];

Contoh :
DELETE FROM PELANGGAN WHERE Id_Pelanggan=6;
```

Berikut ialah contoh pengaplikasian dan hasil dari penggunaan **Delete** :
![Gambar18](Aset/IMG3/IMG3(8).png)


> [!Info]- Analisis
>> **Update** ialah *Query* untuk mengganti nilai yang telah ada pada sebuah table yang telah ada sebelumnya.
>> **Delete** ialah *Query* untuk menghapus baris pada sebuah tabel yang telah dibuat sebelumnya.
>> Penggunaan *Where* masih sangat berperan penting dalam kondisi seperti ini.

### Kesimpulan 
dua *Query* yang akan dipelajari selanjutnya ialah untuk mengganti data dan menghapus baris data pada table. *Query* nya ialah **Update** untuk mengganti data yang telah ada pada table, dan *Query* **Delete** untuk menghapus nilai yang telah ada pada table yang telah kita buat. kedua *Query* ini memiliki format yang lumayan mirip, dimana memerlukan *Where* untuk menuliskan kondisinya.





Pisah file baru
##### Pertemuan 4
# Select Lanjutan
Setelah mempelajari select di materi sebelumnya sekarang kita akan masuk ke dalam materi select lanjutan, fungsi dari select select ini ialah untuk mendapatkan hasil yang lebih spesifik dan lebih luas, sekarang kita akan mempelajari 7 select lanjutan **(AND ,OR ,BETWEEN-AND ,NOT BETWEEN ,<= ,>= ,<> ATAU !=)** Untuk penjelasan lebih lanjutnya ialah seperti berikut :

> [!info]- Isi Table yang akan digunakan :
>>![Gambar19](IMG4(1).png)
>

## AND
untuk **AND** ini akan mengambil "data 1" *dan* "data 2", contoh kodenya adalah seperti berikut :
```mysql
SELECT warna,pemilik FROM mobil WHERE warna="Hitam" AND pemilik="ibrahim";
```
Dan hasilnya akan seperti berikut :
![Gambar20](Aset/IMG4/IMG4(2).png)

## OR
Untuk **OR** ini akan mengambil "data 1" *atau* "data 2", contoh kodenya ialah seperti berikut :
```mysql
SELECT warna,pemilik FROM mobil WHERE warna="Hitam" OR pemilik="ibrahim";
```
Dan hasilnya akan seperti berikut :
![Gambar21](Aset/IMG4/IMG4(3).png)

## BETWEEN-AND
Untuk **BETWEEN-AND** ini akan mengambil antara "data 1" *sampai* "data 2" dibantu dengan **AND**, contoh kodenya ialah seperti berikut :
```mysql
SELECT * FROM mobil WHERE harga_rental BETWEEN 100000 AND 200000;
```
Dan hasilnya akan seperti berikut :
![Gambar22](Aset/IMG4/IMG4(4).png)

## NOT BETWEEN 
Untuk **NOT BETWEEN** ini akan mengambil "data" yang *bukan antara* "data 1" *dan* "data 2", contoh kodenya ialah seperti berikut :
```mysql
MariaDB [rental_nero]> SELECT * FROM mobil WHERE harga_rental NOT BETWEEN 100000 AND 200000;
```
Dan hasilnya akan seperti berikut :
![Gambar23](Aset/IMG4/IMG4(5).png)


## <=
Untuk **<=** ini akan mengambil "data"  lebih kecil atau sama dengan "nilai data", contoh kodenya ialah seperti berikut :
```mysql
MariaDB [rental_nero]> SELECT * FROM mobil WHERE harga_rental <= 50000;
```
Dan hasilnya akan seperti berikut :
![Gambar24](Aset/IMG4/IMG4(6).png)


## >=
Untuk **>=** ini akan mengambil "data"  lebih besar atau sama dengan "nilai data", contoh kodenya ialah seperti berikut :
```mysql
MariaDB [rental_nero]> SELECT * FROM mobil WHERE harga_rental >= 50000;
```
Dan hasilnya akan seperti berikut :
![Gambar25](Aset/IMG4/IMG4(7).png)


## <> atau !=
Untuk **<> atau !=** ini akan mengambil "data"  yang tidak sama dengan "nilai data", contoh kodenya ialah seperti berikut :
```mysql
MariaDB [rental_nero]> SELECT * FROM mobil WHERE harga_rental <> 50000;
```
Dan hasilnya akan seperti berikut :
![Gambar26](Aset/IMG4/IMG4(8).png)


## Tantangan 

Untuk tantangan saya akan mengambil nama pemilik "Ibe" dengan cara memanggilnya dengan syarat nomor pelatnya yaitu "DD 2901 JK" lalu hasilnya akan seperti berikut :
![Gambar27](Aset/IMG4/IMG4(9).png)
.
> [!info]- Analisis
>> "AND" : Mengambil data 1 **dan** data 2.
>> "OR" : Mengambil data antara data 1 **atau** data 2.
>> "BETWEEN-AND" : Mengambil data **antara** data 1 **sampai** data 2.
>> "NOT BETWEEN" : Mengambil data yang tidak  **antara** data 1 **sampai** data 2.
>> "<=" : Mengambil data yang lebih kecil atau sama dengan nilai data.
>> ">=" : Mengambil data yang lebih besar atau sama dengan nilai data.
>> "<> atau !=" : Mengambil data yang **tidak** sama dengan nilai data.


Kesimpulan : 
Select ini memiliki cakupan yang luas dan bervariasi semunya juga memiliki kelebihan dan keunikan masing masing sehingga dapat menampilkan hasil sebuah nilai yang di inginkan, keberagaman select ini mulai dari AND ,OR ,BETWEEN-AND ,NOT BETWEEN ,<= ,>= ,<> ATAU !=.  

