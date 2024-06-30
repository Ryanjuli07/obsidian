# enco
```php
class Enco:
    def __init__(self):
        self._enco_kutip1 = ""
        self._enco_kutip2 = ""
    
    @property
        def enco_kutip1(self):
        return self._enco_kutip1

    @enco_kutip1.setter
    def enco_kutip1(self, value):
        self._enco_kutip1 = value
    
    @property
    def enco_kutip2(self):
        return self._enco_kutip2

    @enco_kutip2.setter
    def enco_kutip2(self, value):
        self._enco_kutip2 = value

# Contoh penggunaan
obj = Enco()
obj.enco_kutip1 = "Nilai pertama"
obj.enco_kutip2 = "Nilai kedua"

print(f"Enco Kutip 1: {obj.enco_kutip1}")
print(f"Enco Kutip 2: {obj.enco_kutip2}")

```

analisis
- class Enco: mendefinisikan sebuah kelas bernama Enco.
- __init__ adalah konstruktor yang digunakan untuk menginisialisasi properti enco_kutip1 dan enco_kutip2 dengan nilai awal berupa string kosong.
- @property mendefinisikan properti getter untuk enco_kutip1 dan enco_kutip2.
- @enco_kutip1.setter dan @enco_kutip2.setter mendefinisikan setter untuk enco_kutip1 dan enco_kutip2.
- Objek obj dibuat dari kelas Enco, dan nilai dari enco_kutip1 dan enco_kutip2 diatur serta dicetak ke layar.

Program ini memungkinkan Anda untuk mengatur dan mendapatkan nilai dari properti enco_kutip1 dan enco_kutip2 dengan cara yang terkontrol.
# komentar 
Lalu untuk membuat komentar dalam kode program kita, kita dapat menggunakan dua cara yaitu `//` untuk komentar satu baris dan `/* */` untuk komentar multi baris. Dan untuk cara pengaplikasiaanya akan seperti di bawah ini

```php
//ini komentar satu baris
/*ini komentar
multi baris*/
```
# variable
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
# operator aritmatika 
```python
# Program Operator Aritmatika

# Fungsi untuk menjumlahkan dua angka
def tambah(a, b):
    return a + b

# Fungsi untuk mengurangi dua angka
def kurang(a, b):
    return a - b

# Fungsi untuk mengalikan dua angka
def kali(a, b):
    return a * b

# Fungsi untuk membagi dua angka
def bagi(a, b):
    if b != 0:
        return a / b
    else:
        return "Pembagian dengan nol tidak diperbolehkan"

# Menu untuk memilih operasi
print("Pilih Operasi:")
print("1. Tambah")
print("2. Kurang")
print("3. Kali")
print("4. Bagi")

# Meminta pengguna untuk memilih operasi
pilihan = input("Masukkan pilihan (1/2/3/4): ")

# Meminta pengguna untuk memasukkan angka
angka1 = float(input("Masukkan angka pertama: "))
angka2 = float(input("Masukkan angka kedua: "))

# Melakukan operasi berdasarkan pilihan pengguna
if pilihan == '1':
    print(f"Hasil: {angka1} + {angka2} = {tambah(angka1, angka2)}")
elif pilihan == '2':
    print(f"Hasil: {angka1} - {angka2} = {kurang(angka1, angka2)}")
elif pilihan == '3':
    print(f"Hasil: {angka1} * {angka2} = {kali(angka1, angka2)}")
elif pilihan == '4':
    print(f"Hasil: {angka1} / {angka2} = {bagi(angka1, angka2)}")
else:
    print("Pilihan tidak valid")
    
```

analisis
Program ini meminta pengguna untuk memilih operasi aritmatika (penjumlahan, pengurangan, perkalian, atau pembagian), kemudian meminta pengguna untuk memasukkan dua angka, dan akhirnya menampilkan hasil dari operasi yang dipilih.
# perbandingan 
```python
# Program Perbandingan Dua Angka

# Fungsi untuk membandingkan dua angka
def bandingkan(a, b):
    if a > b:
        return f"{a} lebih besar dari {b}"
    elif a < b:
        return f"{a} lebih kecil dari {b}"
    else:
        return f"{a} sama dengan {b}"

# Meminta pengguna untuk memasukkan dua angka
angka1 = float(input("Masukkan angka pertama: "))
angka2 = float(input("Masukkan angka kedua: "))

# Menampilkan hasil perbandingan
hasil = bandingkan(angka1, angka2)
print(hasil)

```
# logika

