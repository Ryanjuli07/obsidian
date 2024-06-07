# Web Dinamis
Pembagian jenis website di bagi menjadi dua bagian yaitu web statis dan web dinamis. Web statis adalah website yang hanya menampilkan sebuah output dari hasil program yang telah diketikkan sedangkan web dinamis adalah sebuah web yang lebih kompleks karena kita dapat memberi input pada website dan website tersebut dapat menyimpan data yang kita masukkan.
# PHP
PHP (Hypertext Preprocessor) adalah sebuah bahasa skrip dengan fungsi umum yang terutama digunakan untuk pengembangan sebuah web dinamis ataupun website interaktif. PHP juga mendukung banyak jenis database seperti MySQL, PostgreSQL dan Oracle sehingga pembangunan sebuah website dapat menjadi lebih kompleks

## Echo & Komentar 
Dalam php kita dapat mengetikkan sesuatu dengan kode "echo" dan menambahkan membuat sebuah komentar di penulisan program untuk penjelasan lebih lanjutnya akan dijelaskan di bawah ini. Dalam penulisan echo terdapat dua cara yaitu dengan kutip satu dan kutip dua, lalu untuk perbedaan antara keduanya akan dijelaskan lebih lanjut dibawah ini.
### Echo kutip satu
Untuk penulisan echo dengan kutip satu hasil yang akan tampil adalah seluruh yang ditulis di dalamnya dan hasil yang tampil akan terhitung sebagai string, walaupun ada variable yang dituliskan di dalam kutipnya. Untuk contoh programnya akan seperti berikut.
```php
echo 'Jumlah meja di kelas '. $meja . ' buah';
    echo "<br>";
```
### Echo kutip dua
Sedangkan untuk penulisan kutip dua akan menampilkan hasil dari variable maupun konstanta walapaun ditulis dalam kutip yang sama. Dan untuk contoh cara pengaplikasiannya akan seperti dibawah ini.
```php
echo "Shalat dlu, nabilang pak $wali_kelas dan $ketua_kelas";
    echo "<br>";
    echo "Kalau tidak, diracca' sama ketua gang $ketua_geng";
    echo "<br>";
```

### Komentar
Lalu untuk membuat komentar dalam kode program kita, kita dapat menggunakan dua cara yaitu `//` untuk komentar satu baris dan `/* */` untuk komentar multi baris. Dan untuk cara pengaplikasiaanya akan seperti di bawah ini
```php
//ini komentar satu baris
/*ini komentar
multi baris*/
```

## Variable & Konstanta
Dalam php kita dapat menuliskan variable dan kosntanta untuk menyimpan data yang akan digunakan kedepannya, untuk penjelasan lebih lanjutnya akan dijelaskan di bawah ini.
### Variable
Untuk penulisan variable kita awali dengan `$` lalu menuliskan nama variable nya dan menuliskan nilainya setelahnya dan di akhiri dengan `;`. Untuk contoh penggunaannya akan seperti di bawah ini.
```php
$meja = 30;
    $tk_kelas = "XI";
    $ketua_kelas = "July";
    $wali_kelas = "Saleh";
```

### Konstanta
Untuk konstanta berfungsi untuk menetapkan nilai dari sebuah data agar tidak dapat di ganti ganti kedepannya. Lalu untuk cara penulisannya akan seperti di bawah ini.
```php
const KEPSEK = "Herwelis";
define ('kelas', 'RPL 1');
```

## Operator
Dalam php juga kita dapat menggunakan operator operator untuk memudahkan penulisan program kita, Untuk penjelasan lebih jelasnya akan di dijelaskan di bawah.
### Aritmatika
Operator aritmatika berfungsi untuk penjumlah, pengurangan, perkalian dan pembagian. Untuk penggunaan akan seperti di bawah ini.
1. Penjumlahan
```php
    $a = 10;
    $b = 5;
    //Penambahan
    $penambahan = $a + $b;
    echo "penambahan: " . $Penambahan . "<br>";

```
> [! info]- Analisis Penambahan
>> `$a = 10;` : berfungsi sebagai variable yang memiliki nilai "10"
>> `$b = 5;` : berfungsi sebagai variable yang memiliki nilai "5"
>> `$penambahan = $a + $b;` : `$penambahan` berfungsi menyimpan variable dari hasil dari variable `$a` dan `$b`.
>> `echo "penambahan: " .$penambahan . "<br>;"` berfungsi untuk menampilkan hasil dari penambahan variable `$a` dan `$b`.

**Kesimpulan :**


2. Pengurangan
```php
	//pengurangan
    $Pengurangan = $a - $b;
    echo "Pengurangan: " . $Pengurangan . "<br>";
```
> [! info]- Analisis Penambahan
>> `$a = 10;` : berfungsi sebagai variable yang memiliki nilai "10"
>> `$b = 5;` : berfungsi sebagai variable yang memiliki nilai "5"
>> `$penambahan = $a - $b;` : `$pengurangan` berfungsi menyimpan variable dari hasil dari variable `$a` dan `$b`.
>> `echo "pengurangan: " .$pengurangan . "<br>;"` berfungsi untuk menampilkan hasil dari pengurangan variable `$a` dan `$b`.

**Kesimpulan :**

