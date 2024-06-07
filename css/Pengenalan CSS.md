##### Pertemuan 8
# Anatomi CSS
Anatomi css terdiri dari *Selector, Property* dan *Property Value* untuk contoh lebih jelasnya kita akan masuk kedalam contoh dibawah dimana akan dijelaskan contoh dari ketiga anatomi css.
    
**contoh program :**
```css
p {
	color: red;
}
```
**hasil program :** 
 ![Gambar](Aset/IMG8/IMG8_1.png)
> [!info]- Penjelasan
>>Jadi pada contoh program di atas *P* berperan sebagai **selector** lalu *color* berperean sebagai **Property** dan *Red* berperan sebagai **Property Value**.


# Div & Span
DIV adalah elemen tingkat blok yang digunakan untuk membuat bagian, sedangkan SPAN adalah elemen sebaris untuk menata teks atau elemen sebaris lainnya

> [!Info]- Div 
>>Div ialah tag yang digunakan untuk mengetikkan sesuatu namun cakupan areanya akan 
>>mengambil satu block/baris. 
 
> [!info]- span
>>Span ialah tag yang digunakan untuk mengetikkan sesuatu namun cakupan areanya akan mengambil sesuai yang diketikkan saja.
### Perbedaan div & span
Perbedaanya terletak di cakupan area/area box yang di ambilnya contoh nya seperti yang sudah dijelaskan di atas yaitu div mengambil cakupan satu baris sedangkat span hanya mengambil cakupan sesuai yang diketikkan saja, untuk contohnya akan seperti dibawah ini :
![Gambar](Aset/IMG8/IMG8_2.png)


# Tantangan I
## Percobaan I
**Kode CSS :**
```css
<style>
       p {
          color: red;
         }
</style>
  
      <p>Welcome CSS</p>
```
**Hasil program :**
![Gambar](Aset/IMG8/IMG8_3.png)

> [!info]- Penjelasan 
>> disini isi dari tag p berubah menjadi berwarnah merah di akibatkan oleh style css tepatnya property color yang dibarengi dengan value red sehinggan hasil dari tag p yang telah dipanggil oleh style css berubah menjadi warna merah.
>>  


# Percobaan II
**Kode CSS :
```css
<style>
	button {
            width:150px;
            height: 50px;

            font-weight: bold;
            text-transform: uppercase;
            border-radius: 5px;
    }
</style>
```


### Font-weight
**Before :
![Gambar](Aset/IMG8/IMG8_4.png)
After :**
![Gambar](Aset/IMG8/IMG8_5.png)

> [!info]- Penjelasan *font weight*
>> untuk font-weight ini akan merubah ketebalan teks dan contohnya disini kita mengguanakan *property value* yang bold sehingga merubah teksnya menjadi tebal 

### Text-transform
**Before :
![Gambar](Aset/IMG8/IMG8_4.png)
After :**
![Gambar](Aset/IMG8/IMG8_6.png)

> [!Info]- Penjelasan *Text transfrom*
>> Untuk teks tranfrom kita menggunakan property value uppercase sehingga mengubah tulisan yang telah di ketikkan berubah menjadi huruf capital

### Border-radius
**Before :
![Gambar](Aset/IMG8/IMG8_4.png)
After :**
![Gambar](Aset/IMG8/IMG8_7.png)

> [!Info]- Penjelasan *Border radius*
>> Untuk border radius ini dapat menebalkan atau memperluas jarak dari tepi border sesuai yang kita inginkan


# Pemanggilan CSS
untuk pemanggilan css dibagi menjadi tiga bagian/cara dan ketiga cara tersebut akan dijelaskan di materi di bawah, untuk lebih jelasnya kita akan langsung masuk ke materi dari tiga cara pemanggilan tersebut.

## Inline
Untuk *Inline* pemanggilannya ialah langsung bersamaan dengan tag yang ingin diketikkan misalnya seperti kode program berikut :
```html
<p style=color: red;>ini cara pemanggilan css inline</p>
```
## Internal
Lalu untuk *internal* cara pemanggilannya ialah dengan diketikkan di dalam dokumen html yang telah kita buat namun berbeda dengan *Inline*, contoh nya ialah seperti kode program dibawah berikut :
```html
<head>
	<style>
		p {
		 color: red;
		}
	</style>
</head>
<body>
	<p>ini adalah pemanggilan css internal </p>
</body>
```
## External
Sedangkan *External* cara pemanggilan ini ialah dengan membuat dokumen khusus css lalu menghubungkan antara dokumen html dan css dengan tag `<link>` untuk contoh programnya akan seperti berikut :
```html
<head>
	<link rel="stylesheet" href="nama_dokumen_css.css"
</head>
```


# Selector
Untuk selector css dibagi menjadi 3 cara yaitu *Elemen Selector, Class selector* dan *Id selector*
untuk penjelasan kebih lanjutnya akan kita bahas di materi di bawah ini.
## Elemen selector
Untuk Elemen selector kita melakukan pemanggilan di dalam dokumen html dengan menyebutkan nama tag nya misalnya ialah seperti di bawah ini :
```html
<style>
	div {
	 color: red;
	}
</style>
```
## Class selector
Untuk Class selector kita memanggil di dokumen khusus *css* dan menambahkan atribut class pada tag yang ingin di ubah lalu dipanggil menggunakan "." sebelum nama classnya, untuk contoh programnya akan seperti berikut.
**Halaman html :**
```html
<span class="nama_class">Ini contoh class selector</span>
```
**Halaman css :**
```css
.nama_class {
	color: red;
}
```
## Id selector
Untuk Id selector lumayan mirip dengan class selector yaitu dengan menambahkan id di tag yang ingin di ubah lalu setelah itu di panggil menggunakan tagar sebelum nama id nya, untuk contoh programnya akan seperti berikut.
**halaman html :**
```html
<div id="nama_id">Ini contoh id selector<div>
```
**halaman css :**
```css
#nama_id {
	color: red;
}
```


# Text,Background & Font
property dasar yang akan kita pelajari ialah mulai dari text font dan background untuk penjelasan yang lebih jelas akan dijelaskan di materi dibawah ini.

## ==Materi Text==
Untuk  property text kita akan mempelajari beberapa value dan untuk lebih jelasnya kita akan mempelarinya di bawah ini.

#### Text-Align
text align ini mengatur rata kiri kanan dari sebuah teks yang akan di ketik dan seperti value yang saya gunakan ialah untuk mengatur tulisannya menjadi tengah dengan value *"center"* dan contoh programnya ialah seperti berikut :
```css
.text_align {
    text-align: center;
}
```
dan hasilnya akan seperti berikut :
![Gambar](Aset/IMG8/IMG8_8.png)

#### Text-Decoration
text-decoration berfungsi untuk memberi dekorasi pada teks yang akan ditulis sesuai dengan value yang akan digunakan seperti contoh yang saya ambil yaitu *"underline"* yang berfungsi untuk membuat garis dibawah tulisan, untuk contohnya akan seperti berikut :
```css
.text_decoration {
    text-decoration:underline;
}
```
dan hasilnya akan seperti berikut :
![Gambar](Aset/IMG8/IMG8_9.png)

#### Text-Trasformation
text-transformation ini berfungsi untuk mengtransformasikan teks yang telah dibuat seperti contoh yang saya gunakan ialah membuat teks menjadi kapital menggunakan value *"uppercase"* untuk contohnya akan seperti dibawah ini :
```css
.text_transformation {
    text-transform:uppercase;
}
```
dan hasilnya akan seperti berikut :
![Gambar](Aset/IMG8/IMG8_10.png)

#### Teks-Indent
teks-indent ini berfungsi untuk memberi jarak di awal penulisan atau simpelnya seperti mengetik "tab" pada keayboard kita dan untuk valuenya dapat di isi sesuai dengan keinginan kita. Contohnya akan seperti berikut :
```css
.text_indent {
    text-indent: 20px;
}
```
dan hasilnya akan seperti berikut :
![Gambar](Aset/IMG8/IMG8_11.png)

#### Letter-Spacing
lalu untuk latter-spacing ialah untuk memberi jarak di antara setiap huruf yang telah diketikkan dan untuk valuenya dapat ditentukan sesuai keignginan kita, untuk lebih jelasnya berikut contoh program dan asilnya :
```css
.letter_spacing {
    letter-spacing: 6px;
}
```
dan hasilnya akan seperti berikut :
![Gambar](Aset/IMG8/IMG8_12.png)

#### Line-Height
untuk line-height ialah untuk memberi jarak pada suatu teks dengan teks di atasnya dan valuenya dapat di atur sesuai dengan keinginan, lalu untuk contoh program serta hasilnya akan seperti dibawah ini :
```css
.line_height {
    line-height: 100px;
}
```
dan hasilnya akan seperti dibawah ini :
![Gambar](Aset/IMG8/IMG8_13.png)

#### Word-Spacing
dan terakhir ialah word-spacing fungsinya untuk memberi jarak di antara setiap kata dan valuenya dapat di atur sesuai keinginan kita, lalu untuk contoh program dan hasilnya akan seperti berikut :
```css
.word_spacing {
    word-spacing: 10px;
}
```
dan hasilnya akan seperti berikut :
![Gambar](Aset/IMG8/IMG8_14.png)


## ==Materi Background==
Untuk  property background kita akan mempelajari beberapa value dan untuk lebih jelasnya kita akan mempelarinya di bawah ini.

#### Background-Image
untuk background image ini kita akan dapat menampilkan background dengan image sesuai dengan yang ingin kita pilih/dari file kita, untuk contoh programnya akan seperti berikut :
```css
.background-image {
    background-image:url(./aset/backgroundd.JPG)
}
```
dan hasilnya akan speeri berikut :
![Gambar](Aset/IMG8/IMG8_15.png)

#### Background-Size
lalu untuk background size kita mengatur size/ukuran dari background yang kita gunakan dan valuenya dapat kita atur sesuai dengan keinginan kita. untuk contoh penggunananya akan seperti berikut ini :
```css
.background {
    background-image:url(./aset/backgroundd.JPG);
    width: 100%;
    height: 100VH;
    
    background-size: 50%;
}
```
dan hasilnya akan seperti berikut :
![Gambar](Aset/IMG8/IMG8_16.png)

#### Background-Repeat
untuk background-repeat ini mengulang gambar dalam ukurannya dan untuk penggunaannya akan seperti dibawah ini:
```css
.background {
    background-image:url(./aset/backgroundd.JPG);
    width: 100%;
    height: 100VH;
    background-size: 50px;
    
    background-repeat: repeat;
}
```
dan hasilnya akan seperti dibawah ini :
![Gambar](Aset/IMG8/IMG8_17.png)


#### Background-Attachment
background-attachment ini mengatur ketetapan image yang di gunakan contohnya ialah seperti penggunaan value "fixed" yang membuat gambar tetap berada di posisinya walau di scroll, untuk contoh penggunaanya akan seperti berikut :
```css
.background {
    background-image:url(./aset/backgroundd.JPG);
    width: 100%;
    height: 50px;
    background-size: 90%;
    
    background-attachment: fixed;
}
```
dan hasilnya akan seperti berikut :
![Gambar](Aset/IMG8/IMG8_18.png)


#### Background-Postion
dan yang terakhir ialah background-postion dan fungsinya ialah untuk mengatur posisi dari background yang digunakan, untuk contoh penggunaanya aka seperti dibawah ini :
```css
.background {
    background-image:url(./aset/backgroundd.JPG);
    width: 100vh;
    height: 100vh;
    background-size: 50%;
    background-repeat: no-repeat;
    
    background-position:10% ,50% ;
}
```
dan hasilnya akan seperti dibawah ini :
![Gambar](Aset/IMG8/IMG8_19.png)


## ==Materi Font==
Untuk  property font kita akan mempelajari beberapa value dan untuk lebih jelasnya kita akan mempelarinya di bawah ini.


#### Font-Size
untuk font-size berfungsi untuk mengatur ukuran dari teks yang di ketikkan dan valuenya dapat di atur sesuai dengan keinginan kita, untuk contoh program dan hasilnya akan seperti dibawah ini :
```css
.teks {
    font-size: 10px;
}
```
dan hasilnya akan seperti dibawah ini :
![Gambar](Aset/IMG8/IMG8_20.png)

#### Font-Style
untuk font-style berfungsi untuk mengatur gaya dari teks yang diketikkan untuk value bisa dipilih sesuai dengan yang kita inginkan, contohnya saya disini saya menggunakan *italic* untuk program dan hasilnya akan seperti dibawah ini :
```css
.teks {
    font-size: 10px;
    font-style:italic;
}
```
dan hasilnya akan seperti dibawah ini :
![Gambar](Aset/IMG8/IMG8_21.png)


#### Font-Weight
untuk font-weight adalah untuk mengatur ketebalan dari teks yang kita ketikkan dan untuk valuenya dapat kita pilih sesuai dengan keinginan kita dan disini saya menggunakan value *bold* untuk contoh programnya akan seperti berikut :
```css
.teks {
    font-size: 10px;
    font-style:italic;
    font-weight:bold;
}
```
dan hasilnya akan seperti berikut :
![Gambar](Aset/IMG8/IMG8_22.png)


#### Font-Family
dan yang terakhir ialah font-family ialah untuk mengatur jenis font yang diinginkan seperti contoh yang saya gunakan ialah value *arial* dan contoh program serta hasilnya akan seperti berikut :
```css
.teks {
    font-size: 10px;
    font-style:italic;
    font-weight:bold;
    font-family:arial;
}
```
dan hasilnya akan seperti berikut :
![Gambar](Aset/IMG8/IMG8_23.png)



# Box model
Untuk box model kita akan mempelajari mengenai border, padding, margin dan hal hal lainnya mengenai permodelan box. untuk lebih jelasnya kita akan menggunakan contoh di bawah :
![Gambar](Aset/IMG9/IMG9_1.png)

untuk membuat button dengan model di atas kita akan menggunakan beberapa style disini saya akan menjelaskan mengenai border dan padding pada button ini namun saya tidak akan menjelaskan mengenai style lainnya dikarenakan telah di jelaskan di materi sebelumnya, berikut ialah style style yang digunakan :
```css
.button {
    width: 200px;
    height: 75px;
    background-color: aquamarine;
    font-weight: bold;
    text-transform:uppercase;

    border-radius:10px;
    border-width: 6px;
    border-color: blue;
    border-style: solid;
  
    padding-left:100px;
    padding-bottom: 50px;
    padding-right: 2px;
    padding-top:2px;
}
```

## Tantangan II
**Kode Program Html :**
```html
<!DOCTYPE html>
<html>
<head>
    <title>Website</title>
    <link rel="stylesheet" href="Web_Fachri.css">
</head>
<body class="background">
    <Span>
        <div class="span">
            Selamat datang
        </div>
    </Span><br>
    <span class="span">di <b class="font">Web Fachri !</b></span>
    <img src="./Aset/aset1.jpg" class="foto">
    <button class="button">Klik Disini</button>
</body>
</html>
```
**Kode Program CSS :**
```css
.background {
    background-color: purple;
}

.span {
    font-size: 80px;
    color: white;
    margin-top: 135px;
    margin: left 10px;
    
}

.font{
    font-family: Arial, Helvetica, sans-serif;
}

.foto {
    display: block;
    height: 400px;
    width: 400px;
    margin-left: 700px;
    margin-top: -200px;
    border-width: 10px;
    border-color: white;
    border-style: solid;
    border-radius: 1000px;
    
}

.button {
    display:block;
    width: 160px;
    height: 85px;
    background-color: transparent;
    border-width: 3px;
    border-color: rgb(247, 43, 43);
    color:rgb(247, 43, 43) ;
    border-style: solid;

    margin-top: -150px;
    margin-left: 400px;

    padding-top:10px;
    padding-bottom: 20px;
    padding-right: 40px;
    padding-left: 40px;

}
```
**Hasilnya akan seperti berikut :**
![Gambar](Aset/IMG9/IMG9_3.png)


