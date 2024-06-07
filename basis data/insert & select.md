## insert dan select
Setelah mempelajari cara untuk membuat, melihat struktur dan menampilkan daftar table sekarang kita akan mempelajari cara memasukan data pada table serta menampilkan hasil dari table tersebut, untuk melakukannya kita akan membaginya menjadi dua bagian yaitu Insert dan Select.

## ==Insert==
query satu ini memiliki fungsi untuk memasukkan sebuah nilai pada table yang telah kita buat dan kita akan mempelajari insert data 1 baris dan lebih dari satu baris.

### Insert 1 baris
untuk menginput data satu baris kita menggunakan format seperti berikut :
```mysql
INSERT INTO [NAMA_TABLE]
 VALUES (DATA_1, DATA_2, DATA_3, DATA_4);
```
## Insert lebih 1 baris
Sedangkan untuk menginput nilai yang lebih dari satu baris kita menggunakan foramt seperti dibawah ini :
```mysql
INSERT INTO [NAMA_TABLE]
 VALUES (DATA_1, DATA_2, DATA_3, DATA_4),
(DATA_1, DATA_2, DATA_3, DATA_4),
(DATA_1, DATA_2, DATA_3, DATA_4);
 
```

## ==Select== 
Selanjutnya query ini memiliki fungsi untuk menampilkan hasil dari table yang telah di inputkan (Insert) data kedalam tabel tersebut, berbeda dengan `desc` yang hanya menampilkan struktur dari table query ini menampilkan hasil dari table. 

## Select all table
untuk menampilkan hasil dari seluruh table yang telah dibuat/menampilkan seluruh baris dan kolom kita menggunakan format seperti dibawah ini :

Struktur:
```mysql
select * from [nama_table];
```
contoh:
```mysql
select * from pelanggan;
```
## select field spesifik
lalu untuk menampilkan beberapa kolom yang spesifik kita dapat menggunakan format yang sedikit *berbeda* dengan format all table, yaitu seperti dibawah ini :
```mysql
SELECT NAMA_KOLOM_1, NAMA_KOLOM_2, NAMA_KOLOM_N FROM PELANGGAN;
```
Dan hasil yang akan tampil ialah kolom kolom yang di minta saja contoh dan hasilnya akan seperti ini :
### Select kondisi "where"
lalu kondisi yang saat satu ini berfungsi untuk mengambil data yang lebih spesifik dari sebuah field dengan simbol simbol aritmatika mulai dari "+", "-", "/", "%",">","<". Misalnya kita meminta untuk menampilkan field "Nama_Depan" pada "Id_Pelanggan" ke 2, kita dapat menggunakan simbol aritmatika seperti berikut :
```mysql
SELECT Nama_Kolom FROM Nama_Table WHERE Id_Pelanggan=2; 
```
Dan contoh serta hasilnya akan terlihat seperti berikut ini :
> [!info]- Analisis
>> - Insert ialah query yang berfungsi untuk memasukkan data pada table yang telah kita buat.
>> - Select ialah query yang berfungsi untuk menampilkan hasil table dan select ini terbagi menjadi 3 bagian.
>> - 3 Jenis Select ialah Select All Table, Select Field Spesifik dan Select kondisi atau "Where". 
>> - Where ini berisikan simbol simbol aritamtika mulai dari "+", "-", "/", "%",">","<".
>> - "`*`"simbol bintang ini memiliki makna "all" atau "semua" 
### Kesimpulan
Kesimpulannya ialah **insert** bertugas untuk memasukkan nilai pada table yang telah dibuat dan **Select** berfungsi untuk menampilkan hasil dari table yang telah dibuat dan di input datanya dari *Query* sebelumnya, lalu **Select** ini dapat menampilkan semua sesuai dengan yang kita menggunakan misalnya jika ingin menampilkan seluruh table kita menggunakan simbol "`*`" atau All lalu jika ingin menampilkan beberapa field kita dapat menggunakan format hanya perlu memanggil nama fieldnya.

Lalu yang terakhir ialah kondisi "Where" dimana kita dapat memanggil nama field dengan menggunakan simbol aritmatika, misalnya kita ingin memanggil field "Nama_Pelanggan" tapi hanya ''Id_Pelanggan" 2 kita dapat menggunkan format seperti ini `SELECT Nama_Kolom FROM Nama_Table WHERE Id_Pelanggan=2;`

# update
struktur:
```mysql
update pelanggan set [nama_kolom]=nilai1 where [nama_kolom]=nilai2;
```
contoh:

```mysql
update pelanggan set nama_depan="nurul" where id_pelanggan=3;
```
program sebelum di ubah:
![[IMG_20240213_141351.jpg]]
program sesudah di ubah:
![[IMG_20240213_141403.jpg]]
## ==Delete==
Kita juga dapat menghapus baris pada table dengan *Query* **Delete**, untuk menghapus keseluruhan baris kita dapat menggunakan format seperti ini :
```mysql
Format :
DELETE FROM [Nama_Table] WHERE [Nama_Kolom];

Contoh :
DELETE FROM PELANGGAN WHERE Id_Pelanggan=6;
```

Berikut ialah contoh pengaplikasian dan hasil dari penggunaan **Delete** :

> [!Info]- Analisis
>> **Update** ialah *Query* untuk mengganti nilai yang telah ada pada sebuah table yang telah ada sebelumnya.
>> **Delete** ialah *Query* untuk menghapus baris pada sebuah tabel yang telah dibuat sebelumnya.
>> Penggunaan *Where* masih sangat berperan penting dalam kondisi seperti ini.

### Kesimpulan 
dua *Query* yang akan dipelajari selanjutnya ialah untuk mengganti data dan menghapus baris data pada table. *Query* nya ialah **Update** untuk mengganti data yang telah ada pada table, dan *Query* **Delete** untuk menghapus nilai yang telah ada pada table yang telah kita buat. kedua *Query* ini memiliki format yang lumayan mirip, dimana memerlukan *Where* untuk menuliskan kondisinya.
