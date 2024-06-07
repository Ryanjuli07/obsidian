# ALTER
menambah kolom
```mysql
ALTER TABLE mobil ADD batas_peminjaman varchar(10) AFTER peminjam;
```

hasil
![[IMG_20240423_142342.jpg]]

## Penjelasan
- ALTER TABLE mobil: Perintah untuk mengubah struktur tabel mobil.
- ADD batas_peminjaman varchar(10): Menambahkan kolom baru dengan nama batas_peminjaman yang memiliki tipe data varchar(10).
- AFTER peminjam: Menentukan bahwa kolom baru akan ditambahkan setelah kolom peminjam dalam struktur tabel.

setelah menambahkan kolom kita dapat mengisi kolom tersebut dengan query
```mysql
update mobil set batas_peminjam="20-07-07" where id_pelanggan>3;
```

hasil
![[IMG_20240423_143341.jpg]]

mengubah nama kolom
```mysql
alter table mobil change column batas_peminjam deadline varchar(10);
```

hasil
![[IMG_20240423_144705.jpg]]

mengubah tipe data kolom
```mysql
alter table mobil modify deadline date;
```

hasil
![[IMG_20240423_145820.jpg]]
menambahkan constraint
```mysql
alter table mobil alter deadline set default 'ready';
```

hasil
![[IMG_20240423_151637.jpg]]
 menghapus kolom
 ```mysql
 alter deadline drop default;
```

hasil
![[IMG_20240423_152300.jpg]]

mengubah nama kolom
```mysql
alter table daftar_mobil rename to mobil;
```

Penjelasan
- ALTER TABLE mobil:  adalah perintah untuk mengubah struktur tabel yang ada, dalam hal ini, tabel mobil.
- MODIFY deadline DATE:  adalah bagian dari perintah ALTER TABLE yang menentukan perubahan yang diinginkan. Contoh menggunakan klausa `MODIFY`untuk mengubah tipe data kolom deadline menjadi DATE.
### Kesimpulan
ALTER TABLE mobil MODIFY deadline DATE; digunakan untuk mengubah tipe data kolom `deadline`dalam tabel mobil menjadi tipe data DATE.berguna untuk memastikan bahwa kolom deadline dapat menyimpan tanggal dengan format yang benar