## ==Border==
untuk border terdapat beberapa jenis yang akan digunakan mulai dari radius,width,color dan style untuk penjelasan lebih lanjutnya akan dijelaskan di sub materi di bawah.
#### Border-Radius
Untuk border-radius ini berfungsi untuk mengatur radius pada border, semakin tinggi radius semakin berkurang radius pada bordernya/semakin melengkung.
#### Border-Width
Untuk border-width ini berfungsi menebalkan border atau menebalkan radius pada border dan dapat ditebalkan sesuai value yang diinginkan disini saya menggunakan value *10px* sehingga ketebalannya bertambah lebih dari biasanya.
#### Border-Color
Untuk border-color ini untuk mengatur warna border yang telah dibuat dan valuenya dapat di atur sesuai dengan keinginan kita, valuenya ini berupa warna.
#### Border-Style
Dan Terakhir ialah border-style, border-style ini kita dapat menggunakan value solid untuk membuat bordernya memiliki warna solid dan tanpa bayangan/shadow.


## ==Padding==
untuk padding terdapat beberapa jenis yang akan digunakan mulai dari right,left,top dan bottom untuk penjelasan lebih lanjutnya akan dijelaskan di sub materi di bawah.
#### Padding-Left
Padding-left ini berfungsi untuk mengatur jarak antara objek dengan bordernya khusus untuk bagian sebelah kiri.
#### Padding-Right
Padding-right ini berfungsi untuk mengatur jarak antara objek dengan bordernya khusus untuk bagian sebelah kanan.
#### Padding-Top
Padding-top ini berfungsi untuk mengatur jarak antara objek dengan bordernya khusus untuk bagian sebelah atas.
#### Padding-Bottom
Padding-bottom ini berfungsi untuk mengatur jarak antara objek dengan bordernya khusus untuk bagian sebelah bawah.


## Contoh Border Lain
Untuk contoh border kedua ialah menggunakan margin untuk mengatur jarak buttonnya menggunakan padding  contohnya akan seperti di bawah ini :
![Gambar](Aset/IMG9/IMG9_2.png)

## ==Margin== 
Fungsi dari margin yang akan kita pelajari ialah fungsi dari margin right,left,top dan bottom. Untuk lebih jelasnya akan dijelaskan di bawah ini.

#### Margin-Right
Margin-right ini mengatur jarak antar objek satu dengan objek lainnya lebih tepatnya ke arah kanan objeknya.
#### Margin-Left
Margin-left ini mengatur jarak antar objek satu dengan objek lainnya lebih tepatnya ke arah kiri objeknya.
#### Margin-Top
Margin-top ini mengatur jarak antar objek satu dengan objek lainnya lebih tepatnya ke arah atas objeknya.
#### Margin-Bottom
Margin-bottom ini mengatur jarak antar objek satu dengan objek lainnya lebih tepatnya ke arah bawah objeknya.

# Pseudo-classes

## Hover
- `button:hover`: adalah pseudo-class selector yang menargetkan tombol (button) ketika pengguna mengarahkan kursor ke atasnya (hover) atau diklik. 
- `background-color: red;`: Properti ini menetapkan warna latar belakang tombol menjadi merah ketika tombol sedang di-hover.
- `color: white;`: Properti ini menetapkan warna teks pada tombol menjadi putih ketika tombol di-hover.
- `height: 100px;`: Properti yang digunakan untuk membuat  tinggi (height) tombol menjadi 100 piksel ketika tombol di-hover.
- `width: 100px;`: Properti yang digunakan untuk membuat lebar (width) tombol menjadi 100 piksel ketika tombol di-hover.
**Kode program :**
```
button:hover{
  background-color:red;
  color:white;
  height:100px;
  
  width:100px;

}
```
**Hasil :**
![Gambar](Aset/IMG10/IMG10_1.png)
#### Kesimpulan
property dalam style button yang diberi hover akan mengubah button pada saat kursor di arahkan ke arah objek (Hover) sesuai degan yang di isikan di `button:hover` seperti yang telah nampak di atas. 

## Active
`button:active`: adalah pseudo-class selector yang menargetkan tombol (`button`) ketika tombol tersebut sedang dalam keadaan "active", atau tombol sedang ditekan. 
`color: yellow;`: Properti memberikan warna kuning pada teks ketika tombol sedang active atau tombol sedang ditekan. 
**Kode program :**
```
button:active{
  color: yellow ;
}
```
**Hasil :**
![Gambar](Aset/IMG10/IMG10_2.png)
#### Kesimpulan
Teks "klik broo" akan berganti warna menjadi kuning jika ditekan sesuai dengan program di atas. 

# Transition 
### Penjelasan
+ `Transition`:  untuk mengatur pertunjukan perubahan, mengubah penampilan elemen dari satu keadaan ke keadaan lain, memberikan dinamika visual yang menarik dalam desain web Anda.
+ `Transition-delay`: properti ini memberikan momen kejutan atau antisipasi sebelum perubahan yang dijanjikan terjadi, menambah dramatisasi pada tampilan elemen.
- `Transition-duration`: menentukan lamanya waktu ketika elemen berubah, memungkinkan Anda untuk mengatur seberapa lama penonton (pengguna) menikmati perubahan tersebut.
- `Transition-property`: menentukan apa yang akan berubah, seperti warna, ukuran, atau posisi, menciptakan efek transisi yang beragam dan menarik.
- `Transition-timing-function`:  properti ini mengatur ritme perubahan, menentukan apakah transisi akan bergerak dengan lembut dan halus seperti aliran air, atau tiba-tiba dan dramatis seperti petir yang menyambar.
**Kode program :**
```
button:hover{
  transition:all 0.9s ease-in;  
}
```

## Tantangan III
### Penjelasan HTML
- Tag `<DOCTYPE html>` memberitahu web bahwa dokumen HTML adalah versi 5
- Tag pembuka `<html>` menandai awal sebuah dokumen HTML sampai dengan tag penutup `</html>`
- Tag pembuka `<head>` berisi informasi tentang halaman HTML sampai dengan tag penutup `</head>` ,biasanya dalam tag head terdapat tag `<title>` untuk memberikan informasi judul halaman HTML
- Apapun tag yang berada di antara tag pembuka `<body>` sampai dengan tag penutup `</body>` akan tampil di web browser.
- `<title>`: Menentukan judul halaman.
- `<link rel="stylesheet" href="transition.css">`: Menghubungkan dokumen dengan stylesheet eksternal.
- `<body class="main-container">`: Memulai konten utama halaman dengan kelas "main-container".
- `<div class="hero-container">`: Kontainer utama untuk semua konten.
- `<div class="box-container">`: Kontainer untuk setiap kotak konten.
- `<h1 class="item box-item-1">Selamat Datang</h1>`: Teks "Selamat Datang" dengan kelas "item" dan "box-item-1".
- `<h1 class="item box-item-2">di <b>Web Nero</b></h1>`: Teks "di Web Fadhil" dengan kelas "item" dan "box-item-2", kata "Web Fadhil" ditebalkan.
- `<div class="item box-item-3">`: Kontainer untuk tombol "Klik disini" dengan kelas "item" dan "box-item-3".
- `<button class="button">Klik disini</button>`: Tombol dengan teks "Klik disini" dan kelas "button".
- `<div class="item-box">`: Kontainer untuk gambar.
- `<img src="aset/nero.jpg.png">`: Gambar "F.png" dari direktori "camera".
## Penjelasan CSS
- `body`: Mengatur latar belakang seluruh halaman menjadi warna ungu (purple).
- `.main-container`: Memberikan latar belakang warna ungu (purple) pada elemen dengan kelas "main-container". Ini mungkin digunakan sebagai wadah utama untuk konten.
- `.box-item-1 dan .box-item-2`: Mengatur tampilan teks pada elemen-elemen dengan kelas "box-item-1" dan "box-item-2". Ini termasuk mengatur ukuran font menjadi 50px, warna putih, dan memberikan jarak atas sejauh 10px.
- `.button:hover`: Mengatur tampilan tombol dengan kelas "F" saat kursor berada di atasnya (hover). Saat tombol di-hover, ukurannya diperbesar, warna dan border berubah, dan posisinya digeser ke kiri dengan transisi animasi selama 0.9 detik.
- `button:active`: Memberikan efek transformasi rotasi sebesar 45 derajat pada tombol ketika tombol sedang aktif (ditekan).
- `img`: Mengatur tampilan gambar dengan lebar dan tinggi masing-masing 250px, dengan sudut melingkar sebesar 200px, serta menetapkan margin kiri sejauh 400px dan margin atas sejauh -400px. Hal ini dapat mempengaruhi posisi dan tata letak gambar dalam halaman.

### Kode Program
```HTML
<!DOCTYPE html>
<html>
<head>
    <title>Belajar CSS3</title>
    <link rel="stylesheet" href="transition.css">
</head>
<body class="main-container">
    <div class="hero-container">
    <div class="box-container">
    <h1 class="item box-item-1">
    Selamat Datang
    </h1>
    
    <h1 class="item box-item-2">
    di <b>Web Fadhil</b>
    </h1>
    <div class="item box-item-3">
    <button class="button">Klik disini</button>
    </div>
    </div>
    
    <div class="box-container">
    <div class="item-box">
    <img src="aset/nero.jpg">
    </div>
        </div>
    </div>
</body>
</html>

```

```CSS
body{
  background-color:purple;
}
.main-container {
    background-color: purple;
}
.box-item-1{
    font-size: 50px;
    color: white;
    margin-top:10px;
    }
.box-item-2{
   font-size: 50px;
    color: white;
    margin-top:10px;
}

.button:hover {
    background-color: purple;
    margin-left:200px;
    padding-left:29px;
    padding-top:20px;
    padding-bottom:25px;
    padding-right:29px;
    color: orangered;
    border-color:orangered;
    margin-top: 50px; 
    margin-right:60px;
    margin-bottom:90px;
   transition:all 0.9s ease-in; 
}
 button:active{ 
  transform:rotate(45deg);
  }
img{
    width: 250px;
    height: 250px;
    border-radius: 200px;
    border-color: white;
    border-style: solid;
    margin-left: 400px;
    margin-top: -400px;
}

```
**Hasil Before :**
![Gambar](Aset/IMG10/IMG10_4.png)
**Hasil After :**
![Gambar](Aset/IMG10/IMG10_5.png)


# Transform 
### Penjelasan
- `transform: scale(0.5);`= Mengubah ukuran elemen menjadi setengah dari ukuran aslinya.
- `transform: scalex(0.5);`= Hanya mengubah skala elemen secara horizontal menjadi setengah dari ukuran aslinya.
- `transform: rotate(45deg);`= Memutar elemen sebesar 45 derajat searah jarum jam.
- `transform: skewX(-25deg);`= Membengkokkan elemen secara horizontal sebesar -25 derajat (ke arah kiri).
- `transform: skew(25deg,5deg);`= Membengkokkan elemen sebesar 25 derajat secara horizontal (ke kanan) dan 5 derajat secara vertikal (ke atas).
- `transform: translate(50px,52px);`= Menggeser elemen sebesar 50 piksel ke kanan dan 52 piksel ke bawah.
- `transform: matrix(0.7,-0.5,0.5,0.4,0.5,0.7);`= Menggambarkan transformasi menggunakan matriks 2D den
**Kode Program :**
```
button:active{
  
  transform:matrix(0.7,-0.5,0.5,0.4,0.5,0.7);
  }
```
**Hasil :**
![Gambar](Aset/IMG10/IMG10_3.png)

#### Kesimpulan
Setiap properti transform mengubah tampilan elemen dengan cara yang berbeda-beda sesuai dengan property. 

# Flexbox 
## Flex Container
#### Display Flex
`display: flex`, kita dapat dengan mudah mengatur tata letak elemen-elemen di dalamnya dengan properti-properti seperti `flex-direction`, `justify-content`, `align-items`, dan lain-lain.
##### Kesimpulan
`display: flex`, kita dapat dengan mudah mengatur tata letak elemen-elemen di dalamnya menggunakan properti-properti seperti `flex-direction`, `justify-content`, `align-items`, dan properti lainnya yang terkait dengan model tata letak flexbox.


#### Flex-Direction
- `flex-direction: column;`: Mengatur tata letak dari flex container menjadi vertikal, sehingga flex items diatur dari atas ke bawah.
- `flex-direction: column-reverse;`: Mengatur tata letak dari flex container menjadi vertikal terbalik, sehingga flex items diatur dari bawah ke atas.
- `flex-direction: row;`: Mengatur tata letak dari flex container menjadi horizontal, sehingga flex items diatur dari kiri ke kanan.
- `flex-direction: row-reverse;`: Mengatur tata letak dari flex container menjadi horizontal terbalik, sehingga flex items diatur dari kanan ke kiri.
**Kode Program :**
```css
.box-container{
  flex-direction: column;  
}
```
##### Kesimpulan
Setiap properti flex-direction mengubah tampilan elemen dengan cara yang berbeda-beda sesuai dengan property. 
Contoh`column` untuk tata letak vertikal dari atas ke bawah.
`column-reverse` untuk tata letak vertikal terbalik dari bawah ke atas. `row` untuk tata letak horizontal dari kiri ke kanan.`row-reverse` untuk tata letak horizontal terbalik dari kanan ke kiri.

#### Align-Items
- `align-items: center;`: Flex items akan diatur di tengah-tengah sumbu silang dari flex container.
- `align-items: flex-start;`: Flex items akan diatur pada awal sumbu silang dari flex container.
- `align-items: flex-end;`: Flex items akan diatur pada akhir sumbu silang dari flex container.
- `align-items: baseline;`: Flex items akan diatur sedemikian rupa sehingga garis dasar dari teks pada masing-masing item berada pada level yang sama.
- `align-items: stretch;`: Flex items akan diperpanjang untuk mencapai tinggi maksimal flex container, mengisi ruang kosong di sepanjang sumbu silang.
**Kode Program :**
```css
.box-container{
  align-items:center ;  
}
```

##### Kesimpulan
Setiap properti align-items mengubah tampilan elemen dengan cara yang berbeda-beda sesuai dengan property. 
Contoh`center` untuk menempatkan flex items di tengah-tengah sumbu silang.`flex-start` untuk menempatkan flex items di awal sumbu silang.`flex-end` untuk menempatkan flex items di akhir sumbu silang.`baseline` untuk menempatkan flex items sehingga garis dasar teks masing-masing item berada pada level yang sama.`stretch` untuk memperpanjang flex items sehingga mencapai tinggi maksimal flex container, mengisi ruang kosong di sepanjang sumbu silang.

#### Justify-Content
 - `justify-content: flex-start;`: Mengatur fleks item ditempatkan di bagian awal (mulai) dari sumbu utama flex container.
- `justify-content: flex-end;`: Mengatur fleks item ditempatkan di bagian akhir (akhir) dari sumbu utama flex container.
- `justify-content: center;`: Mengatur fleks item ditempatkan di tengah-tengah sumbu utama flex container.
- `justify-content: space-around;`: Mengatur fleks item didistribusikan secara merata di sekitar sumbu utama flex container, dengan ruang yang sama di antara mereka.
- `justify-content: space-between;`: Mengatur fleks item didistribusikan secara merata di sepanjang sumbu utama flex container, dengan ruang yang sama di antara fleks item pertama dan terakhir, tetapi tidak ada ruang di antara fleks item yang berdekatan.
**Kode Program :**
```
.box-container{
  justify-content: center ;
}
```
##### Kesimpulan
Setiap properti justify-Content mengubah tampilan elemen dengan cara yang berbeda-beda sesuai dengan property. 
Contoh`flex-start` untuk menempatkan flex items di awal (mulai) sumbu utama.`flex-end` untuk menempatkan flex items di akhir (akhir) sumbu utama.`center` untuk menempatkan flex items di tengah-tengah sumbu utama.`space-around` untuk mendistribusikan flex items secara merata di sekitar sumbu utama dengan ruang yang sama di antara mereka.`space-between` untuk mendistribusikan flex items secara merata di sepanjang sumbu utama dengan ruang yang sama di antara flex items pertama dan terakhir, tetapi tidak ada ruang di antara flex items yang berdekatan.