```php
<!DOCTYPE html>
<html>
<head>
    <title>Operasi Logika</title>
</head>
<body>

<form method="post">
    <h3>Pilih Operasi Logika:</h3>
    <input type="radio" name="operation" value="AND"> AND<br>
    <input type="radio" name="operation" value="OR"> OR<br>
    <input type="radio" name="operation" value="NOT"> NOT<br><br>

    <label for="value1">Masukkan nilai pertama (True/False):</label><br>
    <input type="text" id="value1" name="value1"><br><br>

    <label for="value2">Masukkan nilai kedua (True/False):</label><br>
    <input type="text" id="value2" name="value2"><br><br>

    <input type="submit" name="submit" value="Hitung">
</form>

<?php
if ($_SERVER["REQUEST_METHOD"] == "POST") {
    $operation = $_POST['operation'];
    $value1 = filter_var($_POST['value1'], FILTER_VALIDATE_BOOLEAN, FILTER_NULL_ON_FAILURE);
    $value2 = filter_var($_POST['value2'], FILTER_VALIDATE_BOOLEAN, FILTER_NULL_ON_FAILURE);

    if ($operation == "AND") {
        $result = $value1 && $value2;
        echo "<h4>Hasil: $value1 AND $value2 = " . ($result ? "True" : "False") . "</h4>";
    } elseif ($operation == "OR") {
        $result = $value1 || $value2;
        echo "<h4>Hasil: $value1 OR $value2 = " . ($result ? "True" : "False") . "</h4>";
    } elseif ($operation == "NOT") {
        $result = !$value1;
        echo "<h4>Hasil: NOT $value1 = " . ($result ? "True" : "False") . "</h4>";
    } else {
        echo "<h4>Pilihan operasi tidak valid.</h4>";
    }
}
?>

</body>
</html>

```

analisis
- Program ini adalah aplikasi web sederhana menggunakan PHP.
- Ada formulir HTML yang memungkinkan pengguna untuk memilih operasi logika (AND, OR, NOT) dan memasukkan dua nilai boolean (True atau False).
- Setelah formulir disubmit, PHP memproses input, melakukan operasi logika yang dipilih, dan menampilkan hasilnya.
- filter_var digunakan untuk mengonversi string "True" atau "False" menjadi nilai boolean yang sesuai.
Simpan kode ini dalam file .php, lalu jalankan di server web yang mendukung PHP (seperti XAMPP atau WAMP) untuk melihat hasil nya
# Conditional Statement

```php
<!DOCTYPE html>
<html>
<head>
    <title>Conditional Statements in PHP</title>
</head>
<body>

<?php
// Mendapatkan nilai dari form jika sudah disubmit
if ($_SERVER["REQUEST_METHOD"] == "POST") {
    $nilai = $_POST['nilai'];

    // Contoh penggunaan if
    if ($nilai >= 60) {
        echo "Anda lulus!";
    }

    // Contoh penggunaan if-else
    if ($nilai >= 60) {
        echo "Anda lulus!";
    } else {
        echo "Anda tidak lulus.";
    }

    // Contoh penggunaan if-elseif-else
    if ($nilai >= 80) {
        echo "Nilai Anda sangat baik!";
    } elseif ($nilai >= 60) {
        echo "Nilai Anda cukup baik.";
    } else {
        echo "Anda perlu belajar lebih keras.";
    }
}
?>

<!-- Form untuk memasukkan nilai -->
<form method="post" action="<?php echo htmlspecialchars($_SERVER["PHP_SELF"]); ?>">
    Masukkan nilai ujian: <input type="text" name="nilai">
    <input type="submit" name="submit" value="Hitung">
</form>

</body>
</html>

```

analisis 
- Program PHP ini memiliki formulir HTML di mana pengguna dapat memasukkan nilai ujian.

- Setelah formulir dikirim `($_SERVER["REQUEST_METHOD"] == "POST")`, PHP akan mengambil nilai yang dimasukkan pengguna.

- Pernyataan if: Digunakan untuk mengevaluasi kondisi tunggal. Jika kondisi benar `($nilai >= 60)`, maka pesan "Anda lulus!" akan ditampilkan.

- Pernyataan `if-else`: Digunakan untuk mengevaluasi dua kondisi. Jika kondisi pertama benar `($nilai >= 60)`, maka pesan "Anda lulus!" ditampilkan; jika tidak, pesan "Anda tidak lulus." akan ditampilkan.

- Pernyataan `if-elseif-else:` Digunakan untuk mengevaluasi beberapa kondisi berurutan. Jika nilai lebih besar atau sama dengan 80, pesan "Nilai Anda sangat baik!" ditampilkan; jika nilai lebih besar atau sama dengan 60 tetapi kurang dari 80, pesan "Nilai Anda cukup baik." ditampilkan; jika nilai kurang dari 60, pesan "Anda perlu belajar lebih keras." akan ditampilkan.

- htmlspecialchars`($_SERVER["PHP_SELF"])` digunakan untuk mengamankan form dari serangan XSS `(Cross-Site Scripting)`.

Anda dapat menyimpan kode ini dalam sebuah file dengan ekstensi .php, lalu menjalankannya di server web yang mendukung PHP (seperti XAMPP atau WAMP) untuk melihat hasilnya. Pastikan untuk memasukkan nilai dan mengirim formulir untuk melihat output kondisional yang sesuai.
# array

