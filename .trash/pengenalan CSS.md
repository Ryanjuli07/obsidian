# Anatomi CSS
Anatomi css terdiri dari *Selector, Property* dan *Property Value* untuk contoh lebih jelasnya kita akan masuk kedalam contoh dibawah dimana akan dijelaskan contoh dari ketiga anatomi css.
contoh:
```html
p {
	color: red;
}
```
# div & span
DIV adalah elemen tingkat blok yang digunakan untuk membuat bagian, sedangkan SPAN adalah elemen sebaris untuk menata teks atau elemen sebaris lainnya
## div
Div ialah tag yang digunakan untuk mengetikkan sesuatu namun cakupan areanya akan 
mengambil satu block/baris. 
## span
Span ialah tag yang digunakan untuk mengetikkan sesuatu namun cakupan areanya akan mengambil sesuai yang diketikkan saja. 
# percobaan ke 1
kode css:
```html
<style>
       p {
          color: red;
         }
</style>
  
      <p>Welcome CSS</p>
```
hasil:
penjelasan:
disini isi dari tag p berubah menjadi berwarnah merah di akibatkan oleh style css tepatnya property color yang dibarengi dengan value red sehinggan hasil dari tag p yang telah dipanggil oleh style css berubah menjadi warna merah.
# percobaan ke 2
## kode css
```css
<style>
      p {
        color:red;
      }
      button {
          width:150px;
          height:50px;

          border:none;
       font-size:20px;
     background-color:yellow;
      }
    </style>
```
# bordwer
garis batas yang bisa digunakan di setiap elemen. Untuk memperlihatkan garis batas dari sebuah elemen, gunakan properti border pada CSS.
## before
![[IMG_20240224_211425 1.jpg]]
## after
![[IMG_20240224_211417.jpg]]
# font size
Font Size, merupakan atribut yang digunakan dalam Tag Font, untuk mengatur ukuran huruf. Font Face, atribut ini digunakan untuk mengtur jenis huruf yang akan digunakan.
## before
![[IMG_20240224_211405.jpg]]
## after

![[IMG_20240224_211425.jpg]]
# background-color
merupakan attribute untuk menentukan warna pada halaman HTML
## before
![[IMG_20240224_211352 1.jpg]]
## after
![[10.jpg]]

# pemanggilan css

untuk pemanggilan css dibagi menjadi tiga bagian/cara dan ketiga cara tersebut akan dijelaskan di materi di bawah, untuk lebih jelasnya kita akan langsung masuk ke materi dari tiga cara pemanggilan tersebut.

## Inline
Untuk Inline pemanggilannya ialah langsung bersamaan dengan tag yang ingin diketikkan misalnya seperti kode program berikut :

```html
<p style=color: red;>ini cara pemanggilan css inline</p>
```
## internal
Lalu untuk internal cara pemanggilannya ialah dengan diketikkan di dalam dokumen html yang telah kita buat namun berbeda dengan Inline, contoh nya ialah seperti kode program dibawah berikut :
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
Sedangkan External cara pemanggilan ini ialah dengan membuat dokumen khusus css lalu menghubungkan antara dokumen html dan css dengan tag <link> untuk contoh programnya akan seperti berikut :

```html
<head>
	<link rel="stylesheet" href="nama_dokumen_css.css"
</head>

```

# Selector
Untuk selector css dibagi menjadi 3 cara yaitu Elemen Selector, Class selector dan Id selector
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
Untuk Class selector kita memanggil di dokumen khusus css dan menambahkan atribut class pada tag yang ingin di ubah lalu dipanggil menggunakan "." sebelum nama classnya, untuk contoh programnya akan seperti berikut.
halaman html :

```html
<span class="nama_class">Ini contoh class selector</span>
```
halaman css :
```html
.nama_class {
	color: red;
}
```
## Id selector
Untuk Id selector lumayan mirip dengan class selector yaitu dengan menambahkan id di tag yang ingin di ubah lalu setelah itu di panggil menggunakan tagar sebelum nama id nya, untuk contoh programnya akan seperti berikut.
halaman html :
```html
<div id="nama_id">Ini contoh id selector<div>
```
halaman css:
```html
#nama_id {
	color: red;
}
```

