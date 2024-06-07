# termux
termux ialah software yang digunakan untuk menghubungkan android dengan mariadb untuk membuat database.
## cara menginstal termux
untuk menginstal termux kita harus mendownload software nya pada browser, lalu selanjutnya di install, setelah itu untuk masuk ke mariadb melalui proses seperti berikut :
# penggunaan awal mysql
setelah melakukan tahap "menginstal termux" selanjutnya ada tahap membuat, menghapus, melihat dan menggunakan data base.
## membuat database
untuk membuat database kita menggunakan query CREATE_DATABASE [nama_database] setelah langkah ini database
akan terbuat.


## menampilkan database
untuk menampilkan data base kita bisa menggunakan SHOW_DATABASES; untuk menampilkan data base yang telah digunakan.
## menghapus database
lalu untuk menghapus data base kita menggunakan query DROP DATABASE [nama_database]dan database akan terhapus setelah menuliskan query ini.
## menggunakan database
lalu yang terakhir untuk menggunakan database kita menggunakan query USE [nama_database].
# tabel
## buat tabel
objek penting dalam database karena menyimpan semua informasi atau data. Sebagai contoh, database untuk bisnis bisa mempunyai tabel Kontak yang menyimpan nama pemasok, alamat email, dan nomor telepon.

```mysql
create table pelanggan (      id_pelanggan int (4) primary key not null,     
nama_depan varchar (25) not null,
nama_belakang varchar (25) not null,           
no_telp char (12) unique );
```

![[IMG_20240130_153700.jpg]]
## tampilkan struktur tabel
![[IMG_20240130_153821.jpg]]
## menampilkan daftar tabel show tables
![[IMG_20240130_154158.jpg]]
## qna
> [!info]-
>>1) **Mengapa hanya kolom id_pelanggan yang menggunakan constraint PRIMARY KEY?**
>>2) **Mengapa pada kolom no_telp yang menggunakan data CHAR bukan VARCHAR?**
>>3)  **Mengapa hanya kolom no_telp yang menggunakan constraint UNIQUE?**
>>4)  **Mengapa kolom no_telp tidak memakai constraint NOT NULL sementara kolom lainnya menggunakan constraint tersebut?**
>>5) **Tuliskan perbedaan antara PRIMARY KEY dengan UNIQUE?**
>>jawaban:
>>1) Untuk membedakan id Pelanggan  yang sama, mencegah duplikasi, dan mempermudah pencarian data.
>>2) Tipe data char menyimpan data dalam karakter panjang lebih efisien. pencarian pada kolom tipe data `CHAR` dapat lebih cepat
>>3) Karna no_telp tidak ada yang sama semua pasti berbeda dan nilainya unik maka menggunakan constrains unique artinya data dalam tabel id_telpon berbeda tidak ada yang sama. 
>>4) Nomor telpon dianggap opsional. nomor telepon hanya menjadi wajib saat pengguna melakukan langkah-langkah tertentu, Anda mungkin tidak ingin mengharuskan pengguna mengisinya pada tahap awal.
>>5) PRIMERY KEY untuk membedakan data yang sama dan hanya boleh 1 dan tidak boleh tidak ada.Kalau UNiQUE sebuah kolom yang memiliki data yang berbeda atau tidak sama unique boleh 1,2,3 Dan seterusnya dan boleh tidak ada.