3. Perkalian
```php
	//perkalian
    $Perkalian = $a * $b;
    echo "Perkalian: " . $Perkalian . "<br>";
```
> [! info]- Analisis Penambahan
>> `$a = 10;` : berfungsi sebagai variable yang memiliki nilai "10"
>> `$b = 5;` : berfungsi sebagai variable yang memiliki nilai "5"
>> `$perkalian = $a + $b;` : `$perkalian` berfungsi menyimpan variable dari hasil dari variable `$a` dan `$b`.
>> `echo "perkalian: " .$perkalian . "<br>;"` berfungsi untuk menampilkan hasil dari perkalian variable `$a` dan `$b`.

**Kesimpulan :**
4. Pembagian
```php
	//pembagian
    $pembagian = $a / $b;
    echo "pembagian: " . $pembagian . "<br>";
```
> [! info]- Analisis Penambahan
>> `$a = 10;` : berfungsi sebagai variable yang memiliki nilai "10"
>> `$b = 5;` : berfungsi sebagai variable yang memiliki nilai "5"
>> `$pembagian = $a + $b;` : `$pembagian` berfungsi menyimpan variable dari hasil dari variable `$a` dan `$b`.
>> `echo "pembagian: " .$pembagian . "<br>;"` berfungsi untuk menampilkan hasil dari pembagian variable `$a` dan `$b`.

**Kesimpulan :**


### Perbandingan
Operator perbandingan atau operator perbandingan digunakan untuk membandingkan 2 operan atau lebih. Pada umumnya Operator perbandingan digunakan pada kondisi if-else sebagai penentu tingkat kesesuaian.

1. Perbandingan ==
```php
$a = 5;
$b = 10;
// Operator perbandingan ==
if ($a == $b) {
    echo "Nilai a sama dengan nilai b";
} else {
    echo "Nilai a tidak sama dengan nilai b";
}
```
> [! info]- Analisis Penambahan
>> `$a = 5;` : berfungsi sebagai variable yang memiliki nilai "10"
>> `$b = 10;` : berfungsi sebagai variable yang memiliki nilai "5"
>> `if ($a == $b) { echo "Nilai a sama dengan nilai b";` : jika nilai `$a` dan nilai `$b` sama makan akan menampilkan "Nilai a sama dengan nilai b"
>> `} else { echo "Nilai a tidak sama dengan nilai b";}` : Namun jika nilai `$a` dan nilai `$b` tidak sama maka akan menampilkan hasil "Nilai a tidak sama dengan nilai b"

**Kesimpulan :**

2. Perbandingan !=
```php
// Operator perbandingan !=
if ($a != $b) {
    echo "Nilai a tidak sama dengan nilai b";
} else {
    echo "Nilai a sama dengan nilai b";
}
```
> [! info]- Analisis Penambahan
>> `$a = 5;` : berfungsi sebagai variable yang memiliki nilai "10"
>> `$b = 10;` : berfungsi sebagai variable yang memiliki nilai "5"
>> `if ($a != $b) { echo "Nilai a tidak sama dengan nilai b";` : jika nilai `$a` dan nilai `$b` tidal sama makan akan menampilkan "Nilai a tidak sama dengan nilai b"
>> `} else { echo "Nilai a sama dengan nilai b";}` : Namun jika nilai `$a` dan nilai `$b` sama maka akan menampilkan hasil "Nilai a sama dengan nilai b"

**Kesimpulan :**

3. Perbandingan > dan <
```php
if ($a > $b) {
    echo "Nilai a lebih besar dari nilai b";
} else {
    echo "Nilai a tidak lebih besar dari nilai b";
}
```
> [! info]- Analisis Penambahan
>> `$a = 5;` : berfungsi sebagai variable yang memiliki nilai "10"
>> `$b = 10;` : berfungsi sebagai variable yang memiliki nilai "5"
>> `if ($a > $b) { echo "Nilai a lebih besar dari nilai b";` : jika nilai `$a` dan nilai `$b` tidal sama makan akan menampilkan "Nilai a lebih besar dari nilai b"
>> `} else { echo "Nilai a tidak lebih besar dari nilai b";}` : Namun jika nilai `$a` dan nilai `$b` sama maka akan menampilkan hasil "Nilai a tidak lebih besar dari nilai b"
>> **Namun jika tandanya berubah `<` maka hasilnya akan sebaliknya**

**Kesimpulan :**

4. Perbandingan >= dan =<
```php
if ($a >= $b) {
    echo "Nilai a lebih besar dari atau sama dengan nilai b";
} else {
    echo "Nilai a tidak lebih besar dari atau sama dengan nilai b";
}
```
> [! info]- Analisis Penambahan
>> `$a = 5;` : berfungsi sebagai variable yang memiliki nilai "10"
>> `$b = 10;` : berfungsi sebagai variable yang memiliki nilai "5"
>> `if ($a >= $b) { echo "Nilai a lebih besar dari atau sama dengan nilai b";` : jika nilai `$a` dan nilai `$b` tidal sama makan akan menampilkan "Nilai a lebih besar dari atau sama dengan nilai b"
>> `} else { echo "Nilai a tidak lebih besar dari atau sama dengan nilai b` : Namun jika nilai `$a` dan nilai `$b` sama maka akan menampilkan hasil "Nilai a tidak lebih besar dari atau sama dengan nilai b"
>> **Namun jika tandanya berubah `<=` maka hasilnya akan sebaliknya


### Logika

## Conditional Statement
### IF
### IF ELSE
### IF ELSE ELSE
### Switch Case

# Array
## Array 1 dimensi
## Array Asosiatif
## Array Multidimensi

## Var_Dump

## Looping (Pengulangan)
### For
### While
### Do-While
### Do-While
### Foreach

## Function

## PHP Form
### Get Method
### Post Method