# Text,Background & Font
property dasar yang akan kita pelajari ialah mulai dari text font dan background untuk penjelasan yang lebih jelas akan dijelaskan di materi dibawah ini.

## Materi Text
Untuk property text kita akan mempelajari beberapa value dan untuk lebih jelasnya kita akan mempelarinya di bawah ini.

## text-align
text align ini mengatur rata kiri kanan dari sebuah teks yang akan di ketik dan seperti value yang saya gunakan ialah untuk mengatur tulisannya menjadi tengah dengan value "center" dan contoh programnya ialah seperti berikut :
```html
.text_align {
    text-align: center;
}
```

![[IMG_20240324_215036.jpg]]
## text-decoration
text-decoration berfungsi untuk memberi dekorasi pada teks yang akan ditulis sesuai dengan value yang akan digunakan seperti contoh yang saya ambil yaitu *"underline"* yang berfungsi untuk membuat garis dibawah tulisan, untuk contohnya akan seperti berikut :
```css
.text_decoration {
    text-decoration:underline;
}
```
hasil:
## text-trasformation
text-transformation ini berfungsi untuk mengtransformasikan teks yang telah dibuat seperti contoh yang saya gunakan ialah membuat teks menjadi kapital menggunakan value *"uppercase"* untuk contohnya akan seperti dibawah ini :
```css
.text_transformation {
    text-transform:uppercase;
}
```
hasil:
## teks-indent
teks-indent ini berfungsi untuk memberi jarak di awal penulisan atau simpelnya seperti mengetik "tab" pada keayboard kita dan untuk valuenya dapat di isi sesuai dengan keinginan kita. Contohnya akan seperti berikut :
```css
.text_indent {
    text-indent: 20px;
}
```
hasil:
## letter-spacing
lalu untuk latter-spacing ialah untuk memberi jarak di antara setiap huruf yang telah diketikkan dan untuk valuenya dapat ditentukan sesuai keignginan kita, untuk lebih jelasnya berikut contoh program dan asilnya :
```css
.letter_spacing {
    letter-spacing: 6px;
}
```
hasil:
## line-height
untuk line-height ialah untuk memberi jarak pada suatu teks dengan teks di atasnya dan valuenya dapat di atur sesuai dengan keinginan, lalu untuk contoh program serta hasilnya akan seperti dibawah ini :
```css
.line_height {
&nbsp; &nbsp; line-height: 100px;
}
```
hasil:
## word-spacing
dan terakhir ialah word-spacing fungsinya untuk memberi jarak di antara setiap kata dan valuenya dapat di atur sesuai keinginan kita, lalu untuk contoh program dan hasilnya akan seperti berikut :
```css
.word_spacing {
&nbsp; &nbsp; word-spacing: 10px;
}
```
hasil:
## Materi Background
Untuk property background kita akan mempelajari beberapa value dan untuk lebih jelasnya kita akan mempelarinya di bawah ini.