## Tantangan IV
### Penjelasan HTML
- Tag `<DOCTYPE html>` memberitahu web bahwa dokumen HTML adalah versi 5
- Tag pembuka `<html>` menandai awal sebuah dokumen HTML sampai dengan tag penutup `</html>`
- Tag pembuka `<head>` berisi informasi tentang halaman HTML sampai dengan tag penutup `</head>` ,biasanya dalam tag head terdapat tag `<title>` untuk memberikan informasi judul halaman HTML
- Apapun tag yang berada di antara tag pembuka `<body>` sampai dengan tag penutup `</body>` akan tampil di web browser.
- `<title>`: Menentukan judul halaman.
- `<link rel="stylesheet" href="Tugassbox.css">`: Menghubungkan dokumen dengan stylesheet eksternal.
- `<body class="main-container">`: Memulai konten utama halaman dengan kelas "main-container".
- `<div class="hero-container">`: Kontainer utama untuk semua konten.
- `<div class="box-container">`: Kontainer untuk setiap kotak konten.
- `<h1 class="item box-item-1">Selamat Datang</h1>`: Teks "Selamat Datang" dengan kelas "item" dan "box-item-1".
- `<h1 class="item box-item-2">di <b>Web Nero</b></h1>`: Teks "di Web Nero" dengan kelas "item" dan "box-item-2", kata "Web Nero" ditebalkan.
- `<div class="item box-item-3">`: Kontainer untuk tombol "Klik disini" dengan kelas "item" dan "box-item-3".
- `<button class="button">Klik disini</button>`: Tombol dengan teks "Klik disini" dan kelas "button".
- `<div class="item-box">`: Kontainer untuk gambar.
- `<img src="aset/nero.jpg">`: Gambar "nero.jpg" dari direktori "aset".
## Penjelasan CSS
- `body`: Mengatur latar belakang seluruh halaman menjadi warna ungu (purple).
- `.main-container`: Memberikan latar belakang warna ungu (purple) pada elemen dengan kelas "main-container". Ini mungkin digunakan sebagai wadah utama untuk konten.
- `.box-item-1 dan .box-item-2`: Mengatur tampilan teks pada elemen-elemen dengan kelas "box-item-1" dan "box-item-2". Ini termasuk mengatur ukuran font menjadi 50px, warna putih, dan memberikan jarak atas sejauh 10px.
- `img`: Mengatur tampilan gambar dengan lebar dan tinggi masing-masing 250px, dengan sudut melingkar sebesar 200px, serta menetapkan margin kiri sejauh 400px dan margin atas sejauh -400px. Hal ini dapat mempengaruhi posisi dan tata letak gambar dalam halaman.

**Kode Program Html:**
```HTML
<!DOCTYPE html>
<html>
<head>
    <title>Belajar CSS3</title>
    </head>
<body class="main-container">
    <div class="hero-container">
    <div class="box-container">

    <h1 class="item box-item-1">Selamat Datang</h1>
    <h1 class="item box-item-2">di <b>Web Nero</b></h1>
    <div class="item box-item-3">
    <button class="button">Klik disini</button>
    </div>

    </div>
    
    <div class="box-container">
    <div class="item-box">
    <img src="aset/nero.jpg">
    </div>
    </div>

    </div>
</body>
</html>

```
**Kode Program CSS :**
```CSS
	body{
        background-color:purple;
      }
      .main-container {
        margin-top: 90px;
        margin-left:90px ;
          background-color: purple;
      }
      .box-item-1{
          font-size: 50px;
          color: white;
          margin-top:10px;
          }
      .box-item-2{
         font-size: 50px;
          color: white;
          margin-top:10px;
      }
      img{
          width: 250px;
          height: 250px;
          border-radius: 200px;
          border-color: white;
          border-style: solid;
          margin-left: 400px;
          margin-top: -400px;
      }
```
**Hasil :**
![Gambar](Aset/IMG10/IMG10_4.png)

# Position
## Position Relative
### Penjelasan
- `background-color: aqua;`: Memberikan warna latar belakang elemen menjadi aqua. 
- `position: relative;`: Menetapkan posisi elemen relatif terhadap posisi defaultnya. 
- `top: 20px;`: Menggeser elemen 20 piksel ke bawah dari posisi defaultnya.
- `left: 30px;`: Menggeser elemen 30 piksel ke kanan dari posisi defaultnya. 
### Kode Program
```
box-1{
  background-color:aqua;
  position:relative;
  top:20px;
  left:30px; 
}
```
### Hasil 
**Before :**
![Gambar](Aset/IMG11/IMG11_1.png)
**After :**
![Gambar](Aset/IMG11/IMG11_2.png)
#### Kesimpulan
elemen dengan kelas "box-1" mengatur latar belakang menjadi warna aqua dan menggeser elemen 20 piksel ke bawah dan 30 piksel ke kanan dari posisi defaultnya.
## Position Absolute
### Penjelasan

- `background-color: purple;`: Mengatur latar belakang elemen menjadi warna ungu (purple).
- `position: absolute;`: Menetapkan elemen ke dalam konteks posisi yang dihitung relatif terhadap elemen induk yang memiliki posisi non-static. 
- `top: 15px;`: . elemen 15 piksel dari atas relatif terhadap posisi elemen induk yang ditetapkan dalam konteks posisi absolut.
- `left: 10px;`: Menggeser elemen 10 piksel dari kiri relatif terhadap posisi elemen induk yang ditetapkan dalam konteks posisi absolut.
### Kode Program
```
.box-2{
  background-color:purple;
  position:absolute;
  top:15px;
  left:10px; 
}
```
### Hasil 
**Before :**
![Gambar](Aset/IMG11/IMG11_1.png)
**After :**
![Gambar](Aset/IMG11/IMG11_3.png)
### Kesimpulan
kelas "box-2" menetapkan latar belakangnya menjadi warna ungu (purple) dan mengatur posisinya secara absolut,dimana elemen digeser 15 piksel dari atas dan 10 piksel dari kiri.

## Position Fixed
### Penjelasan
- `top: 50px;`: Menggeser elemen 50 piksel ke bawah dari posisi defaultnya.
- `left: 30px;`: Menggeser elemen 55 piksel ke kanan dari posisi defaultnya. 
- `background-color: aqua;`: Mengatur latar belakang elemen menjadi warna aqua.
- `position: fixed;`: Mengatur elemen dalam posisi tetap, yang berarti elemen akan tetap berada pada lokasi yang sama saat kita scroll. 
### Kode Program
```
box-1{
  background-color:aqua;
  position:Fixed;
  top:50px;
  left:55px; 
}
```
### Hasil 
**Before :**
![Gambar](Aset/IMG11/IMG11_1.png)
**After :**
![Gambar](Aset/IMG11/IMG11_4.png)
### Kesimpulan
position: fixed, elemen akan tetap berada pada posisinya yang ditentukan jika discrool.properti top dan left digunakan untuk menentukan jarak elemen dari tepi atas dan kiri. 

## Position Sticky
### Penjelasan
- `background-color: aqua;`: Mengatur latar belakang elemen menjadi warna aqua.
- `Position: sticky;`: Mengatur elemen dalam posisi "sticky", yang berarti elemen akan berperilaku seperti posisi relatif sampai mencapai posisi tertentu saat discrool kemudian akan tetap berada di tempat.elemen akan "melekat" pada posisi yang telah ditentukan saat jarak scroll mencapai nilai tertentu.
 - `top: 50px;`: Menggeser elemen sejauh 50 piksel dari atas elemen induk yang memiliki posisi tetap.
- `left: 55px;`: Menggeser elemen sejauh 55 piksel dari sisi kiri elemen induk yang memiliki posisi tetap.
### Kode Program
```
box-1{
  background-color:aqua;
  position:Sticky;
  top:50px;
  left:55px; 
}
```
### Hasil 
**Before :**
![Gambar](Aset/IMG11/IMG11_1.png)
**After :**
![Gambar](Aset/IMG11/IMG11_5.png)
### Kesimpulan
`position: sticky`, elemen akan seperti posisi relatif sampai jarak scroll mencapai nilai tertentu. elemen akan tetap berada pada posisi yang telah ditentukan saat jarak scroll mencapai nilai tertentu, sambil tetap mengikuti pergeseran scroll di bawahnya.

## Tantangan V
**Kode Program :**
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tantangan Position</title>
</head>
<body>
    <div class="container">
        <div class="item1">
            <img src="./naon.jpg" alt="" >
        </div>
        <div class="item2">
            <p class="text1">Thursday,July 16, 2015</p>
            <h4 class="text2">The standard chunk of Lorem Ipsum</h4>
            <p class="text3">Sed posuere consectectur est at lobortis.Anean eu leo quam.</p>
        </div>
        <div class="item3">
            <p class="text4">Read more</p>
            <img src="aset/arrow.jpeg" alt="">
        </div>
          <div class="like">
              <button>
              <img src="aset/like.jpeg" alt="">
            </button>
        </div>
    </div>
</body>
</html>
```
## Penjelasan HTML
- `<!DOCTYPE html>`: Mendefinisikan tipe dokumen HTML.
- `<html lang="en">`: Menandakan awal dari dokumen HTML dengan bahasa Inggris.
- `<head>`: Bagian kepala dokumen HTML yang berisi metadata dan referensi ke stylesheet.
- `<meta charset="UTF-8">`: Menentukan pengkodean karakter dokumen sebagai UTF-8.
- `<meta http-equiv="X-UA-Compatible" content="IE=edge">`: Menentukan versi IE yang kompatibel.
- `<meta name="viewport" content="width=device-width, initial-scale=1.0">`: Menyesuaikan tampilan halaman dengan lebar perangkat.
- `<title>Tantangan Position</title>`: Memberikan judul halaman.
- `<style>`: Mulai dari bagian CSS yang didefinisikan dalam dokumen HTML.
- `<body>`: Bagian utama dari dokumen HTML yang berisi konten yang akan ditampilkan di browser.
- `<div class="container">`: Sebuah div yang bertindak sebagai wadah untuk semua konten. Ini memiliki beberapa div anak yang akan di-styling.
- `<div class="item1">`, `<div class="item2">`, `<div class="item3">`: Div-div yang bertindak sebagai item atau bagian-bagian dari konten.
- `<img>`: Elemen gambar untuk menampilkan gambar.
- `<p>`, `<h4>`: Elemen paragraf dan heading untuk menampilkan teks.
- `<button>`: Tombol untuk berbagai fungsi, seperti menyukai konten.
- `<div class="like">`: Sebuah div yang berisi tombol "suka" atau "like".

```css
        body{
            background-color: aqua;
        }

        .container {
            display: flex;
            flex-direction: column;
            background-color: white;
            height: 458px;
            width: 300px;
            border-radius: 10px;
            margin-top: 150px;
            margin-left: 720px;
            position: relative;
        }

        .item1{
            background-color: red;
            height: 250px;
            width: 300px;
            border-radius: 10px 10px 0px 0px;
        }

        img {
            width:100%;
            height:100%;
            border-radius: 5px 5px 0px 0px;
        }

        .item2{
            background-color: whitesmoke;
            height: 175px;
            width: 300px;
            justify-content: center;
            align-items: center;
        }

        .text1 {
            font-size: small;
            font-family: Arial, Helvetica, sans-serif;
            margin-left: 20px;
        }

        .text2 {
            font-size: 20px;
            font-family: Arial, Helvetica, sans-serif;
            margin-left: 20px;
        }

        .text3 {
            margin-left: 20px;
            font-family: Arial, Helvetica, sans-serif;
            font-size: medium;
            margin-bottom: 30px;
        }  

        .item3 {
            display: flex;
            flex-direction: row;
            padding: 2px;
            background-color: gainsboro;
            border-radius: 0px 0px 5px 5px;
            width: 296px;
            justify-content: space-between;
            font-weight: bold;
        }

        .text4 {
            margin-left: 20px;
            font-family: Arial, Helvetica, sans-serif;
        }

        button {
            width: 62px;
            height: 55px;
            background-color: transparent;
            border: none;
            border-radius: 100px 100px 100px 100px;
            position: fixed;
            background-repeat: no-repeat;
            top: 350px;
            right: 520px;

        }

        .like img {
            border-radius: 100% ;
            margin-right: 110px;
            margin-left: 190px;
            position: absolute;
        }

        .item3 img {
            height: 30px;
            width: 30px;
            border-radius: 100% 100% ;
            align-items: center;
            justify-items: center;
            margin-right: 25px;
            margin-top: 10px;
        }
