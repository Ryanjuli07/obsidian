# AND
 select and ini akan menampilkan data dengan "nilai1" dan "nilai2".
 contoh:
 
 ```mysql
 select warna,pemilik from mobil where warna="hitam" and pemilik="ibrahim";
```

![[IMG_20240227_145125.jpg]]
## OR
select or ini akan menampilkan data dengan "nilai1" atau "nilai2".
contoh:

```mysql
select warna, pemilik from mobil where warna="hitam" or pemilik="Ibrahim";
```

![[IMG_20240227_145533.jpg]]

# BETWEEN- AND
select between-and ini akan menampilkan data antara "nilai1" dan "nilai2".karena didukung dengan AND.
CONTOH:

```mysql
select * FROM mobil WHERE harga_rental BETWEEN 100000 AND 200000;
```

![[IMG_20240227_150451.jpg]]
# NOT BETWEEN
## <=
untuk <= ini akan menampilkan "data" yang lebih kecil atau sama dengan "nilai_data yang telah ditentukan.
CONTOH:

```mysql
SELECT * FROM mobil WHERE harga_rental <= 50000;
```

![[IMG_20240227_151052.jpg]]
# >=
untuk >= ini akan menampilkan "data" yang lebih besar atau sama dengan "nilai_data yang telah ditentukan.
CONTOH:

```mysql
SELECT * FROM mobil WHERE harga_rental >= 50000;
```

![[IMG_20240227_151323.jpg]]
# <> atau !=
untuk <>atau != ini akan menampilkan "data" yang tidak sama dengan "nilai_data yang telah ditentukan.
CONTOH:

```mysql
SELECT * FROM mobil WHERE harga_rental <> 50000;
```

![[IMG_20240227_151707.jpg]]
ANALISIS:
SELECT adalah sebuah perintah query yang tugas memilih.
FROM adalah sebuah perintah query yang tugas nya untuk pemanggilan dari.
WHERE adalah sebuah perintah query yang tugas untuk menentukan pemanggilan yang mana ditujukannya.
MOBIL adalah sebuah nama tabel.
harga_rental adalah sebuah nama kolom.
500000 adalah nama data pada sebuah kolom.
<> adalah perintah query yang betugas menentukan syarat kurang dari atau lebih dari .

KESIMPULAN: query diatas adalah perintah untuk menampilkan sebuah data dari tabel mobil yang bertujukan pada kolom *harga rental* dengan data *LEBIH DARI ATAU  KURANG DARI  **500000**  jadi hanya data  dengan jumlah lebih dari 50000 atau kurang dari  500000 yang akan ditampilkan (selain dari nilai 500000 yang akan ditampilkan).

## Tantangan
Untuk tantangan saya akan mengambil nama pemilik "baim" dengan cara memanggilnya dengan syarat nomor pelatnya yaitu "B 1611 QC" lalu hasilnya akan seperti berikut :

## IN 

STRUKTUR:
```MYSQL 
 select * from nama_tabel where nama_kolom in ("nama_data","nama_data");
```

CONTOH:
```MYSQL 
 select * from data_mobil where warna in ("silver","merah");
```

analisis:
- **SELECT** adalah sebuah perintah query yang tugas memilih.
- **FROM** adalah sebuah perintah query yang tugas nya untuk pemanggilan dari.
- **WHERE** adalah sebuah perintah query yang tugas untuk menentukan 