## background-image
untuk background image ini kita akan dapat menampilkan background dengan image sesuai dengan yang ingin kita pilih/dari file kita, untuk contoh programnya akan seperti berikut :
```css
.background-image {
    background-image:url(./aset/backgroundd.JPG)
}
```
hasil:
## background-size
lalu untuk background size kita mengatur size/ukuran dari background yang kita gunakan dan valuenya dapat kita atur sesuai dengan keinginan kita. untuk contoh penggunananya akan seperti berikut ini :
```css
.background {
    background-image:url(./aset/backgroundd.JPG);
    width: 100%;
    height: 100VH;
    
    background-size: 50%;
}
```
hasil:
## background-repeat
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
hasil:
## background-attachment
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
hasil:
## Background-postion
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
hasil:
## Materi Font
Untuk  property font kita akan mempelajari beberapa value dan untuk lebih jelasnya kita akan mempelarinya di bawah ini.
## Font-size
untuk font-size berfungsi untuk mengatur ukuran dari teks yang di ketikkan dan valuenya dapat di atur sesuai dengan keinginan kita, untuk contoh program dan hasilnya akan seperti dibawah ini :
```css
.teks {
    font-size: 10px;
}
```
hasil:
## Font-style
untuk font-style berfungsi untuk mengatur gaya dari teks yang diketikkan untuk value bisa dipilih sesuai dengan yang kita inginkan, contohnya saya disini saya menggunakan *italic* untuk program dan hasilnya akan seperti dibawah ini :
```css
.teks {
    font-size: 10px;
    font-style:italic;
}
```
hasil:
## Font-weight
untuk font-weight adalah untuk mengatur ketebalan dari teks yang kita ketikkan dan untuk valuenya dapat kita pilih sesuai dengan keinginan kita dan disini saya menggunakan value *bold* untuk contoh programnya akan seperti berikut :
```css
.teks {
    font-size: 10px;
    font-style:italic;
    font-weight:bold;
}
```
hasil:
## Font-family
dan yang terakhir ialah font-family ialah untuk mengatur jenis font yang diinginkan seperti contoh yang saya gunakan ialah value *arial* dan contoh program serta hasilnya akan seperti berikut :
```css
.teks {
    font-size: 10px;
    font-style:italic;
    font-weight:bold;
    font-family:arial;
}
```

# Box model
Untuk box model kita akan mempelajari mengenai border, padding, margin dan hal hal lainnya mengenai permodelan box. untuk lebih jelasnya kita akan menggunakan contoh di bawah :

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

## Border
untuk border terdapat beberapa jenis yang akan digunakan mulai dari radius,width,color dan style untuk penjelasan lebih  lanjutnya akan dijelaskan di sub materi di bawah.
## Border-radius
Untuk border-radius ini berfungsi untuk mengatur radius pada border, semakin tinggi radius semakin berkurang radius pada bordernya/semakin melengkung.
## Border-width
Untuk border-width ini berfungsi menebalkan border atau menebalkan radius pada border dan dapat ditebalkan sesuai value yang diinginkan disini saya menggunakan value 10px sehingga ketebalannya bertambah lebih dari biasanya.

## Border-color
Untuk border-color ini untuk mengatur warna border yang telah dibuat dan valuenya dapat di atur sesuai dengan keinginan kita, valuenya ini berupa warna.

## Border-style
Dan Terakhir ialah border-style, border-style ini kita dapat menggunakan value solid untuk membuat bordernya memiliki warna solid dan tanpa bayangan/shadow.

## Padding
untuk padding terdapat beberapa jenis yang akan digunakan mulai dari right,left,top dan bottom untuk penjelasan lebih lanjutnya akan dijelaskan di sub materi di bawah.

## Padding-left
Padding-left ini berfungsi untuk mengatur jarak antara objek dengan bordernya khusus untuk bagian sebelah kiri.

## Padding-right
Padding-right ini berfungsi untuk mengatur jarak antara objek dengan bordernya khusus untuk bagian sebelah kanan.

## Padding-top
Padding-top ini berfungsi untuk mengatur jarak antara objek dengan bordernya khusus untuk bagian sebelah atas.

## Padding-bottom
Padding-bottom ini berfungsi untuk mengatur jarak antara objek dengan bordernya khusus untuk bagian sebelah bawah.

## Contoh Border Lain
Untuk contoh border kedua ialah menggunakan margin untuk mengatur jarak buttonnya untuk contohnya akan seperti di bawah ini :

## Margin
Fungsi dari margin yang akan kita pelajari ialah fungsi dari margin right,left,top dan bottom. Untuk lebih jelasnya akan dijelaskan di bawah ini.

## Margin-right
Margin-right ini mengatur jarak antar objek satu dengan objek lainnya lebih tepatnya ke arah kanan objeknya.

## Margin-left
Margin-left ini mengatur jarak antar objek satu dengan objek lainnya lebih tepatnya ke arah kiri objeknya.

## Margin-top
Margin-top ini mengatur jarak antar objek satu dengan objek lainnya lebih tepatnya ke arah atas objeknya.

## Margin-bottom
Margin-bottom ini mengatur jarak antar objek satu dengan objek lainnya lebih tepatnya ke arah bawah objeknya.