```
## Penjelasan CSS
- `body`: Memberi warna latar belakang aqua pada halaman.
- `.container`: Membuat tata letak kontainer menggunakan flexbox, memberi warna latar belakang putih, dan menentukan dimensi dan posisi.
- `.item1`, `.item2`, `.item3`: Masing-masing memberikan warna latar belakang dan menentukan dimensi dan posisi elemen.
- `img`: Mengatur dimensi gambar dan memberikan efek sudut melengkung pada beberapa gambar.
- `.text1`, `.text2`, `.text3`, `.text4`: Mengatur gaya teks untuk paragraf dan judul.
- `button`: Mengatur gaya untuk tombol, termasuk dimensi, warna latar belakang transparan, dan posisi.
- `.like img`: Mengatur gaya untuk gambar di dalam tombol "suka".
- `.item3 img`: Mengatur gaya untuk gambar di dalam item 3.
**Hasil :**
![Gambar](Aset/IMG11/IMG11_6.png)
## Kesimpulan
Program ini menggunakan HTML untuk membuat struktur konten dan CSS untuk merancang tampilannya. Elemen-elemen seperti gambar, teks, dan tombol diberikan gaya untuk menciptakan tampilan yang menarik dan responsif. Penggunaan posisi relatif, absolut, dan sticky memungkinkan penempatan yang tepat dari elemen-elemen tersebut di halaman.



# Pengenalan Responsive Web Design
Responsive web design atau desain web responsif adalah sebuah teknik atau metode bagi web designer untuk membuat suatu layout website yang dapat menyesuaikan diri sesuai dengan ukuran layar pengguna. Baik dari ukuran huruf, user interface, gambar dan tata letak akan menyesuaikan dengan lebar layar dan resolusi device yang digunakan. 
Selain dapat memengaruhi apa yang ditampilkan pada perangkat tertentu, ini juga untuk meningkatkan kenyamanan pengguna dalam mengunjungi suatu website.


# Mengapa perlu CSS Responsive?
Pernahkah Anda mengunjungi situs web di smartphone Anda dan halaman webnya berantakan atau teksnya terlalu kecil untuk dibaca? Ini artinya situs web tersebut belum responsif. Dengan memakai css responsif maka web kita memungkinkan tampil optimal di berbagai perangkat, mulai dari desktop, laptop, tablet, hingga smartphone. Berikut alasan beberapa alasan mengapa css responsif penting: 
- *Tampilan yang Bagus di Semua Perangkat*
	CSS responsif memungkinkan tampilan situs web beradaptasi dengan baik terhadap berbagai perangkat dan ukuran layar, sehingga pengguna akan memiliki pengalaman yang konsisten dan optimal, baik mereka mengakses situs melalui desktop, tablet, atau ponsel.
- *Mudah Diakses*
	Situs yang responsif bisa diakses dengan mudah oleh lebih banyak orang, termasuk yang menggunakan ponsel untuk browsing.
- *Interaksi yang Lebih Baik*
	Situs yang responsif cenderung membuat orang merasa lebih nyaman dan lebih mudah berinteraksi. Ini bisa meningkatkan kemungkinan orang melakukan hal-hal seperti membeli produk atau menghubungi Anda.
# Teknik Dasar CSS Responsif
## Konsep Dasar
- *Grid System*: Menggunakan grid system dalam CSS untuk mempermudah penataan elemen pada halaman web.
- *Flexbox*: Memahami penggunaan flexbox untuk menata elemen secara responsif.
## Media Query
Media query adalah fitur CSS yang memungkinkan Anda menargetkan perangkat dan ukuran layar yang berbeda dengan aturan CSS yang spesifik. Hal ini sangat penting untuk membuat website yang responsif, yaitu website yang dapat menyesuaikan tata letak dan desainnya secara otomatis agar terlihat optimal di semua perangkat, mulai dari desktop, laptop, tablet, hingga smartphone.
### Cara Kerja Media Query
Media query menggunakan aturan @media untuk menargetkan perangkat dan ukuran layar yang berbeda. Aturan ini terdiri dari dua bagian:
- *Media type:* Menentukan jenis perangkat yang ingin Anda targetkan, seperti screen (untuk desktop, laptop, tablet, dan smartphone) atau print (untuk printer).
- *Media feature:* Menentukan karakteristik perangkat yang ingin Anda targetkan, seperti max-width (lebar layar maksimum), min-width (lebar layar minimum), device-width (lebar perangkat), dan orientation (orientasi perangkat).
### Breakpoints
Breakpoints adalah titik-titik di mana tata letak halaman web akan berubah. Breakpoints biasanya ditentukan berdasarkan lebar layar perangkat.

- *320px:* Lebar minimum untuk smartphone.
- *768px:* Lebar minimum untuk tablet.
- *1024px:* Lebar minimum untuk laptop.
- *1200px:* Lebar minimum untuk desktop.

```css
@media screen and (max-width: 768px) {
  /* Aturan CSS untuk perangkat mobile */
  body {
    font-size: 16px;
  }
  .container {
    width: 100%;
  }
}
```

## Unit Relatif
Unit relatif adalah unit yang digunakan dalam CSS untuk menentukan ukuran elemen secara proporsional. Berbeda dengan unit absolut seperti piksel dan sentimeter, unit relatif tidak memiliki nilai tetap dan dapat berubah tergantung pada konteksnya.
### Keuntungan
- *Fleksibilitas:* Unit relatif memungkinkan Anda membuat website yang responsif dan dapat menyesuaikan dengan berbagai ukuran layar dan perangkat.
- *Kemudahan Penggunaan:* Unit relatif lebih mudah digunakan untuk menentukan ukuran elemen yang proporsional dan konsisten di seluruh website.
- *Pemeliharaan:* Website yang menggunakan unit relatif lebih mudah dipelihara dan diubah karena ukuran elemen akan menyesuaikan secara otomatis.
### Jenis-jenis Unit Relatif:
- *em:* Ukuran font elemen induk
- *rem:* Ukuran font elemen root (biasanya elemen `<html>`)
- *vw:* Lebar viewport (layar perangkat pengguna)
- *vh:* Tinggi viewport (layar perangkat pengguna)
- *vmin:* Nilai terkecil antara vw dan vh
- *vmax:* Nilai terbesar antara vw dan vh
## Viewport Meta Tag
Viewport meta tag adalah sebuah elemen HTML yang memberitahu browser web bagaimana cara menampilkan website Anda pada perangkat pengguna. Tag ini sangat penting untuk website responsif, yaitu website yang dapat menyesuaikan tata letak dan desainnya secara otomatis agar terlihat optimal di semua perangkat, mulai dari desktop, laptop, tablet, hingga smartphone.


```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```


- *width=device-width:* Menentukan lebar awal website agar sama dengan lebar perangkat pengguna.
- *initial-scale=1.0:* Mengatur skala awal website menjadi 100%.
# Best Practices
## Gunakan Mobile-First
Saat mendesain website, mulailah dengan mempertimbangkan tampilan website pada perangkat mobile. Hal ini akan membantu Anda membuat website yang lebih ringkas dan mudah digunakan di semua perangkat.

# Implementasi CSS Responsif
**Sebelum Responsif :**
![Gambar](Aset/IMG12/IMG_1.png)
**Sesudah Responsif :**
![Gambar](Aset/IMG12/IMG_2.png)
## Kode
### HTML
```html
<!DOCTYPE html>
<html>
  <head>
    <link rel="stylesheet" href="style.css" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>CSS Responsif</title>
  </head>
  <body>
    <header></header>
    <section class="container">
      <div class="list">
        <div class="item"></div>
        <div class="item"></div>
        <div class="item"></div>
        <div class="item"></div>
      </div>
      <aside></aside>
    </section>
    <footer></footer>
  </body>
</html>
```

### CSS
```css
body {
  background-color: #222831;
  color: white;
}

header {
  width: 100%;
  height: 77px;
  background-color: #EEEEEE;
}

.container {
  display: flex;
  justify-content: space-between;
}
.item {
  width: 250px;
  height: 70px;
  background-color: teal;
  margin: 1em 0;
}

aside {
  width: 300px;
  height: 70vh;
  background-color: salmon;
}

footer {
  width: 100%;
  height: 100px;
  background-color: yellow;
}

@media screen and (max-width: 768px) {
  .container {
    padding: 1rem;
    flex-direction: column;
  }
  .item {
    width: 100%;
  }
  aside {
    width: 100%;
  }
}
```

### Penjelasan Singkat
```css
body {
  background-color: #222831;
  color: white;
}
```

- body: Ini adalah elemen HTML yang menandakan seluruh konten halaman web.
- background-color: #222831: Ini mengatur warna latar belakang dari elemen "body" menjadi warna gelap dengan kode warna #222831 (hampir hitam).
- color: white: Ini mengatur warna teks di dalam elemen "body" menjadi putih.

```css
header {
  width: 100%;
  height: 77px;
  background-color: #EEEEEE;
}
```

- header:  elemen HTML yang menandakan bagian atas halaman web.
- width: 100%: membuat lebar elemen "header" sejajar dengan lebar area yang mengandungnya, yang mungkin adalah lebar jendela browser atau lebar elemen induk lainnya. Dengan memberikan nilai 100%, elemen "header" akan merentang ke seluruh lebar area tersebut.
- height: 77px: menetapkan tinggi elemen "header" menjadi 77 piksel. Jadi, meskipun lebarnya mengikuti lebar area induknya (100%), tingginya tetap diberikan secara spesifik dengan 77 piksel. Ini bertujuan untuk memastikan bahwa tinggi header tetap konsisten meskipun konten di dalamnya berubah.
- background-color: #EEEEEE : Ini mengatur warna latar belakang dari elemen "header" menjadi abu-abu muda dengan kode warna # EEEEEE.

``` css
.container {
  display: flex;
  justify-content: space-between;
}
```

- .container: Ini adalah kelas CSS yang digunakan untuk menargetkan elemen HTML dengan kelas "container".
- display: flex: membuat elemen dengan kelas "container" menggunakan model tata letak flexbox.
- justify-content: space-between: Ini mengatur jarak antara elemen-elemen di dalam flexbox container agar rata di sepanjang sumbu utama (biasanya sumbu horizontal), dengan menjaga jarak yang sama antara elemen-elemen dan meletakkan mereka pada posisi ujung container.

```css
.item {
  width: 250px;
  height: 70px;
  background-color: teal;
  margin: 1em 0;
}
```

- .item: Ini adalah sebuah selektor CSS yang memilih elemen dengan kelas "item".
- width: 250px: Ini mengatur lebar elemen menjadi 250 piksel.
- height: 70px;: Ini mengatur tinggi elemen menjadi 70 piksel.
- background-color: teal;: Ini mengatur warna latar belakang elemen menjadi warna teal.
- margin: 1em 0;: Ini mengatur jarak antara elemen dengan elemen lainnya, dengan 1 em (ukuran relatif terhadap font-size) pada bagian atas dan bawah, dan 0 pada bagian kanan dan kiri.

```css
aside {
  width: 300px;
  height: 70vh;
  background-color: salmon;
}
```

- aside: Ini adalah sebuah elemen HTML yang biasanya digunakan untuk menunjukkan konten tambahan di samping konten utama.
- width: 300px;: Ini mengatur lebar elemen "aside" menjadi 300 piksel.
- height: 70vh;: Ini mengatur tinggi elemen "aside" menjadi 70% dari tinggi viewport.
- background-color: salmon;: Ini mengatur warna latar belakang elemen "aside" menjadi warna salmon.

```css
footer {
  width: 100%;
  height: 100px;
  background-color: yellow;
}
```

- footer: Ini adalah sebuah elemen HTML yang biasanya digunakan untuk menampilkan informasi tambahan di bagian bawah halaman web.
- width: 100%;: Ini mengatur lebar elemen "footer" agar mengisi seluruh lebar dari parent element (biasanya body atau container lainnya).
- height: 100px;: Ini mengatur tinggi elemen "footer" menjadi 100 piksel.
- background-color: yellow;: Ini mengatur warna latar belakang elemen "footer" menjadi warna kuning.

```css
@media screen and (max-width: 768px) {
  .container {
    padding: 1rem;
    flex-direction: column;
  }
  .item {
    width: 100%;
  }
  aside {
    width: 100%;
  }
}
```

- @media screen and (max-width: 768px): Ini adalah aturan media query yang diterapkan ketika lebar layar kurang dari atau sama dengan 768 piksel.
- .container: Mengatur tampilan untuk elemen dengan kelas "container" ketika media query aktif.
    - padding: 1rem;: Memberikan padding sebesar 1 rem di sekitar elemen "container".
    - flex-direction: column;: Mengubah arah penataan elemen menjadi vertikal (kolom), sehingga elemen akan ditata dari atas ke bawah.
- .item: Mengatur tampilan untuk elemen dengan kelas "item" ketika media query aktif.
    - width: 100%;: Memberikan lebar sebesar 100% dari parent element, sehingga elemen akan mengisi lebar penuh.
- aside: Mengatur tampilan untuk elemen "aside" ketika media query aktif.
    - width: 100%;: Memberikan lebar sebesar 100% dari parent element, sehingga elemen "aside" akan mengisi lebar penuh.



# Pengenalan Bootstrap
## Apa Itu Bootstrap?
Bootstrap adalah salah satu dari banyak framework front-end yang ada di web development. Framework-front end menyediakan serangkaian alat dan gaya bawaan untuk mempercepat proses pengembangan web dengan menyediakan komponen-komponen UI siap pakai dan sistem grid yang responsif. Bootstrap khususnya, terkenal dengan kemampuannya dalam menciptakan tata letak yang responsif dan komponen-komponen UI yang seragam.
# Instalasi Bootstrap
## Cara instalasi Bootstrap secara online / CDN.
sekarang kita akan menjelaskan bagaimana cara menginstall bootstrap secara online. Berikut langkah-langkahnya:

1. Masuklah ke website resmi Bootstrap dengan mengunjungi situs web resmi di https://getbootstrap.com/.
2. Di laman utama web Bootstrap, cari dan klik menu "Introduction" yang terletak pada sisi sebelah kiri website.
3. Pada bagian "Starter Template" di halaman Introduction, kita akan melihat kode yang dapat kita gunakan untuk menghubungkan website kita yang mau diterapkan Bootstrap.
4. Klik tombol "Copy" untuk menyalin seluruh kode tersebut.
5. Buatlah file baru dengan nama index.html atau nama yang kita inginkan menggunakan teks editor atau editor HTML yang kita biasa pakai.
6. Tempelkan(paste) kode yang telah kita salin dari langkah sebelumnya ke dalam file html yang baru kita buat. dengan menempelkan kode tersebut maka bootstrap kita sudah terhubung namun harus secara online.
7. kita dapat mulai memberikan gaya pada tag-tag atau elemen dalam file HTML tersebut dengan menggunakan kelas-kelas Bootstrap. kita dapat melihatnya pada website resmi Bootstrap untuk mempelajari lebih lanjut tentang kelas-kelas yang tersedia dan cara penggunaannya.
8. Untuk melihat hasilnya, buka file html tadi menggunakan web browser kita.
9. Halaman web yang ditampilkan akan menggunakan Bootstrap untuk gaya dan fungsionalitasnya

## Mengunduh dan menginstal Bootstrap secara lokal.
Untuk menginstal Bootstrap secara offline, kita perlu mengunduh file Bootstrap dan menyimpannya di folder proyek kita. Berikut adalah langkah-langkah untuk menginstal Bootstrap secara offline:
1. **Unduh File Bootstrap:** Kunjungi situs web resmi Bootstrap di https://getbootstrap.com/ dan cari tautan unduhan untuk versi Bootstrap yang diinginkan. Klik atau ikuti instruksi untuk mengunduh file ZIP Bootstrap.
2. **Ekstrak File Bootstrap:** Setelah mengunduh file ZIP Bootstrap, temukan file tersebut di komputer kita dan ekstrak isi file ZIP ke folder proyek kita. kita dapat menggunakan aplikasi pengarsipan file atau ekstraksi bawaan (Archiver, 7zip, dll) pada sistem operasi kita untuk mengekstrak file ZIP . Setelah diekstrak, kita akan memiliki folder Bootstrap yang berisi berkas-berkas Bootstrap yang diperlukan.
3. **Hubungkan Berkas Bootstrap pada Halaman HTML:** Buka file HTML proyek kita menggunakan teks editor atau editor HTML yang biasa kita gunakan. Di dalam tag pada halaman HTML , tambahkan tautan ke berkas CSS Bootstrap dan skrip JavaScript Bootstrap. Gunakan tag link di dalam tag head untuk tautan CSS dan tag script di dalam tag body untuk javascript. Berikut contoh tautan yang umum di bootstrap:
```html
<link href="path/to/bootstrap.min.css" rel="stylesheet">
// tautan bootstrap CSS
<script src="path/to/bootstrap.bundle.min.js"></script>
// tautan bootstrap Javascript
```
dengan menuliskan script diatas, maka kita telah menghubungkan antara file html kita dengan bootstrap yang kita unduh tadi.
4. **Gunakan Kelas Bootstrap:** Setelah tautan Bootstrap ditambahkan, Kita dapat menggunakan kelas-kelas Bootstrap dalam elemen HTML proyek Kita untuk menerapkan gaya dan fungsionalitas yang disediakan oleh bootstrap kita. Kita dapat masuk ke web resmi Bootstrap untuk mempelajari lebih lanjut tentang kelaskelas yang tersedia dan cara penggunaannya.
5. **Jalankan File HTML:** Setelah Kita selesai menghbungkan tautan dan menggunakan kelas Bootstrap, Kita dapat menjalankan halaman HTML kita di web browser Kita untuk melihat hasilnya. Buka file HTML menggunakan web browser Kita dan lihat hasilnya
# Komponen-Komponen Bootstrap
Bootstrap menyediakan berbagai komponen yang siap pakai untuk membangun tampilan website yang responsif dan menarik. Berikut adalah beberapa komponen utama yang disediakan oleh Bootstrap:
## Grid System
Grid system Bootstrap adalah sistem layout yang responsif dan fleksibel. kita dapat membagi halaman menjadi baris(rows) dan kolom(columns) yang membentuk grid. Grid terdiri dari 12 kolom, yang dapat kita susun sesuai kebutuhan. Dengan menggunakan kelas CSS yang disediakan oleh Bootstrap, kita dapat dengan mudah menentukan berapa banyak kolom yang akan digunakan oleh setiap elemen di halaman web kita. Grid system ini sangat berguna dalam menciptakan tata letak yang responsif dan dapat menyesuaikan diri dengan berbagai ukuran layar
## Typography
Komponen typography Bootstrap menyediakan gaya dan kelas CSS yang konsisten untuk tipografi di halaman web kita. kita dapat dengan mudah mengatur ukuran teks, gaya huruf, dan pengaturan lainnya menggunakan kelas-kelas yang telah ditentukan. Ini memastikan bahwa teks di halaman web kita memiliki tampilan yang konsisten dan mudah dibaca di berbagai perangkat.
## Button
Komponen tombol Bootstrap memungkinkan kita dengan mudah membuat tombol dengan tampilan yang menarik dan responsif. kita dapat menggunakan kelas-kelas Bootstrap untuk mengatur berbagai gaya tombol, termasuk ukuran (large, small), warna (default, primary, secondary, dll.), dan variasi lainnya. Tombol-tombol ini dapat digunakan untuk tindakan seperti mengirim formulir, memuat ulang halaman, atau memicu tindakan lainnya di aplikasi web kita.
## Forms
Bootstrap menyediakan komponen form yang mudah digunakan untuk membuat form input. Ini termasuk input teks, area teks, kotak centang (checkbox), tombol radio, dropdown, dan lain-lain. Komponen form Bootstrap telah dirancang dengan tampilan yang responsif dan mudah dikustomisasi. kita dapat dengan mudah menambahkan validasi form dan mengatur tampilan form kita dengan menggunakan kelas-kelas Bootstrap yang telah ditentukan.
## Navbar
Komponen navbar Bootstrap memungkinkan kita membuat navigasi yang responsif dan mudah dikustomisasi di halaman web. kita dapat menambahkan logo, menu, tombol, dan komponen lainnya ke navbar dengan mudah. Navbar Bootstrap juga menyediakan fitur seperti menu dropdown, navigasi yang terlipat untuk perangkat mobile, dan tata letak yang fleksibel.
## Cards
Cards adalah komponen yang digunakan untuk menampilkan informasi dalam format yang terstruktur. Komponen kartu Bootstrap memungkinkan kita untuk membuat kolom dengan gambar, teks, tombol, dan komponen lainnya. cards ini dapat digunakan untuk menampilkan artikel, produk, profil pengguna, atau konten lainnya dengan tampilan yang menarik.
## Modal
Komponen modal Bootstrap digunakan untuk menampilkan jendela pop-up yang tumpang tindih dengan konten utama halaman. Modal ini berfungsi untuk menyoroti konten tambahan, pesan, atau form yang membutuhkan fokus pengguna. kita dapat menyesuaikan tampilan modal, mengatur ukuran, menambahkan judul, dan mengatur perilaku saat modal ditampilkan atau ditutup.
## Carousel
Carousel adalah komponen Bootstrap yang digunakan untuk membuat tampilan slide gambar atau konten lainnya. kita dapat menambahkan gambar, teks, tombol navigasi, dan indikator slide untuk membuat tampilan yang menarik dan interaktif. Carousel Bootstrap mendukung navigasi otomatis, kontrol manual, dan animasi transisi yang halus.
## Icons
Bootstrap sendiri menggunakan ikon dari Font Awesome, yang merupakan kumpulan ikon vektor yang sangat populer dan kaya akan fitur. kita dapat dengan mudah menambahkan ikon ke elemen seperti tombol, tautan, dan elemen lainnya menggunakan class-class ikon Bootstrap. Ini berfungsi untuk memperindah halaman web kita.
## Jumbotron
Jumbotron adalah komponen Bootstrap yang digunakan untuk menyoroti konten utama di halaman web. Biasanya ditempatkan di bagian atas halaman dengan judul besar danTerima kasih atas klarifikasinya.Komponen carousel Bootstrap digunakan untuk membuat tampilan slide yang interaktif. kita dapat menambahkan gambar, teks, dan tombol navigasi ke dalam carousel. Carousel Bootstrap mendukung navigasi otomatis, kontrol manual, dan animasi transisi. 

kita dapat menemukan daftar komponen lengkap dan dokumentasi resmi di situs web Bootstrap (https://getbootstrap.com/docs/).
# Contoh Penerapan Komponen Bootstrap
## Typography
1. Buka situs resmi Bootstrap di [getboostrap.com](getbootstrap.com)
	![[btc-1.png]]
2. Klik "Read the docs". Maka kita akan diarahkan pada halaman web yang berisi berbagai macam Typografi (class Bootstrap).
	![[btc-2.png]]
3. Misalnya kita akan membuat sebuah teks quotes seperti di bawah ini:
	![[btc-3.png]]
4. Ketikan "Typography" di kolom search lalu enter. Maka kita akan masuk ke halaman berikut:
	![[btc-4.png]]
5. Carilah Subbab "Alignment":
	![[btc-5.png]]
6. Salinlah kode yang tertera, lalu tempelkan di tag body pada halaman html yang telah kita hubungkan dengan Bootstrap kita
```html
<figure class="text-center">
<blockquote class="blockquote">
<p>A well-known quote, contained in a blockquote element.</p>
</blockquote>
<figcaption class="blockquote-footer">
Someone famous in 
<cite title="Source Title">Source Title </cite>
</figcaption>
</figure>
```
![btc-6.png](btc-6.png)
7. Hasilnya akan terlihat seperti berikut:
	![[btc-7.png]]
8. Kita bisa mengganti kata kata nya dengan cara mengganti teks yang ada di dalam tag p dan untuk teks kecil bagian bawah kita ganti pada bagian dalam tag figcaption
```html
<figure class="text-center">
  <blockquote class="blockquote">
    <p>Sebenarnya otak kita sama aja, yang <br>
    membedakan hanya siapa yang <br>
    mulai belajar duluan dan siapa yang <br>
    belajar terus menerus </p>
  </blockquote>
  <figcaption class="blockquote-footer">
    Dea Afrizal Doroboka<cite title="Source Title">Doroboka</cite>
  </figcaption>