```php
<!DOCTYPE html>
<html>
<head>
    <title>Contoh Program PHP dengan Berbagai Jenis Array</title>
</head>
<body>

<?php
// Array 1 dimensi berisi nama-nama buah
$buah = array("Apel", "Pisang", "Jeruk", "Mangga", "Anggur");

// Array multidimensi berisi data mahasiswa (nim, nama, dan nilai)
$mahasiswa = array(
    array("101", "John Doe", 85),
    array("102", "Jane Smith", 90),
    array("103", "Michael Johnson", 78)
);

// Array asosiatif berisi informasi seorang pegawai
$pegawai = array(
    "nama" => "John Doe",
    "jabatan" => "Manager",
    "gaji" => 5000000
);

// Menampilkan seluruh elemen array 1 dimensi
echo "<h2>Array 1 Dimensi (Nama-nama Buah):</h2>";
echo "<ul>";
foreach ($buah as $nama_buah) {
    echo "<li>$nama_buah</li>";
}
echo "</ul>";

// Menampilkan seluruh elemen array multidimensi (Data Mahasiswa)
echo "<h2>Array Multidimensi (Data Mahasiswa):</h2>";
echo "<table border='1'>";
echo "<tr><th>NIM</th><th>Nama</th><th>Nilai</th></tr>";
foreach ($mahasiswa as $data) {
    echo "<tr>";
    foreach ($data as $nilai) {
        echo "<td>$nilai</td>";
    }
    echo "</tr>";
}
echo "</table>";

// Menampilkan seluruh elemen array asosiatif (Informasi Pegawai)
echo "<h2>Array Asosiatif (Informasi Pegawai):</h2>";
echo "<ul>";
foreach ($pegawai as $key => $value) {
    echo "<li><b>$key:</b> $value</li>";
}
echo "</ul>";
?>

</body>
</html>

```

analisis
Program ini menggabungkan tiga jenis array: array 1 dimensi `($buah)`, array multidimensi `($mahasiswa)`, dan array asosiatif `($pegawai)`.

Array 1 Dimensi: Berisi nama-nama buah yang ditampilkan dalam bentuk daftar `(<ul>)`.

Array Multidimensi: Berisi data mahasiswa yang ditampilkan dalam bentuk tabel `(<table>)`.

Array Asosiatif: Berisi informasi seorang pegawai yang ditampilkan dalam bentuk daftar `(<ul>)`.
# looping (pengulangan)

```php
<!DOCTYPE html>
<html>
<head>
    <title>Contoh Program PHP dengan Berbagai Jenis Perulangan</title>
</head>
<body>

<?php
// Array berisi nama-nama buah
$buah = array("Apel", "Pisang", "Jeruk", "Mangga", "Anggur");

// Menampilkan seluruh elemen array menggunakan perulangan for
echo "<h2>Perulangan for:</h2>";
echo "<ul>";
for ($i = 0; $i < count($buah); $i++) {
    echo "<li>$buah[$i]</li>";
}
echo "</ul>";

// Menampilkan seluruh elemen array menggunakan perulangan while
echo "<h2>Perulangan while:</h2>";
$j = 0;
echo "<ul>";
while ($j < count($buah)) {
    echo "<li>$buah[$j]</li>";
    $j++;
}
echo "</ul>";

// Menampilkan seluruh elemen array menggunakan perulangan do-while
echo "<h2>Perulangan do-while:</h2>";
$k = 0;
echo "<ul>";
do {
    echo "<li>$buah[$k]</li>";
    $k++;
} while ($k < count($buah));
echo "</ul>";

// Menampilkan seluruh elemen array menggunakan perulangan foreach
echo "<h2>Perulangan foreach:</h2>";
echo "<ul>";
foreach ($buah as $nama_buah) {
    echo "<li>$nama_buah</li>";
}
echo "</ul>";
?>

</body>
</html>

```

 analisis
 Program ini menggunakan array $buah yang berisi nama-nama buah.

Perulangan for: Menampilkan seluruh elemen array menggunakan for dengan mengakses indeks dari 0 sampai jumlah elemen array.

Perulangan while: Menampilkan seluruh elemen array menggunakan while dengan menggunakan variabel counter ($j) yang ditambah setiap iterasi.

Perulangan do-while: Menampilkan seluruh elemen array menggunakan do-while yang pasti menjalankan satu kali iterasi minimal.

Perulangan foreach: Menampilkan seluruh elemen array menggunakan foreach untuk mengulangi setiap nilai dalam array $buah.
# function
```php
function greet($name) { 
echo "Hello, $name!"; } 

greet("Alice");
```

analisis 
function ini berfungsi untuk menjadi tempat untuk menyimpan data yang bisa di panggil berkali kali dan data atau nilai dari variable akan di isi di bagian bawah, seperti pada contoh di atas yang telah di tuliskan.
# php form

```php
<form>
     <input type="text" name="nama_lengkap" placeholder="Masukkan nama">
     <input type="number" name="umur" placeholder="Masukkan umur"><br>
     <button type="submit">Kirim</button>
</form>
```

analisis
form dalam php berfungsi untuk mengambil data yang akan dimasukkan di data base dan proses pembuatannya di lakukan atau diketikkan pada html.









 