</figure>
```
Hasilnya adalah sebagai berikut:
![[btc-8.png]]
*Keterangan :*
1. ==`text-center`== pada ==`<figure>`==: Kelas ini diterapkan pada elemen ==`<figure>`== , yang mengakibatkan kontennya, termasuk elemen ==`<blockquote>`== dan ==`<figcaption>`== , akan diatur menjadi ketengah halaman maupun kontainer.
2. blockquote pada ==`<blockquote>`== : Kelas ini memberikan gaya khusus pada elemen ==`<blockquote>`== . Elemen ini digunakan untuk merinci sebuah kutipan atau teks yang dianggap signifikan. Penggunaan kelas ini dari Bootstrap mungkin memberikan tampilan tertentu, seperti memodifikasi gaya margin atau padding, untuk memberikan estetika yang lebih baik.
3. blockquote-footer pada ==`<figcaption>`== : Kelas ini memberikan gaya khusus pada elemen ==`<figcaption>`== yang berada di dalam ==`<figure>`== . Elemen ini kemungkinan berisi informasi tambahan atau keterangan terkait elemen-elemen lain dalam ==`<figure>`==.
	- **`Dea Afrizal Doroboka`**: Ini adalah teks yang berada di dalam elemen ==`<figcaption>`==, memberikan informasi tambahan atau keterangan terkait dengan kutipan atau elemen-elemen lain dalam ==`<figure>`==.
	-  **`<cite title="Source Title">Doroboka / cite>`**: Ini adalah elemen ==`<cite>`== yang memberikan judul sumber ("Source Title"). Penggunaan kelas `blockquote-footer` dari Bootstrap mungkin menyusun elemen ini dengan tata letak dan gaya tertentu, seperti menetapkannya sebagai teks kaki atau memberikan gaya yang konsisten dengan elemen lain dalam kelompok ==`<figure>`==.
*Keterangan*: 
Untuk bagian "Dea Afrizal" adalah nama seseorang yang mengatakan quotes tersebut dan "Doroboka" adalah sumber dimana orang tersebut mengatakn kata-kata itu. Kata- kata yang dituliskan yaitu berada dalam tag ==`p`== .
## Navbar
1. Bukalah Kembali [getbootstrap.com](getbootstrap.com) lalu ketik "navbar" dikolom "search" dan klik enter
	![[btc-15.png]]
2. Carilah jenis navbar yang diinginkan.
	![[btc-16.png]]
3. Jika misalnya kita telah menemukan jenis navbar yang kita inginkan, maka, salinlah kode program yang ada dibawah gambar contoh navbar tersebut
	![[btc-17.png]]
```html
<nav class="navbar navbar-expand-lg bg-body-tertiary">
    <div class="container-fluid">
        <a class="navbar-brand" href="#">Navbar</a>
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNavDropdown" aria-controls="navbarNavDropdown" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarNavDropdown">
            <ul class="navbar-nav">
                <li class="nav-item">
                    <a class="nav-link active" aria-current="page" href="#">Home</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#">Features</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#">Pricing</a>
                </li>
                <li class="nav-item dropdown">
                    <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                        Dropdown link
                    </a>
                    <ul class="dropdown-menu">
                        <li><a class="dropdown-item" href="#">Action</a></li>
                        <li><a class="dropdown-item" href="#">Another action</a></li>
                        <li><a class="dropdown-item" href="#">Something else here</a></li>
                    </ul>
                </li>
            </ul>
        </div>
    </div>
</nav>

```
4. Tempelkanlah kode program yang terlah kita salin ke dalam tag body di file html kita. Jangan lupa untuk menautkan file html kita dengan bootstrap seperti pada langkah-langkah sebelumnya
	![[btc-18.png]]
5. Jalankanlah file html yang sudah ditempeli kode program bootstrap tadi melalui web browser. Maka lihatlah hasilnya
	![[btc-19.png]]
6. Misalnya kita ingin memberikan warna hijau pada background navbar kita. Pertama ketiklah "background" di kolom search
	![[btc-20.png]]
7. Carilah Warna yang kita inginkan. Misalnya dalam praktek ini adalah warna hijau
	![[btc-21.png]]
	![[btc-22.png]]
	Terdapat banyak jenis warna dalam bootstrap.
8. Karena kita ingin mengkostumisasi warna background kita menjadi hijau maka kita akan memakai bg-succes . ketikkan bg-succes pada class tag pembuka seperti di bawah ini
	![[btc-23.png]]
	*Keterangan*:
	Karena kita akan memberikan warna background pada navbar maka untuk menerapkannya, langsung terapkan class tag yang membungkus semua eleme-elemen yang ada pada tag tersebut.
9. Jika sudah maka hasilnya akan seperti ini:
	![[btc-24.png]]
10. Sekarang kita akan mengubah warna font yang ada pada navbar. Langkah pertama klik "Colors" pada bagian Utilities
	![[btc-25.png]]
11. Maka kita akan diarahkan pada halaman yang memuat berbagai macam warna font
	![[btc-26.png]]
12. Carilah warna font yang kita inginkan. Misalnya pada kostumisasi navbar ini. Kita akan menggunakan warna font putih
	![[btc-27.png]]
13. Karena kita ingin menggunakan warna font putih maka perintah yang digunakan adalah "text-white"
14. Masuklah kembali ke dalam file html kita
15. pada bagian class sebuah tag yang membungkus text yang akan kita ganti warna, ketiklah text-white . Contohny ada pada gambar berikut:
	![[btc-28.png]]
16. Hasilnya akan terlihat seperti di gambar ini:
	![[btc-29.png]]
17. Terapkanlah Text-White diseluruh class pada tag yang membungkus text-text itu seperti halnya pada text navbar tadi
	![[btc-30.png]]
18. Jika file html dijalankan, hasilnya adalah sebagai berikut
	![[btc-31.png]]
19. Sekarang kita akan mengganti text yang ada di navbar tersebut. Caranya sangat mudah, yaitu cukup kita ganti text-text tadi dengan kata kata yang kita inginkan. Misalnya adalah sebagai berikut:
	![[btc-32.png]]
20. Maka hasilnya adalah sebagai berikut:
	![[btc-33.png]]
21. Sekarang kita akan menambahkan kolom search pada navbar kita. pada bagian navbar di [getbootstrap.com](getbootstrap.com) Scroll ke bawah hingga menemukan seperti pada gambar
	![[btc-34.png]]
22. Salin kodenya lalu tempelkan di bagian bawah kode navbar kita tadi. Jadi jangan disatukan ke dalam kode navbar tadi.
```html
<nav class="navbar bg-body-tertiary">
    <div class="container-fluid">
        <form class="d-flex" role="search">
            <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search">
            <button class="btn btn-outline-success" type="submit">Search</button>
        </form>
    </div>
</nav>
```
![[btc-35.png]]

*Keterangan*:
1. ==`navbar`== : Kelas ini menunjukkan bahwa elemen ==`<nav>`== adalah bagian dari komponen navbar. Navbar adalah bagian dari Bootstrap yang menyediakan navigasi di bagian atas halaman web. Dengan memberikan kelas navbar , kita memberitahu Bootstrap untuk menerapkan gaya dan tata letak khusus yang terkait dengan navigasi.
2. ==`bg-body-tertiary`== : Kelas ini memberikan warna latar belakang pada navbar. Dalam hal ini, warna latar belakangnya diberi warna sesuai dengan warna "hijau" Warna latar belakang ini dapat disesuaikan sesuai kebutuhan desain.
3. ==`container-fluid`== : Kelas ini diterapkan pada elemen ==`<div>`== yang membungkus elemen-elemen dalam navbar. Kelas ini memberikan padding yang sesuai dan membuat elemen-elemen di dalamnya menjaga lebar penuh dari layar (menggunakan grid system Bootstrap). Dengan kata lain, kontennya akan merespons secara baik pada berbagai lebar perangkat.
4. ==`d-flex`== : Kelas ini mengubah elemen ==`<form>`== menjadi kontainer flex. Flexbox adalah teknik tata letak yang kuat di CSS yang memudahkan pengaturan dan penataan elemen dalam satu atau dua dimensi. Dengan memberikan kelas d-flex , elemen form dan anak-anaknya dapat disusun secara fleksibel.
5. ==`form-control`== : Kelas ini diterapkan pada elemen ==`<input>`== untuk memberikan gaya yang konsisten pada elemen formulir. Di sini, elemen input diberi gaya Bootstrap standar untuk mengubahnya menjadi kontrol formulir yang responsif dan berada dalam baris yang sesuai.
6. ==`me-2`== : Ini adalah kelas Bootstrap yang memberikan margin kanan sebesar 2 pada elemen yang memilikinya. Dalam codingan ini, kelas ini diterapkan pada elemen input untuk memberikan jarak margin kanan.
7. ==`btn`== dan ==`btn-outline-success`== : Kelas ini memberikan gaya pada elemen ==`<button>`== . Kelas btn mengindikasikan bahwa ini adalah elemen tombol Bootstrap, sedangkan btn-outline-success memberikan gaya tombol dengan warna tepi hijau ("success" dalam Bootstrap).
8. ==`type="submit"`== pada tombol: Ini menentukan bahwa tombol tersebut bertindak sebagai tombol submit dalam formulir. Ketika ditekan, formulir akan dikirim.
9. Maka hasilnya adalah seperti berikut:
	![[btc-36.png]]
10. Untuk membuat agar navbar tersebut terlihat menyatu, berikan background-color yang sama pada navbar diatasnya, yaitu menggunakan kode bg-succes . Letakkan di class tag yang membungkus seluruh elemen search tadi.
	![[btc-37.png]]
11. Maka hasil yang muncul akan seperti ini
	![[btc-38.png]]
## Buttons
Pada praktek sebelumnya kita sudah mengatur navbar dan juga menambahkan kolom search. Namun ada masalah dengan tombolnya. Karena tombolnya memiliki warna yang sama dengan warna background yang digunakan yaitu hijau, Maka tombol tersebut tidak terlihat akibat warnanya menyatu. Pada bagian kali kita akan membahas cara mengatur sebuah tombol di bootstrap. Berikut caranya:

1. Permasalahan tadi ialah background color tombolnya yang menyatu dengan warna backgriund navbarnya. Untuk mengatur warna tombol, pertama di situs getbootstrap.com, carilah bagian "buttons" di Components
	![[btc-39.png]]
2. Jika sudah menemukan klik bagian tersebut, maka kita akan diarahkan pada bagian buttons seperti pada gambar
	![[btc-40.png]]
3. Scroll lah ke bawah hingga menemukan bagian "Outlines Buttons"
	![[btc-41.png]]
4. Saat ini kita akan menggunakan jenis warna putih agar tidak lagi menyatu dengan warna background navabrnya. Pada outline buttons yang berwarna putih, tertulis "Light". Oleh karena itu salinlah kode program yang ada tulisan "Light".
```html
<button type="button" class="btn btn-outline-light">Light</button>
```
5. Blok lah terlebih dahulu kode program yang mengatur tombol pada bagian search tadi
	![[btc-42.png]]
6. Tempelkanlah kode program outline light, untuk menggantikan kode program button yang lama
	![[btc-43.png]]
7. Maka hasilnya akan bagus seperti pada gambar dibawah ini:
	![[btc-44.png]]
8. Ubahlah Text "Light" menjadi "Search"
	![[btc-45.png]]
9. Maka hasilnya akan seperti ini:
	![[btc-46.png]]
## Cards dan Form
Sekarang kita akan membuat sebuah form, dimana form tersebut kita asumsikan sebagai login page dari web kita tadi. Dalam pembuatan form login ini, kita akan menggunakan cards sebagai layout/tata letak yang akan mengatur form login tadi. Berikut langkah-langkahnya:

1. Yang pertama kita tentunya harus menentukan layout cards nya terlebih dahulu. Hal ini bertujuan agar jika tata letak card sudah ada, maka kita tinggal mengatur form nya di dalam card tadi. Masuk ke situs bootstrap tadi lalu pilih cards
	![[btc-47.png]]
2. Scrol ke bawah hingga menemukan layout yang kita inginkan, misalnya seperti pada gambar:
	![[btc-48.png]]
3. Pada bagian bawah contoh, terdapat kode program. Salinlah kode program tersebut
```html
<div class="card">
    <div class="card-header">
        Featured
    </div>
    <div class="card-body">
        <h5 class="card-title">Special title treatment</h5>
        <p class="card-text">With supporting text below as a natural lead-in to additional content.</p>
        <a href="#" class="btn btn-primary">Go somewhere</a>
    </div>
</div>
```
4. Tempelkanlah kode program itu pada halaman html terkait. Tentu saja dengan bootstrap yang sudah ditautkan, baik offline, maupun online.
5. Maka hasil awalnya adalah sebagai berikut:
	![[btc-49.png]]
6. karena jarak atas antara card dengan batas website terlalu dekat maka pada class card tambahkan mt-2 .
```html
<div class="card mt-2">
    <div class="card-header">
        Featured
    </div>
    <div class="card-body">
        <h5 class="card-title">Special title treatment</h5>
        <p class="card-text">With supporting text below as a natural lead-in to additional content.</p>
        <a href="#" class="btn btn-primary">Go somewhere</a>
    </div>
</div>
```
7. Maka hasilnya adalah seperti ini:
	![[btc-50.png]]
8. Sekarang kita ingin membuatnya terlihat ke tengah. Maka buatlah sebuah div dengan class yaitu "container", lalu salin masuklah kode program card tadi. Dengan kata lain, bungkuslah kode program card dengan sebuah div dengan class="container".
```html
<div class="container">
    <div class="card mt-2">
        <div class="card-header">
            Featured
        </div>
        <div class="card-body">
            <h5 class="card-title">Special title treatment</h5>
            <p class="card-text">With supporting text below as a natural lead-in to additional content.</p>
            <a href="#" class="btn btn-primary">Go somewhere</a>
        </div>
    </div>
</div>
```
9. Berikut hasil dari di bungkusnya cards tadi.
	![[btc-51.png]]
10. Sekarang kita akan membuat form nya. Pertama-tama, kita perlu membuat judul form. Caranya adalah ganti tulisan "Featured" di html kita dengan kata yang kita inginkan. misalnya pada program ini kita akan mengganti tulisan menjadi "Form Login".
	![[btc-10.png]]
```html
<div class="container">
    <div class="card mt-2">
        <div class="card-header">
            <h5>Form Login</h5>
        </div>
        <div class="card-body">
            <h5 class="card-title">Special title treatment</h5>
            <p class="card-text">With supporting text below as a natural lead-in to additional content.</p>
            <a href="#" class="btn btn-primary">Go somewhere</a>
        </div>
    </div>
</div>
```
*Keterangan*:
	1. ==`container`== pada ==`<div class="container">`== : Kelas ini memberikan tata letak yang terkandung pada lebar tertentu (dalam pixel) dan ditengahkan di tengah halaman atau elemen yang memuatnya. Ini membantu dalam mengatur konten agar sesuai dengan standar desain Bootstrap.
	2. ==`card`== pada ==`<div class="card mt-2">`== : Kelas ini memberikan gaya dan tata letak khusus untuk elemen ==`<div>`== yang merupakan kartu (card). Kartu adalah elemen Bootstrap yang sering digunakan untuk menampilkan konten atau informasi dalam satu unit terpisah dengan gaya yang konsisten.
		- `mt-2` : Kelas ini memberikan margin atas (margin-top) sebesar 2 unit. Ini membantu memberikan ruang di bagian atas kartu dan memisahkannya dari elemen-elemen sekitarnya.
	3. ==`card-header`== pada ==`<div class="card-header">`== : Kelas ini memberikan gaya khusus untuk elemen ==`<div>`== yang berfungsi sebagai header kartu. Header kartu biasanya berisi judul atau informasi lain yang menandai atau menjelaskan konten kartu.
		- ==`<h5>Form Login / h5>`== : Ini adalah elemen judul level 5 (h5) di dalam header kartu yang memberikan judul "Form Login" pada kartu.
	4. ==`card-body`== pada ==`<div class="card-body">`== : Kelas ini memberikan gaya khusus untuk elemen ==`<div>`== yang berisi tubuh atau konten utama kartu. Ini membantu memisahkan dan memvisualisasikan konten utama kartu.
		- ==`<h5 class="card-title">Special title treatment / h5>`== : Ini adalah elemen judul level 5 (h5) di dalam tubuh kartu yang memberikan judul khusus.
		- ==`<p class="card-text">With supporting text below as a natural lead-in to additional content. / p>`== : Ini adalah elemen paragraf di dalam tubuh kartu yang memberikan teks pendukung atau keterangan untuk konten utama kartu.
		- ==`<a href="#" class="btn btn-primary">Go somewhere / a>`== : Ini adalah elemen anchor (tautan) yang merupakan tombol dengan kelas Bootstrap "btn" dan "btn-primary", memberikan tampilan dan warna tertentu sesuai dengan desain Bootstrap.
	**Perbedaan Container dengan Container-fluid**: 
	**container**: 
	- ==`container`== memberikan tata letak yang terpusat dan memiliki lebar yang tetap (fixed-width).
	- Lebar ==`container`== diatur dalam satuan piksel dan tetap konstan terlepas dari ukuran layar pengguna.
	- Digunakan untuk membuat tata letak yang terkonsentrasi di tengah halaman dan memberikan batasan pada lebar kontennya.
	**container-fluid**:
		- ==`container-fluid`== memberikan tata letak yang penuh lebar, mengisi seluruh lebar layar.
		- Lebar ==`container-fluid`== disesuaikan dengan lebar layar pengguna, sehingga konten dapat memanfaatkan seluruh lebar tampilan tanpa batasan piksel tertentu.
		- Digunakan ketika Anda ingin membuat tata letak yang menyesuaikan diri dengan lebar layar dan memberikan tampilan responsif.
11. Hasilnya adalah sebagai berikut
	![[btc-9.png]]
12. Sekarang pada bagian dalam div card-body hapus semua elemen yang ada didalamnya kecuali button:
```html
<div class="container">
    <div class="card mt-2">
        <div class="card-header">
            <h5>Form Login</h5>
        </div>
        <div class="card-body">
            <a href="#" class="btn btn-primary">Go somewhere</a>
        </div>
    </div>
</div>
```
13. Hasilnya akan seperti ini
	![[btc-11.png]]
14. Langkah selanjutnya adalah menambahkan elemen-elemen form ke dalam card-body untuk membuat formulir login. Anda dapat menggunakan elemen-elemen HTML seperti form , input , dan button untuk ini. bukalah kembali getbootstrap.com dan pilihlah form yang kita inginkan:
	![[btc-12.png]]
15. Salinlah kode program dibawah contoh forms tadi:
```html
<form>
    <div class="mb-3">
        <label for="exampleInputEmail1" class="form-label">Email address</label>
        <input type="email" class="form-control" id="exampleInputEmail1" aria-describedby="emailHelp">
        <div id="emailHelp" class="form-text">We'll never share your email with anyone else.</div>
    </div>
    <div class="mb-3">
        <label for="exampleInputPassword1" class="form-label">Password</label>
        <input type="password" class="form-control" id="exampleInputPassword1">
    </div>
    <div class="mb-3 form-check">
        <input type="checkbox" class="form-check-input" id="exampleCheck1">
        <label class="form-check-label" for="exampleCheck1">Check me out</label>
    </div>
    <button type="submit" class="btn btn-primary">Submit</button>
</form>
```
16. Tempelkanlah didalam cards-body tadi
	![[btc-13.png]]
17. Maka hasilnya adalah sepert ini:
	![[btc-14.png]]
Dengan demikian kita sudah berhasil membuat layoutcards dimana form login sebagai kontennya
# Grid For Responsive Web/Layouting
Bootstrap memiliki sistem tata letak yang kuat yang bernama grid. Grid berguna untuk membuat tata letak yang responsif di halaman web kita. Sistem grid Bootstrap berdasarkan konsep kolom yang dapat diatur dalam baris. Berikut adalah beberapa hal penting yang perlu kita ketahui tentang grid dan layouting di Bootstrap:

1. **KONTAINER (Container)**
	Grid Bootstrap harus ditempatkan dalam elemen kontainer. Terdapat dua jenis kontainer yang tersedia, yaitu .container dan .container-fluid. .container memiliki lebar terbatas dan akan disesuaikan dengan lebar layar. .container ini digunakan ketika kita ingin membuat tata letak yang terpusat dan terbatas pada lebar tertentu. .container-fluid memiliki lebar penuh dan akan mengisi seluruh lebar layar. Kontainer ini digunakan ketika kita ingin membuat tata letak yang menyesuaikan dengan lebar layar penuh.
2. **BARIS (Row)**
	Baris digunakan untuk mengelompokkan kolom-kolom dalam tata letak. kita dapat menambahkan class .row pada elemen yang berfungsi sebagai wadah kolom. Baris ini akan memastikan bahwa kolom-kolom di dalamnya akan diatur secara horizontal.
3. **KOLOM (Column):**
	Kolom adalah bagian dasar dari sistem grid Bootstrap. Kolom- kolom ditempatkan di dalam baris dan digunakan untuk membagi horizontal ruang dalam grid. Setiap baris dipecah menjadi 12 kolom, yang dapat kita bagi sesuai kebutuhan.

	**Catatan**: kita dapat menggunakan kelas seperti .col- , .col-sm- , .col-md- , .col-lg- , atau .col-xl- untuk menentukan bagaimana kolom akan berperilaku di berbagai ukuran perangkat. Misalnya, .col-sm-6 akan membuat kolom tersebut memiliki lebar setengah dari baris pada ukuran layar kecil. kita dapat menggabungkan kelas kolom untuk ukuran layar yang berbeda untuk menciptakan tata letak yang responsif. Misalnya, .col-md-6 .col-lg-4 akan membuat kolom tersebut memiliki lebar setengah dari baris pada ukuran layar medium, dan memiliki lebar sepertiga dari baris pada ukuran layar besar.
4. **OFFSET**
	Kita dapat menggunakan kelas offset untuk memindahkan kolom ke samping. Misalnya, .offset-md-2 akan memindahkan kolom 2 satuan ke kanan pada layar dengan ukuran medium. Offset digunakan ketika Kita ingin membuat ruang kosong di antara kolom-kolom.
5. **Perilaku pada Ukuran Layar yang Berbeda**
	Kita dapat menggunakan kelas-kelas grid Bootstrap yang berbeda untuk mengontrol tampilan kolom pada ukuran layar yang berbeda. Misalnya, Kita dapat menggunakan .colsm- untuk ukuran layar kecil, .col-md- untuk ukuran layar medium, dan sebagainya. Dengan cara ini, Kita dapat membuat tata letak yang responsif untuk berbagai perangkat.
6. **NESTING**
	Nesting memungkinkan Kita menempatkan baris dan kolom di dalam kolom lainnya. Dengan cara ini, Kita dapat membuat tata letak yang lebih kompleks dengan komponen-komponen yang terkait. Misalnya, Kita dapat menempatkan sebuah baris di dalam kolom yang ada di dalam baris lainnya
7. **ORDER**
	Kita dapat menggunakan kelas .order- untuk mengubah urutan kolom pada ukuran layar tertentu. Misalnya, .order-first akan memindahkan kolom ke posisi pertama, dan .orderlast akan memindahkan kolom ke posisi terakhir. Dengan menggunakan kelas ini, Kita dapat mengatur ulang urutan kolom untuk mencapai tata letak yang diinginkan pada berbagai ukuran layar.

Itu adalah beberapa konsep penting dalam sistem grid Bootstrap. Dengan menggunakan sistem grid ini, kita dapat membuat tata letak yang responsif dan menyesuaikan tampilan elemen-elemen pada berbagai ukuran layar dengan mudah.
## Contoh Penggunaan dan Penjelasannya
Sekarang kita akan mencoba penggunaan grid yang dengan bantuan Bootstrap. Berikut langkah-langkahnya:

1. Masuklah kembali ke web getbootstrap.com.
	![[btc-52.png]]
2. carilah "Grid" di Kolom search lalu klik enter. Maka kita akan diarahkan pada halaman web yang berisi tentang grid.
	![[btc-53.png]]
3. Carilah layout atau tata letak grid yang kita inginkan. Misalnya pada praktek kali ini, kita akan menggunakan layout "Row columns".
	![[btc-54.png]]
4. Salinlah kode program yang terletak di kode bawah contohnya.
```html
<div class="container text-center">
    <div class="row row-cols-2">
        <div class="col">Column</div>
        <div class="col">Column</div>
        <div class="col">Column</div>
        <div class="col">Column</div>
    </div>
</div>
```
5. Tempelah pada file html yang tentunya telah dihubungkan dengan tautan bootstrap, baik secara offline maupun online.
	![[btc-55.png]]
6. Maka hasilnya akan seperti berikut:
	![[btc-56.png]]
	*Keterangan:*
	Jadi tulisan "Column" adalah isi konten yang sudah teratur dalam grid ini. kita bisa mengganti "konten" ini dengan konten yang kita inginkan
7. Untuk mengganti kontennya hapuslah tulisan "Column" lalu gantilah dengan kontent yang kita inginkan.
```html
<div class="container text-center">
    <div class="row row-cols-2">
        <div class="col">
            <div>
                <img width="50px" height="50px" src="img/HTML5_badge.png" alt="logo html" class="mt-5">
                <h3>HTML</h3>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. <br>Nobis totam assumenda unde quod et vitae minus beatae, <br> quibusdam impedit laboriosam earum, <br> possimus consequatur quisquam dolore ex ipsa eaque cupiditate neque.</p>
            </div>
        </div>
        <div class="col">
            <div>
                <img width="50px" height="60px" src="img/css-3-logo.png" alt="logo html" class="mt-4">
                <h3>CSS</h3>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. <br>Nobis totam assumenda unde quod et vitae minus beatae, <br> quibusdam impedit laboriosam earum, <br> possimus consequatur quisquam dolore ex ipsa eaque cupiditate neque.</p>
            </div>
        </div>
        <div class="col">
            <div>
                <img width="50px" height="50px" src="img/OIP.jpeg" alt="logo html" class="mt-2">
                <h3>JavaScript</h3>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. <br>Nobis totam assumenda unde quod et vitae minus beatae, <br> quibusdam impedit laboriosam earum, <br> possimus consequatur quisquam dolore ex ipsa eaque cupiditate neque.</p>
            </div>
        </div>
        <div class="col">
            <div>
                <img width="50px" height="50px" src="img/R.png" alt="logo html" class="mt-2">
                <h3>JQuery</h3>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. <br> Nobis totam assumenda unde quod et vitae minus beatae, <br> quibusdam impedit laboriosam earum, <br> possimus consequatur quisquam dolore ex ipsa eaque cupiditate neque.</p>
            </div>
        </div>
    </div>
</div>
```
8. Hasil nya akan menjadi seperti berikut:
	![[btc-57.png]]
	*Keterangan:*
	Jadi Grid tadi mengatur Row dan Column dimana terdapat 2 baris berisi 4 kolom sebagai kontennya. Kontennya tadi kita ganti dengan konten yang kita inginkan
9. Apabila layar yang kita kecilkan, maka grid akan menyesuaikan ukurannya seperti pada gambar ini
	![[btc-58.png]]
	*Keterangan:*
	Jadi grid ini sudah mengatur mengenai penyesuaian ukuran layar kita, sehingga, dapat menyesuaikan di segala ukuran monitor.
10. Apabila kita melihatnya di perangkat, maka akan terlihat seperti ini:
	![[btc-59.png]]
	*Keterangan:*
	Jadi karena grid yang disediakan oleh bootstrap telah mendukung fitur responsive, maka ketika user melihat tampilan web kita di ponsel, maka tata letak akan mengikutinya sesuai dengan ukuran ponsel, seperti yang terlihat pada gambar di atas
## Contoh Penggunaan `col-md`, `col-lg` dan `col-sm`
Kelas ==`col-md`== , ==`col-lg`== , dan ==`col-sm`== adalah kelas-kelas kolom dalam Bootstrap yang digunakan untuk meresponsifkan tata letak halaman web sesuai dengan ukuran layar perangkat. Bootstrap menggunakan sistem grid yang terdiri dari 12 kolom, dan kelas-kelas ini memungkinkan Anda mengontrol sejauh mana elemen-elemen tersebut harus meluas pada layar yang berbeda.

- ==`col-sm`== : Digunakan untuk layar kecil (small), seperti pada perangkat mobile atau tablet dalam orientasi potret. Kolom ini akan berlaku untuk layar dengan lebar 576px atau lebih.
- ==`col-md`== : Digunakan untuk layar sedang (medium), yang mencakup perangkat seperti tablet dalam orientasi landscape. Kolom ini akan berlaku untuk layar dengan lebar 768px atau lebih.
- ==`col-lg`== : Digunakan untuk layar besar (large), yang mencakup desktop. Kolom ini akan berlaku untuk layar dengan lebar 992px atau lebih.

**Contoh**:
Sekarang kita akan coba untuk membuat sebuah tampilan dengan menggunakan class diatas tadi. Berikut contohnya: 
1. Bukalah kembali web getbootsrap lalu di kolom pencarian carilah "grid".
	![[btc-60.png]]
2. Cari dan copylah kembali codingan grid yang kita gunakan pada praktek sebelumnya.
	![[btc-61.png]]
```html
<div class="container text-center">
    <div class="row row-cols-2">
        <div class="col">Column</div>
        <div class="col">Column</div>
        <div class="col">Column</div>
        <div class="col">Column</div>
    </div>
</div>
```
3. Tempelkanlah codingan tadi di visual studio kode pada file tempat kita mempraktekkan grid pada praktikum sebelumnya, agar kita bisa menggunakan satu file saja untuk praktek.
	![[btc-62.png]]
4. Maka akan terlihat seperti gambar di bawah ini:
	![[btc-63.png]]
	*Keterangan*:
	Perhatikanlah di bawah kolom JavaScript dan JQuery, terdapat tulisan column sebanyak 4 dan bersusun hal ini dikarenakan pada kodingan tadi, teks yang dipakai sebagai template di bootstrap adalah "Column", nanti pada tahap selanjutnya kita akan mengganti "Column" itu dengan text atau item yang kita inginkan.
5. Sekarang, pada codingan yang kita ambil dari web bootstrap tadi pada bagian ==`<div class="col">`== yang pertama, tambahkanlah -md sehingga menjadi ==`<div class="col-md>"`== . Kemudian pada ==`<div class="col">`== yang kedua, tambahkanlah - lg sehingga menjadi ==`<div class="col-lg">`== , dan terakhir pada ==`<div class="col">`== yang ketiga, tambahkanlah -sm sehingga menjadi ==`<div class="col-sm">`== , sementara pada ==`<div class="col">`== yang terakhir kita biarkan saja seperti bawaan.
```html
<div class="container text-center">
    <div class="row row-cols-2">
        <div class="col-md">Column</div>
        <div class="col-lg">Column</div>
        <div class="col-sm">Column</div>
        <div class="col">Column</div>
    </div>
</div>
```
![[btc-65.png]]
6. Maka hasilnya akan menjadi seperti ini:
	**Sebelum:**
	![[btc-66.png]]
	**Sesudah:**
	![[btc-67.png]]

*Keterangan:*
- ==`col-md`== :Dengan menambahkan -md pada codingan tadi akan membuat kolom tersebut mengambil sebagian besar lebar tersedia (12 kolom) pada layar dengan lebar medium (768px atau lebih).
- ==`col-lg`== : Sama seperti col-md , tetapi ditujukan untuk layar lebar (large, 992px atau lebih). col-sm : Sama seperti col-md , tetapi ditujukan untuk layar kecil (small, 576px atau lebih).
7. Tambahkanlah teks ataupun item dari yang kita inginkan dengan cara hapuslah teks "Column" tadi, dan ditempat teks "Column" yang sudah dihapus, tempelkan lah item atau teks yang kita inginkan
```html
<div class="container text-center">
    <div class="row row-cols-2">
        <div class="col-md">
            <div>
                <img width="50px" height="50px" src="img/HTML5_badge.png" alt="logo html" class="mt-5">
                <h3>HTML</h3>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. <br>
                    Nobis totam assumenda unde quod et vitae minus beatae, <br> quibusdam impedit laboriosam earum, <br>
                    possimus consequatur quisquam dolore ex ipsa eaque cupiditate neque.</p>
            </div>
        </div>
        <div class="col-lg">
            <div>
                <img width="50px" height="60px" src="img/css-3-logo.png" alt="logo html" class="mt-4">
                <h3>CSS</h3>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. <br>
                    Nobis totam assumenda unde quod et vitae minus beatae, <br> quibusdam impedit laboriosam earum, <br>
                    possimus consequatur quisquam dolore ex ipsa eaque cupiditate neque.</p>
            </div>
        </div>
        <div class="col-sm">
            <div>
                <img width="50px" height="50px" src="img/OIP.jpeg" alt="logo html" class="mt-2">
                <h3>JavaScript</h3>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. <br>
                    Nobis totam assumenda unde quod et vitae minus beatae, <br> quibusdam impedit laboriosam earum, <br>
                    possimus consequatur quisquam dolore ex ipsa eaque cupiditate neque.</p>
            </div>
        </div>
        <div class="col">
            <div>
                <img width="50px" height="50px" src="img/R.png" alt="logo html" class="mt-2">
                <h3>JQuery</h3>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. <br>
                    Nobis totam assumenda unde quod et vitae minus beatae, <br> quibusdam impedit laboriosam earum, <br>
                    possimus consequatur quisquam dolore ex ipsa eaque cupiditate neque.</p>
            </div>
        </div>
    </div>
</div>
```
![[btc-100.png]]
8. Maka hasilnya akan seperti ini:
	![[btc-68.png]]
	*Keterangan:*
	Jadi pada praktek sebelumnya tanpa adanya tambahan pada class bootstrap tadi maka elemen akan menyesuaikan lebar pada pembungkus menjadi full, sedangkan untuk praktek yang saat ini kita tampilkan, item dan teks nya menyesuaikan ukurannya sesuai dengan tambahannnya. Untuk penjelasan ukurannya **Penjelasannya telah kami sediakan di langkah ke-6**.
# Penggunaan Tema
Dalam Bootstrap, tema dasarnya terdiri dari sejumlah variabel CSS yang mengontrol aspek-aspek seperti warna, ukuran teks, jarak, dan banyak lagi. Untuk melakukan kostumisasi tema, kita dapat mengganti nilai-nilai variabel ini sesuai dengan preferensi kita.

Berikut adalah langkah-langkah umum untuk melakukan kostumisasi tema Bootstrap:
1. **Menentukan gaya desain**: Pertama, tentukan gaya desain yang ingin kita terapkan pada situs web kita. Apakah kita ingin tampilan yang lebih minimalis, warna yang cerah, atau mungkin tampilan yang lebih kustom dengan elemen desain yang unik? Menentukan gaya desain akan membantu kita memutuskan bagaimana mengubah tema Bootstrap.
2. **Menggunakan Sass atau CSS**: Bootstrap menyediakan versi Sass (Syntactically Awesome Style Sheets) dari file sumbernya. Sass adalah bahasa pemrograman yang memungkinkan kita menulis CSS dengan sintaks yang lebih kuat dan fleksibel. Jika kita memiliki pengetahuan tentang Sass, kita dapat mengunduh versi Sass Bootstrap dan mengedit variabel-variabelnya. Jika kita tidak familiar dengan Sass , kita masih dapat mengedit file CSS Bootstrap langsung.
3. **Membuat file kustom**: Buat file kustom yang akan berisi kostumisasi tema kita. Dalam file ini, kita dapat menetapkan nilai-nilai variabel yang ingin kita ubah. Misalnya, kita dapat mengubah warna primer, warna latar belakang, ukuran huruf, dan lain sebagainya.
4. **Mengganti variabel**: Temukan variabel yang relevan dalam file sumber Bootstrap dan ubah nilainya sesuai dengan preferensi kita. Misalnya, jika kita ingin mengubah warna primer, cari variabel ==`$primary-color`== atau sejenisnya dalam file sumber dan ubah nilainya menjadi warna yang diinginkan.
5. **Mengompilasi tema kustom**: Setelah kita selesai mengedit file kustom, kita perlu mengompilasinya ke dalam file CSS yang dapat digunakan pada situs web kita. Jika kita menggunakan Sass, kita perlu mengompilasi file Sass menjadi CSS . Jika kita mengedit file CSS langsung, kita dapat menggunakan file tersebut langsung.
6. **Menerapkan tema kustom**: Setelah kita memiliki file CSS tema kustom, kita perlu menggantikan file Bootstrap default dengan file tema kustom kita pada situs web kita. Pastikan untuk menghubungkan file CSS tema kustom kita setelah file Bootstrap default sehingga kostumisasi kita akan ditimpa pada tema default. Kita dapat membuat tema kostuminasi Bootstrap yang sesuai dengan kebutuhan dan gaya desain kita. Penting untuk diingat bahwa jika kita menggunakan versi Bootstrap yang lebih baru, beberapa variabel atau struktur file mungkin telah berubah.

Kita dapat membuat tema kostuminasi Bootstrap yang sesuai dengan kebutuhan dan gaya desain kita. Penting untuk diingat bahwa jika kita menggunakan versi Bootstrap yang lebih baru, beberapa variabel atau struktur file mungkin telah berubah.
# Contoh Penggunaan Tema dalam Bootstrap
1. Jadi misalnya kita ingin memberikan tema pada website yang telah kita buat sebelumnya
	![[btc-70.png]]
2. Bukalah website bootswacth.com dimana website ini menyediakan tema tema yang dapat digunakan untuk web bootstrap kia.
	![[btc-71.png]]
3. Scroll lah ke bawah hingga kita menemukan kumpulan tema tema yang telah disediakaan oleh website ini
	![[btc-72.png]]
4. Misalnya kita akan memilih tema "Darkly", oleh karena itu, klik download pada bagian bawah contoh tema tersebut.
	![[btc-73.png]]
5. Jika sudah mendownloadnya maka kita telah mendapatkan file css untuk tema tersebut
	![[btc-74.png]]
6. Pindahkanlah file css tersebut ke dalam folder yang berisi file html yang akan kita berikan tema
	![[btc-75.png]]
7. Sekarang, masuklah ke dalam file html yang akan kita berikan tema bootstrap, lalu panggillah secara eksternal file css tema tadi ke dalam file html tersebut
	![[btc-76.png]]
8. Maka hasilnya adalah sebagai berikut dengan demikian kita sudah berhasil memberikan tema gelap pada tampilan html kita menggunakan tema dark pada bootstrap
	![[btc-77.png]]
	dengan demikian kita sudah berhasil memberikan tema gelap pada tampilan html kita menggunakan tema dark pada bootstrap
# Modifikasi Template Bootstrap 
Kostumasisasi dalam bootstrap adalah menggunakan template bootstrap kemudian kita akan memodifikasi template tersebut sesuai dengan keinginan kita.

Template dalam Bootstrap adalah struktur dasar atau kerangka kerja yang telah dirancang sebelumnya dan dapat digunakan sebagai dasar untuk membangun halaman web. Bootstrap adalah sebuah framework front-end yang populer digunakan untuk pengembangan web responsif. Dalam konteks Bootstrap, template menyediakan struktur HTML dan gaya CSS dasar yang dapat digunakan sebagai dasar untuk membangun halaman web yang responsif dan mudah diatur.

Dengan menggunakan template Bootstrap, kita dapat menghemat waktu dan usaha dalam merancang tata letak dan gaya dasar dari suatu proyek web. Template ini biasanya sudah mencakup elemen￾elemen umum seperti navigasi, grid system, tombol, formulir, dan banyak lagi. Dengan cara ini, kita dapat fokus pada konten dan fitur unik dari situs web kita tanpa harus memulai dari awal.

Template dalam Bootstrap juga mendukung konsep responsivitas, yang berarti halaman web atau aplikasi yang dibangun dengan menggunakan template ini dapat menyesuaikan diri dengan berbagai ukuran layar, mulai dari perangkat seluler hingga desktop, tanpa perlu penyesuaian tambahan. Ini membuat pengembangan web lebih efisien dan memastikan pengalaman pengguna yang konsisten di berbagai perangkat.

Berikut cara mengkostumisasi template bootstrap:

1. Pertama adalah kita akan membuka sebuah website yang menyediakan template bootstrap. Kali ini web akan kita gunakan adalah themewagon.com
	![[btc-78.png]]
2. Masuklah ke dalam website tersebut
	![[btc-79.png]]
3. Carilah template yang ingin kita sesuaikan dengan cara mensearch ataupun menscroll hingga menemukan tema yang sesuai
	![[btc-80.png]]
4. Jika sudah menemukan template yang kita inginkan, masuk ke template tersebut lalu klik download pada bagian kanan sebelah, contoh gambar dibawah ini.
	![[btc-81.png]]
5. Jika sudah mendownloadnya maka kita telah mendapatkan file template bootsrap kita dalam bentuk zip. File ini berisi asset gambar, style css, index tml, maupun javascript yang menyusun komponen template ini
	![[btc-82.png]]
6. Ekstraklah file tersebut hingga berbentuk seperti file biasa dengan cara klik kanan pada file zip tadi lalu pilih "Extract All".
	![[btc-83.png]]
7. Jika proses ekstrak sudah selesai maka kita tela mendapatkan folder template tersebut dalam bentuk folder biasa
	![[btc-84.png]]
8. Masuklah ke dalam folder template yang telah diekstrak tadi
	![[btc-85.png]]
9. Masuklah ke dalam folder index.html. didalam sana terdapat tampilan template kita
	![[btc-86.png]]
10. Sekarang kita akan mengkostumasisasi tampilan web template ini. Caranya adalah buka file template nya di visual studio code
	![[btc-87.png]]
11. Mulailah mengganti konten-konten seperti teks, gambarm dan lainnya seperti yang kita inginkan. Misalnya saya akan mengganti teks yang ada di gambar ini
	![[btc-.png]]
12. Buka kembali visual studio dan masuk ke file index.html tersebut lalu carilah penyusun konten itu
	![[btc-88.png]]
13. Gantilah kalimat dan tujuan email dan nomor telp itu dengan yang kita inginkan
```html
<a class="navbar-sm-brand text-light text-decoration-none" href="mailto:powershop179@gmail.com">powershop179@gmail.com</a>
<i class="fa fa-phone mx-2"></i>
<a class="navbar-sm-brand text-light text-decoration-none" href="tel:082133273167">082133273167</a>
```
Maka hasilnya akan terlihat seperti dibawah ini:
	![[btc-89.png]]
14. Mulailah mengganti elemen-elemen lainnya sesuai keinginan kita. Misalnya kita ingin juga mengganti logo yang ada di website ini
	![[btc-90.png]]
```html
<a class="navbar-brand text-success logo h1 align-self-center" href="index.html">
    Powershop179
</a>
```
15. Hasil setelah diganti adalah seperti ini
	![[btc-91.png]]
16. Sekarang kita akan mengganti Nama web kita yang ada di slide carousel
	![[btc-92.png]]
```html
<div class="col-lg-6 mb-0 d-flex align-items-center">
    <div class="text-align-left align-self-center">
        <h1 class="h1 text-success"><b>PowerShop179</b> eCommerce</h1>
        <h3 class="h2">Tiny and Perfect eCommerce Template</h3>
        <p>
            PowerShop179 is an eCommerce HTML5 CSS template with the latest version of Bootstrap 5 (beta 1).
            This template is 100% free provided by <a rel="sponsored" class="text-success" href="https://templatemo.com" target="_blank">TemplateMo</a> website. Image credits go to
            <a rel="sponsored" class="text-success" href="https://stories.freepik.com/" target="_blank">Freepik Stories</a>,
            <a rel="sponsored" class="text-success" href="https://unsplash.com/" target="_blank">Unsplash</a> and
            <a rel="sponsored" class="text-success" href="https://icons8.com/" target="_blank">Icons 8</a>.
        </p>
    </div>
</div>

```
Hasilnya akan menjadi seperti ini:
	![[btc-93.png]]
17. bagaimana jika kita ingin mengganti gambar? Misalnya kita akan mengganti gambar yang ada di card ini
	![[btc-94.png]]
18. Masuklah ke visual studio code dan ke index.html tadi lalu carilah kode penyusun untuk gambar ini, kemudian gantilah di bagian src gambar yang sudah ada dengan gambar yang kita inginkan
```html
<a href="shop-single.html">
<img src="./assets/img/feature_prod_01.jpg" class="card-img-top" alt="..." />
</a>
```
Maka haslinya akan menjadi seperti ini:
	![[btc-95.png]]
Demikianlah kostumisasi template bootstrap ini. Kesimpulanya kita dapat mengganti text, gambar, link tujuan, atau menambahkan elemen tertentu sesuai dengan kebutuhan kita. Ini tentunya sangat menghemat waktu dan tenaga, dimana kita hanya fokus pada konten yang kita sajikan dibanding harus menyusun grid, responsif, dan lainnya dari awal
# Studi Kasus Pengaplikasian Bootstrap dalam Desain Web
**Contoh Desain Web Yang Akan di Implementasikan**:
![[bf-1.jpg]]
1. dalam desain web tersebut terdapat beberapa komponen, yaitu
   - Navbar, Hero Section, Button dll
2. Pertama-tama kita perlu Inisialisasikan class ==`container`== agar dapat memberikan tata letak konten yang sesuai dengan desainnya.
```html
<div class="container">
</div>
```
*Keterangan*:
- pada ==`<div class="container">`== : Kelas ini memberikan tata letak yang terkandung pada lebar tertentu (dalam pixel) dan ditengahkan di tengah halaman atau elemen yang memuatnya. Ini membantu dalam mengatur konten agar sesuai dengan standar desain Bootstrap.

3. Selanjutnya kita akan implementasikan navbarnya, bukalah kembali web getbootsrap lalu di kolom pencarian carilah "navbar".
	   ![[bf-2.png]]
4. Cari dan copylah codingan komponen navbar yang mungkin sesuai dengan desainnya.
	   ![[bf-3.png]]
```html
<nav class="navbar navbar-expand-lg bg-body-tertiary"> <div class="container-fluid"> <a class="navbar-brand" href="#">Navbar</a> <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation"> <span class="navbar-toggler-icon"></span> </button> <div class="collapse navbar-collapse" id="navbarSupportedContent"> <ul class="navbar-nav me-auto mb-2 mb-lg-0"> <li class="nav-item"> <a class="nav-link active" aria-current="page" href="#">Home</a> </li> <li class="nav-item"> <a class="nav-link" href="#">Link</a> </li> <li class="nav-item dropdown"> <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false"> Dropdown </a> <ul class="dropdown-menu"> <li><a class="dropdown-item" href="#">Action</a></li> <li><a class="dropdown-item" href="#">Another action</a></li> <li> <hr class="dropdown-divider"> </li> <li><a class="dropdown-item" href="#">Something else here</a></li> </ul> </li> <li class="nav-item"> <a class="nav-link disabled" aria-disabled="true">Disabled</a> </li> </ul> <form class="d-flex" role="search"> <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search"> <button class="btn btn-outline-success" type="submit">Search</button> </form> </div> </div> </nav>
```
*Keterangan*:
	1. ==`navbar`== : Kelas ini menunjukkan bahwa elemen ==`<nav>`== adalah bagian dari komponen navbar. Navbar adalah bagian dari Bootstrap yang menyediakan navigasi di bagian atas halaman web. Dengan memberikan kelas navbar , kita memberitahu Bootstrap untuk menerapkan gaya dan tata letak khusus yang terkait dengan navigasi.
	2. ==`bg-body-tertiary`== : Kelas ini memberikan warna latar belakang pada navbar. Dalam hal ini, warna latar belakangnya diberi warna sesuai dengan warna "hijau" Warna latar belakang ini dapat disesuaikan sesuai kebutuhan desain.
	3. ==`container-fluid`== : Kelas ini diterapkan pada elemen ==`<div>`== yang membungkus elemen-elemen dalam navbar. Kelas ini memberikan padding yang sesuai dan membuat elemen-elemen di dalamnya menjaga lebar penuh dari layar (menggunakan grid system Bootstrap). Dengan kata lain, kontennya akan merespons secara baik pada berbagai lebar perangkat.
	4. ==`d-flex`== : Kelas ini mengubah elemen ==`<form>`== menjadi kontainer flex. Flexbox adalah teknik tata letak yang kuat di CSS yang memudahkan pengaturan dan penataan elemen dalam satu atau dua dimensi. Dengan memberikan kelas d-flex , elemen form dan anak-anaknya dapat disusun secara fleksibel.
	5. ==`me-2`== : Ini adalah kelas Bootstrap yang memberikan margin kanan sebesar 2 pada elemen yang memilikinya. Dalam codingan ini, kelas ini diterapkan pada elemen input untuk memberikan jarak margin kanan.

5. Tempelkanlah kode program itu didalam class ==`container`== sebelumnya pada halaman html terkait. Tentu saja dengan bootstrap yang sudah ditautkan, baik offline, maupun online.
6. Maka hasilnya akan seperti ini:
	   ![[bf-4.png]]
7. Sekarang pada bagian dalam div `navbar-collapse` hapus elemen form:
```html
<form class="d-flex" role="search"> <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search" /> <button class="btn btn-outline-success" type="submit">Search</button> </form>
```
![[bf-r1.png]]
8. Hasilnya akan seperti ini:
	   ![[bf-5.png]]
9. Langkah Selanjutnya kita perlu mengganti list list serta nama logo pada navbarnya
```html
<ul class="navbar-nav me-auto mb-2 mb-lg-0"> <li class="nav-item"> <a class="nav-link active fw-bold" aria-current="page" href="#">Home</a> </li> <li class="nav-item"> <a class="nav-link text-muted" href="#">Discover</a> </li> <li class="nav-item"> <a class="nav-link text-muted" href="#">Post a Job</a> </li> <li class="nav-item"> <a class="nav-link text-muted" href="#">Contact Us</a> </li> </ul>
```
*Keterangan*:
	1. Disini kita mengganti text list item, dari sebelumnya default dari bootstrap ke desain yang akan diimplementasikan seperti: home,discover,post a job dan contact us
	2. ==`fw-bold`== dalam Bootstrap digunakan untuk memberikan tebal pada teks. Kelas ini merupakan bagian dari utilitas ==`font-weight`== yang disediakan oleh Bootstrap, yang memungkinkan Anda untuk dengan cepat mengubah berat font teks dengan kelas `.fw-*`. Kelas ==`fw-bold`== setara dengan berat font 700
	3. ==`text-muted`== digunakan untuk memberi gaya pada teks dengan warna yang redup. Kelas ini merupakan bagian dari utilitas ==`text-color`== yang disediakan oleh Bootstrap, yang memungkinkan Anda untuk dengan mudah mengubah warna teks dengan kelas ==`.text-*`.== Kelas ==`text-muted`== setara dengan warna ==`$gray-600`==, yang merupakan warna abu-abu yang redup.

![[bf-6.png]]
10. Kemudian tambah tombol `sign-up`  di sebelah kanan, sama seperti form namun kita berikan tag anchor
```html
<a href="/sign-up" class="btn btn-outline-dark rounded-0 fw-bold"> Sign Up </a>
```
*Keterangan*:
	1. class ==`btn`==  digunakan untuk mengatur tampilan tombol. Class ini menambahkan beberapa stil ke tampilan tombol, seperti padding, margin, dan warna latar belakang.
	2. ==`btn-outline-dark`== digunakan untuk mengatur tampilan tombol dengan latar belakang transparan dan warna tekstu yang hitam.
	3. ==`rounded-0`==  digunakan untuk mengatur bentuk tombol dengan sudut yang tidak ada (0).
	4. ==`fw-bold`==  digunakan untuk mengatur font teks dengan berat font yang tebal.
	5.  ==`text-muted`==  digunakan untuk mengatur warna teks dengan warna yang redup.

![[bf-7.png]]
11. Selanjutnya ganti background navbarnya dari `bg-body-tertiary` menjadi transparan dengan menggunakan class `bg-trasnparent`
![[bf-r2.png]]
	![[bf-8.png]]
12. Sekarang kita akan menengahkan list navbarnya dengan menggunakan class `m-auto`

sebelum
![[bf-9.png]]
sesudah
![[bf-10.png]]
13. Hasilnya akan seperti ini:
	![[bf-11.png]]
14. Sekarang kita akan implementasikan komponen hero section, tuliskan kode berikut.
```html
<section id="hero"></section>
```
15. dapat kita lihat pada komponen hero terdapat text dan tombol posisinya ditengah, nah disini kita bisa menggunakan grid system bootstrap agar dapat mengatur posisinya.
```html
<div class="row h-100 justify-content-center align-items-center text-center"> <div class="col-12"> <h1 class="fw-bold">Get Connected to the Best Remote <br />Jobs in Your Field </h1> <p class="text-muted">Discover a wide range of remote opportunities on our platform and<br />take control of your career</p> </div> </div>
```
*Keterangan*:
	1.  ==`row`== digunakan untuk mengatur tata letak konten dalam satu baris. Class ini menambahkan beberapa stil ke tata letak konten, seperti mengatur margin dan padding untuk konten yang berada di sisi.
	2.  ==`h-100`== adalah class Bootstrap yang digunakan untuk mengatur tinggi konten dalam sebuah halaman web. Class ini menambahkan stil yang memastikan konten berada pada tinggi penuh dari bagian atas ke bawah.d
	3.  ==`justify-content-center`== adalah class Bootstrap yang digunakan untuk mengatur posisinya konten di tengah bagian horizontal.
	4. class ==`align-items-center`== adalah class Bootstrap yang digunakan untuk mengatur posisinya konten di tengah bagian vertikal.
	5. class ==`text-center`== adalah class Bootstrap yang digunakan untuk mengatur posisi teks di tengah bagian konten.
	6. class ==`col-12`== adalah class Bootstrap yang digunakan untuk mengatur lebar konten. Class ini menambahkan stil yang memastikan konten berada pada lebar penuh dari bagian atas ke bawah.

16. Hasilnya akan seperti ini:
	![[bf-12.png]]
17. Disini text nya hanya ke tengah secara horizontal, agar dapat ke tengah secara vertikal perlu kita atur tinggi pada hero sectionnya dengan external style
```html
<style> #hero { height: 85vh; } </style>
```
![[bf-r3.png]]
*Keterangan*:
	 ini mengatur tinggi dari elemen yang memiliki ID `hero` menjadi 85% dari tinggi viewport (viewport height).

18. Hasilnya akan seperti ini:
	![[bf-13.png]]
19. Sekarang kita akan implementasikan komponen button nya, dapat kita lihat pada desainnya terdapat dua button sejajar secara horizontal, maka kita perlu memakai flexbox yang disediakan oleh bootstrap.
```html
<div class="d-flex gap-4 justify-content-center align-items-center"> <a href="#" class="">Explore Remote Jobs</a> <a href="#" class="">How it works?</a> </div>
```
*Keterangan*:
	1. ==`d-flex`==  digunakan untuk mengatur tata letak konten dalam satu baris. Class ini menambahkan stil yang memastikan konten berada pada satu baris dan tidak berpindah ke baris baru.
	2. ==`gap-4`==  digunakan untuk mengatur jarak antara konten dalam satu baris. Class ini menambahkan stil yang membuat jarak antara konten berada 4 unit.
	3. ==`justify-content-center`== digunakan untuk mengatur posisinya konten di tengah bagian horizontal.
	4. ==`align-items-center`== digunakan untuk mengatur posisinya konten di tengah bagian vertikal.

![[bf-14.png]]
20. Selanjutnya kita perlu beri space dari setiap buttonnya, dan beri warna pada button sebelah kiri
```html
<div class="d-flex gap-4 justify-content-center align-items-center"> <a href="#" class="p-2 px-3 text-decoration-none bg-primary rounded-5 text-white shadow-sm ">Explore Remote Jobs</a> <a href="#" class="p-2 px-3 text-primary rounded-5 fw-semibold">How it works?</a> </div>
```
*Keterangan*:
	1.  ==`p-2`== digunakan untuk mengatur padding pada tautan. Class ini menambahkan stil yang membuat padding pada tautan berada 0.5 unit pada sisi atas dan bawah, serta 0.75 unit pada sisi kiri dan kanan.
	2. ==`px-3`== digunakan untuk mengatur padding pada tautan. Class ini menambahkan stil yang membuat padding pada tautan berada 0.75 unit pada sisi kiri dan kanan.
	3. ==`text-decoration-none`== digunakan untuk mengatur dekorasi teks pada tautan. Class ini menghilangkan dekorasi garis bawah yang biasanya muncul pada tautan.
	4. ==`bg-primary`== digunakan untuk mengatur warna latar belakang pada tautan. Class ini menambahkan stil yang membuat latar belakang tautan berwarna hitam.
	5.  ==`rounded-5`== digunakan untuk mengatur bentuk tautan. Class ini menambahkan stil yang membuat bentuk tautan berbentuk lingkaran dengan jari-jari 5 unit.
	6. ==`text-white`== digunakan untuk mengatur warna teks pada tautan. Class ini menambahkan stil yang membuat warna teks tautan berwarna putih.
	7. ==`shadow-sm`== digunakan untuk mengatur gaya bagian atas tautan. Class ini menambahkan stil yang membuat bagian atas tautan berwarna abu-abu dengan efek shadow.
	8. ==`fw-semibold`== digunakan untuk mengatur font teks dengan berat font yang semibold.
	9. ==`text-primary`== digunakan untuk mengatur warna teks pada tautan. Class ini menambahkan stil yang membuat warna teks tautan berwarna hitam.

![[bf-15.png]]
21. Sekarang kita akan mengganti background body nya
```html
<style> body { background-color: #F6FAFF; background-image: linear-gradient(90deg, #0500FF 0%, #F8FB76 35%, #4EFF75 64%, #00FFD1 100%); background-blend-mode: overlay; } </style>
```
![[bf-r4.png]]
22. Hasilnya akan seperti ini:
	![[bf-16.png]]
# Best Practices dan Tips
## Gunakan Grid Sistem:
Manfaatkan grid sistem Bootstrap untuk mengatur tata letak (layout) situs Anda dengan baik. Gunakan kelas-kelas seperti `container`, `row`, dan `col` untuk membagi konten Anda menjadi bagian-bagian yang sesuai.
## Gunakan Komponen Bootstrap:
Manfaatkan komponen-komponen yang disediakan oleh Bootstrap seperti navbar, card, form, dll. Komponen-komponen ini sudah dirancang dan diuji untuk memastikan konsistensi dan fungsionalitas yang baik.
## Uji pada Berbagai Browser:
Pastikan situs Anda berfungsi dengan baik di berbagai browser, termasuk versi lama dan baru, dengan melakukan pengujian silang browser.


