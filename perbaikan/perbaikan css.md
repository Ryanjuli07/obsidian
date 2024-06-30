# selector
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contoh Anatomi CSS</title>
    <style>
        /* Selector: Elemen HTML */
        body {
            /* Property: background-color, Property Value: #f4f4f4 */
            background-color: #f4f4f4;
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 20px;
        }

        /* Selector: Kelas */
        .container {
            /* Property: max-width, Property Value: 600px */
            max-width: 600px;
            margin: 0 auto;
            background-color: #fff;
            padding: 20px;
            box-shadow: 0 0 10px rgba(0,0,0,0.1);
        }

        /* Selector: Elemen HTML */
        h1 {
            /* Property: text-align, Property Value: center */
            text-align: center;
        }

        /* Selector: ID */
        #specialMessage {
            /* Property: color, Property Value: #ff0000 */
            color: #ff0000;
            font-weight: bold;
        }

        /* Selector: Pseudo-class */
        a:hover {
            /* Property: color, Property Value: #0056b3 */
            color: #0056b3;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Contoh Anatomi CSS</h1>
        <p>Ini adalah contoh penggunaan berbagai selector, property, dan property value dalam CSS.</p>
        <p id="specialMessage">Ini adalah pesan khusus dengan ID.</p>
        <a href="#">Link yang berubah warna saat di-hover</a>
    </div>
</body>
</html>
```

analisis
Selector

Elemen HTML: Menargetkan elemen langsung seperti body dan h1. Contoh: body { ... }.
Class: Menargetkan elemen dengan class tertentu seperti .container. Contoh: .container { ... }.
ID: Menargetkan elemen dengan ID tertentu seperti #specialMessage. Contoh: #specialMessage { ... }.
Pseudo-class: Menargetkan elemen pada kondisi tertentu seperti a:hover (ketika link di-hover). Contoh: a:hover { ... }.
Property dan Property Value

Property: Karakteristik yang diatur, seperti background-color, font-family, margin, dll.
Property Value: Nilai yang diberikan pada properti tersebut, seperti #f4f4f4 untuk background-color atau center untuk text-align.
Contoh: background-color: #f4f4f4; mengatur warna latar belakang elemen menjadi #f4f4f4.
Program ini mendemonstrasikan penggunaan berbagai selector untuk menargetkan elemen, serta property dan property value untuk mengatur tampilan elemen-elemen tersebut. Selector digunakan untuk memilih elemen mana yang ingin diubah tampilannya, property menentukan apa yang diubah, dan property value memberikan nilai spesifik untuk perubahan tersebut
# div&span
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contoh Penggunaan div dan span</title>
    <style>
        .container {
            background-color: #f9f9f9;
            padding: 20px;
            margin: 20px auto;
            max-width: 800px;
            border: 1px solid #ddd;
        }

        .header {
            background-color: #007BFF;
            color: white;
            padding: 10px;
            text-align: center;
        }

        .content {
            padding: 20px;
        }

        .highlight {
            color: #007BFF;
            font-weight: bold;
        }

        .footer {
            background-color: #f1f1f1;
            padding: 10px;
            text-align: center;
            border-top: 1px solid #ddd;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <h1>Contoh Penggunaan div dan span</h1>
        </div>
        <div class="content">
            <p>Ini adalah paragraf dengan kata <span class="highlight">highlighted</span>.</p>
        </div>
        <div class="footer">
            &copy; 2024 Contoh Footer
        </div>
    </div>
</body>
</html>
```

analisis
div:

Struktur: Digunakan sebagai kontainer blok untuk membagi bagian halaman (container, header, content, footer).
Styling: Class .container untuk mengatur latar belakang, padding, margin, lebar maksimum, dan border.
span:

Inline: Digunakan untuk penandaan teks tanpa memulai baris baru.
Styling: Class .highlight mengatur warna teks dan ketebalan font.
# inline
```html
<p style="color: red;">ini cara pemanggilan css inline</p>
```

analisis
HTML:

Elemen p digunakan untuk mendefinisikan paragraf.
CSS Inline:

Inline Style: Properti CSS didefinisikan langsung di dalam tag HTML menggunakan atribut style.
Property dan Property Value: color: red; mengatur warna teks elemen p menjadi merah.
# internal

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

analisis
HTML:

Elemen head: Menyimpan informasi tentang dokumen dan elemen-elemen seperti meta, title, dan style.

Elemen style: Menyimpan kode CSS yang diterapkan pada halaman web.

CSS Internal:

Selector: p menargetkan semua elemen paragraf (p) dalam dokumen.
Property dan Property Value: 

color: red; mengatur warna teks semua elemen paragraf menjadi merah.

Body:

Elemen p: Paragraf ini akan mendapatkan warna teks merah sesuai dengan aturan CSS yang didefinisikan dalam tag `<style>`.

# eternal

```html
<head>
	<link rel="stylesheet" href="nama_dokumen_css.css"
</head>
```

analisis
HTML:

Elemen head: Menyimpan metadata dan referensi ke resource eksternal seperti CSS.
Elemen link: Menghubungkan dokumen HTML dengan file CSS 

eksternal.
Atribut rel: Menentukan hubungan antara dokumen HTML dan resource yang dihubungkan, dalam hal ini stylesheet.
Atribut href: Menentukan path atau URL dari file CSS eksternal (nama_dokumen_css.css).

CSS Eksternal:

File Eksternal: Semua aturan CSS didefinisikan dalam file terpisah (nama_dokumen_css.css).

Keuntungan:
Pemeliharaan: Mudah dikelola karena semua aturan CSS berada di satu tempat.

Efisiensi: Memungkinkan penggunaan ulang stylesheet yang sama di beberapa halaman, mengurangi redundansi dan ukuran dokumen HTML.

Performa: Browser dapat menyimpan cache file CSS eksternal, mempercepat waktu muat halaman untuk pengguna.

Body:

Elemen p: Paragraf ini akan menerima gaya yang ditentukan dalam file nama_dokumen_css.css.
Penggunaan CSS eksternal adalah praktik terbaik untuk situs web dengan beberapa halaman atau aturan CSS yang kompleks, karena memisahkan konten (HTML) dari presentasi (CSS) dan meningkatkan efisiensi serta keterbacaan kode.
# selector

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Selector Example</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <h1>Heading 1 - Elemen Selector</h1>
    <p class="text">This is a paragraph with a class selector.</p>
    <p id="uniqueText">This is a paragraph with an ID selector.</p>
    <div>
        <p>This is another paragraph inside a div element.</p>
    </div>
</body>
</html>
```

```css
/* Elemen Selector */
h1 {
    color: blue;
    font-size: 24px;
}

/* Class Selector */
.text {
    color: green;
    font-size: 18px;
}

/* ID Selector */
#uniqueText {
    color: red;
    font-size: 20px;
}

/* Additional Example: Nested Elemen Selector */
div p {
    color: purple;
    font-size: 16px;
}
```

Analisis
Elemen Selector:

h1 { color: blue; font-size: 24px; }
Selector ini memilih semua elemen `<h1>` di dalam dokumen HTML dan mengaplikasikan gaya teks berwarna biru dengan ukuran font 24px.
Class Selector:

.text { color: green; font-size: 18px; }
Selector ini memilih semua elemen yang memiliki atribut class="text". Dalam contoh ini, paragraf pertama yang memiliki kelas text akan memiliki teks berwarna hijau dengan ukuran font 18px.
ID Selector:

#uniqueText { color: red; font-size: 20px; }
Selector ini memilih elemen yang memiliki atribut id="uniqueText". Dalam contoh ini, paragraf kedua yang memiliki ID uniqueText akan memiliki teks berwarna merah dengan ukuran font 20px.

# text

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Text Properties Example</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <h1>Text Properties Example</h1>
    
    <p class="text-align">This text is center-aligned using the <code>text-align</code> property.</p>
    <p class="text-decoration">This text has an underline using the <code>text-decoration</code> property.</p>
    <p class="text-transform">this text is transformed to uppercase using the <code>text-transform</code> property.</p>
    <p class="text-indent">This text is indented using the <code>text-indent</code> property.</p>
    <p class="letter-spacing">This text has increased letter spacing using the <code>letter-spacing</code> property.</p>
    <p class="line-height">This text has increased line height using the <code>line-height</code> property, making it more readable.</p>
    <p class="word-spacing">This text has increased word spacing using the <code>word-spacing</code> property.</p>
</body>
</html>
```

```css
body {
    font-family: Arial, sans-serif;
    margin: 20px;
}

/* Text Align */
.text-align {
    text-align: center;
}

/* Text Decoration */
.text-decoration {
    text-decoration: underline;
}

/* Text Transform */
.text-transform {
    text-transform: uppercase;
}

/* Text Indent */
.text-indent {
    text-indent: 50px;
}

/* Letter Spacing */
.letter-spacing {
    letter-spacing: 2px;
}

/* Line Height */
.line-height {
    line-height: 2;
}

/* Word Spacing */
.word-spacing {
    word-spacing: 10px;
}
```

Analisis
Text Align:

text-align: center;
Properti ini mengatur perataan teks. Dalam contoh ini, teks di paragraf akan diratakan di tengah.

Text Decoration:

text-decoration: underline;
Properti ini mengatur dekorasi teks. Dalam contoh ini, teks di paragraf akan diberi garis bawah.

Text Transform:

text-transform: uppercase;
Properti ini mengatur transformasi teks. Dalam contoh ini, teks di paragraf akan diubah menjadi huruf kapital semua.

Text Indent:

text-indent: 50px;
Properti ini mengatur indentasi baris pertama dari teks dalam sebuah elemen blok. Dalam contoh ini, baris pertama teks di paragraf akan diberi indentasi sebesar 50 piksel.

Letter Spacing:

letter-spacing: 2px;
Properti ini mengatur jarak antar huruf. Dalam contoh ini, jarak antar huruf di paragraf akan ditambah sebesar 2 piksel.

Line Height:

line-height: 2;
Properti ini mengatur tinggi baris teks. Dalam contoh ini, tinggi baris teks di paragraf akan digandakan, membuat teks lebih mudah dibaca.

Word Spacing:

word-spacing: 10px;
Properti ini mengatur jarak antar kata. Dalam contoh ini, jarak antar kata di paragraf akan ditambah sebesar 10 piksel.

Dengan menggunakan atribut style langsung di elemen HTML, kita dapat dengan mudah mengatur tampilan teks tanpa memerlukan file CSS terpisah.
# background 
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Background Properties Example</title>
</head>
<body>
    <h1>Background Properties Example</h1>

    <!-- Background Image -->
    <div style="background-image: url('https://via.placeholder.com/300'); height: 200px; width: 300px;">
        <p>This div uses a background image.</p>
    </div>
    <br>
    
    <!-- Background Size -->
    <div style="background-image: url('https://via.placeholder.com/300'); background-size: cover; height: 200px; width: 300px;">
        <p>This div uses background-size: cover.</p>
    </div>
    <br>
    
    <!-- Background Repeat -->
    <div style="background-image: url('https://via.placeholder.com/100'); background-repeat: no-repeat; height: 200px; width: 300px;">
        <p>This div uses background-repeat: no-repeat.</p>
    </div>
    <br>
    
    <!-- Background Attachment -->
    <div style="background-image: url('https://via.placeholder.com/300'); background-attachment: fixed; height: 200px; width: 300px; overflow: auto;">
        <p>This div uses background-attachment: fixed. Scroll this text to see the effect.</p>
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla nec purus ut nunc ornare vulputate. Vestibulum ac dui id lacus auctor feugiat. Ut pulvinar, massa in vehicula fermentum, purus orci egestas elit, a cursus augue nunc at enim.</p>
    </div>
    <br>
    
    <!-- Background Position -->
    <div style="background-image: url('https://via.placeholder.com/300'); background-position: center; height: 200px; width: 300px;">
        <p>This div uses background-position: center.</p>
    </div>
</body>
</html>

```

analisis
Analisis
Background Image:

background-image: url('https://via.placeholder.com/300');
Properti ini mengatur gambar latar belakang untuk elemen. Dalam contoh ini, div menggunakan gambar dari URL yang diberikan sebagai latar belakang.

Background Size:

background-size: cover;
Properti ini mengatur ukuran gambar latar belakang. Dalam contoh ini, cover membuat gambar latar belakang menutupi seluruh elemen tanpa mengubah rasio aspek gambar.

Background Repeat:

background-repeat: no-repeat;
Properti ini mengatur pengulangan gambar latar belakang. Dalam contoh ini, no-repeat mencegah gambar latar belakang diulang.

Background Attachment:

background-attachment: fixed;
Properti ini mengatur apakah gambar latar belakang bergulir dengan konten halaman atau tetap tetap. Dalam contoh ini, fixed membuat gambar latar belakang tetap di tempat saat konten bergulir.

Background Position:

background-position: center;
Properti ini mengatur posisi gambar latar belakang. Dalam contoh ini, center menempatkan gambar latar belakang di tengah elemen.
Dengan menggunakan atribut style langsung di elemen HTML, kita dapat dengan mudah mengatur properti latar belakang tanpa memerlukan file CSS terpisah. 

Properti-properti ini membantu dalam mengontrol bagaimana gambar latar belakang ditampilkan dan berperilaku dalam elemen HTM
# font

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Font Properties Example</title>
</head>
<body>
    <h1>Font Properties Example</h1>
    
    <!-- Font Size -->
    <p style="font-size: 20px;">This text has a font size of 20 pixels using the <code>font-size</code> property.</p>
    
    <!-- Font Style -->
    <p style="font-style: italic;">This text is italicized using the <code>font-style</code> property.</p>
    
    <!-- Font Weight -->
    <p style="font-weight: bold;">This text is bold using the <code>font-weight</code> property.</p>
    
    <!-- Font Family -->
    <p style="font-family: 'Arial', sans-serif;">This text uses the Arial font family using the <code>font-family</code> property.</p>
</body>
</html>
```

analisis
Analisis
Font Size:

font-size: 20px;
Properti ini mengatur ukuran teks. Dalam contoh ini, teks di paragraf memiliki ukuran font 20 piksel.
Font Style:

font-style: italic;
Properti ini mengatur gaya teks. Dalam contoh ini, teks di paragraf dibuat miring (italic).
Font Weight:

font-weight: bold;
Properti ini mengatur ketebalan teks. Dalam contoh ini, teks di paragraf dibuat tebal (bold).
Font Family:

font-family: 'Arial', sans-serif;
Properti ini mengatur jenis font yang digunakan untuk teks. Dalam contoh ini, teks di paragraf menggunakan font Arial. Jika Arial tidak tersedia, font default sans-serif akan digunakan.

Dengan menggunakan atribut style langsung di elemen HTML, kita dapat dengan mudah mengatur berbagai properti font tanpa memerlukan file CSS terpisah. 
Properti-properti ini membantu dalam mengontrol tampilan teks, seperti ukuran, gaya, ketebalan, dan jenis font yang digunakan.

# Box model
Untuk box model kita akan mempelajari mengenai border, padding, margin dan hal hal lainnya mengenai permodelan box

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Border Properties Example</title>
</head>
<body>
    <h1>Border Properties Example</h1>

    <!-- Border Radius -->
    <div style="border: 2px solid black; border-radius: 15px; padding: 20px; margin-bottom: 20px;">
        <p>This div has a border radius of 15 pixels using the <code>border-radius</code> property.</p>
    </div>
    
    <!-- Border Width -->
    <div style="border: 5px solid black; padding: 20px; margin-bottom: 20px;">
        <p>This div has a border width of 5 pixels using the <code>border-width</code> property.</p>
    </div>
    
    <!-- Border Color -->
    <div style="border: 2px solid red; padding: 20px; margin-bottom: 20px;">
        <p>This div has a red border using the <code>border-color</code> property.</p>
    </div>
    
    <!-- Border Style -->
    <div style="border: 2px dashed black; padding: 20px; margin-bottom: 20px;">
        <p>This div has a dashed border using the <code>border-style</code> property.</p>
    </div>
</body>
</html>
```

analisis 
Analisis

Border Radius:

border-radius: 15px;
Properti ini mengatur sudut-sudut elemen agar membulat. Dalam contoh ini, div memiliki sudut yang melengkung dengan radius 15 piksel.

Border Width:

border-width: 5px;
Properti ini mengatur lebar garis border. Dalam contoh ini, div memiliki border dengan lebar 5 piksel.

Border Color:

border-color: red;
Properti ini mengatur warna garis border. Dalam contoh ini, div memiliki border berwarna merah.

Border Style:

border-style: dashed;
Properti ini mengatur gaya garis border. Dalam contoh ini, div memiliki border dengan gaya garis putus-putus (dashed).

Dengan menggunakan atribut style langsung di elemen HTML, kita dapat dengan mudah mengatur berbagai properti border tanpa memerlukan file CSS terpisah. Properti-properti ini membantu dalam mengontrol tampilan border, seperti bentuk sudut, lebar, warna, dan gaya garis.
# padding

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Padding Properties Example</title>
</head>
<body>
    <h1>Padding Properties Example</h1>

    <!-- Padding Left -->
    <div style="border: 1px solid black; padding-left: 20px; margin-bottom: 20px;">
        <p>This div has left padding of 20 pixels using the <code>padding-left</code> property.</p>
    </div>
    
    <!-- Padding Right -->
    <div style="border: 1px solid black; padding-right: 20px; margin-bottom: 20px;">
        <p>This div has right padding of 20 pixels using the <code>padding-right</code> property.</p>
    </div>
    
    <!-- Padding Top -->
    <div style="border: 1px solid black; padding-top: 20px; margin-bottom: 20px;">
        <p>This div has top padding of 20 pixels using the <code>padding-top</code> property.</p>
    </div>
    
    <!-- Padding Bottom -->
    <div style="border: 1px solid black; padding-bottom: 20px; margin-bottom: 20px;">
        <p>This div has bottom padding of 20 pixels using the <code>padding-bottom</code> property.</p>
    </div>
</body>
</html>
```

analisis
Padding Left:

padding-left: 20px;
Properti ini mengatur jarak antara konten elemen dan batas kiri elemen. Dalam contoh ini, div memiliki jarak padding kiri sebesar 20 piksel.
Padding Right:

padding-right: 20px;
Properti ini mengatur jarak antara konten elemen dan batas kanan elemen. Dalam contoh ini, div memiliki jarak padding kanan sebesar 20 piksel.
Padding Top:

padding-top: 20px;
Properti ini mengatur jarak antara konten elemen dan batas atas elemen. Dalam contoh ini, div memiliki jarak padding atas sebesar 20 piksel.
Padding Bottom:

padding-bottom: 20px;
Properti ini mengatur jarak antara konten elemen dan batas bawah elemen. Dalam contoh ini, div memiliki jarak padding bawah sebesar 20 piksel.

Dengan menggunakan atribut style langsung di elemen HTML, kita dapat dengan mudah mengatur berbagai properti padding tanpa memerlukan file CSS terpisah. Properti-properti ini membantu dalam mengontrol jarak antara konten elemen dan batas elemen itu sendiri, sehingga memberikan kontrol yang lebih baik terhadap tata letak dan ruang di dalam elemen.

# margin

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Margin Properties Example</title>
</head>
<body>
    <h1>Margin Properties Example</h1>

    <!-- Margin Right -->
    <div style="border: 1px solid black; margin-right: 20px;">
        <p>This div has right margin of 20 pixels using the <code>margin-right</code> property.</p>
    </div>
    <br>
    
    <!-- Margin Left -->
    <div style="border: 1px solid black; margin-left: 20px;">
        <p>This div has left margin of 20 pixels using the <code>margin-left</code> property.</p>
    </div>
    <br>
    
    <!-- Margin Top -->
    <div style="border: 1px solid black; margin-top: 20px;">
        <p>This div has top margin of 20 pixels using the <code>margin-top</code> property.</p>
    </div>
    <br>
    
    <!-- Margin Bottom -->
    <div style="border: 1px solid black; margin-bottom: 20px;">
        <p>This div has bottom margin of 20 pixels using the <code>margin-bottom</code> property.</p>
    </div>
</body>
</html>
```

analisis
Analisis
Margin Right:

margin-right: 20px;
Properti ini mengatur jarak luar elemen dari elemen di sebelah kanan. Dalam contoh ini, div memiliki margin kanan sebesar 20 piksel.
Margin Left:

margin-left: 20px;
Properti ini mengatur jarak luar elemen dari elemen di sebelah kiri. Dalam contoh ini, div memiliki margin kiri sebesar 20 piksel.
Margin Top:

margin-top: 20px;
Properti ini mengatur jarak luar elemen dari elemen di atasnya. Dalam contoh ini, div memiliki margin atas sebesar 20 piksel.
Margin Bottom:

margin-bottom: 20px;
Properti ini mengatur jarak luar elemen dari elemen di bawahnya. Dalam contoh ini, div memiliki margin bawah sebesar 20 piksel.

Dengan menggunakan atribut style langsung di elemen HTML, kita dapat dengan mudah mengatur berbagai properti margin tanpa memerlukan file CSS terpisah. Properti-properti ini membantu dalam mengontrol jarak luar elemen dari elemen-elemen lain di sekitarnya, memberikan kontrol yang lebih baik terhadap tata letak dan ruang di luar elemen.
# pseudo

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Pseudo-class Example</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <h1>Pseudo-class Example</h1>
    
    <button class="hover-button">Hover over me</button>
    <br><br>
    <button class="active-button">Click me</button>
</body>
</html>
```

```css
/* Hover Pseudo-class */
.hover-button {
    background-color: lightblue;
    border: 2px solid blue;
    padding: 10px 20px;
    font-size: 16px;
    cursor: pointer;
}

.hover-button:hover {
    background-color: blue;
    color: white;
}

/* Active Pseudo-class */
.active-button {
    background-color: lightgreen;
    border: 2px solid green;
    padding: 10px 20px;
    font-size: 16px;
    cursor: pointer;
}

.active-button:active {
    background-color: green;
    color: white;
}
```

analisis
Analisis
Hover Pseudo-class:

hover-button:hover
Pseudo-class :hover diterapkan pada elemen ketika pengguna mengarahkan kursor ke elemen tersebut. Dalam contoh ini, tombol dengan kelas hover-button akan berubah warna latar belakang menjadi biru dan warna teks menjadi putih ketika pengguna mengarahkan kursor ke tombol tersebut.
Penggunaan:
css
Salin kode
.hover-button:hover {
    background-color: blue;
    color: white;
}
Hasil: Saat pengguna mengarahkan kursor ke tombol, tampilannya akan berubah sesuai dengan aturan yang didefinisikan dalam pseudo-class :hover.
Active Pseudo-class:

active-button:active
Pseudo-class :active diterapkan pada elemen ketika elemen tersebut sedang dalam keadaan aktif, seperti saat tombol ditekan. Dalam contoh ini, tombol dengan kelas active-button akan berubah warna latar belakang menjadi hijau dan warna teks menjadi putih ketika tombol tersebut ditekan.
Penggunaan:
css
Salin kode
.active-button:active {
    background-color: green;
    color: white;
}
Hasil: Saat pengguna menekan tombol, tampilannya akan berubah sesuai dengan aturan yang didefinisikan dalam pseudo-class :active.

Dengan menggunakan pseudo-class hover dan active, kita dapat memberikan umpan balik visual yang interaktif kepada pengguna, meningkatkan pengalaman pengguna (user experience) dengan memperjelas tindakan yang mereka lakukan pada elemen interaktif seperti tombol.
# transition
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Transition Properties Example</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <h1>Transition Properties Example</h1>
    
    <div class="transition-example">Hover over me</div>
    <br>
    <div class="transition-delay-example">Hover over me</div>
    <br>
    <div class="transition-duration-example">Hover over me</div>
    <br>
    <div class="transition-property-example">Hover over me</div>
    <br>
    <div class="transition-timing-function-example">Hover over me</div>
</body>
</html>
```

```css
/* Basic Transition */
.transition-example {
    width: 100px;
    height: 100px;
    background-color: lightblue;
    transition: background-color 2s;
}

.transition-example:hover {
    background-color: blue;
}

/* Transition Delay */
.transition-delay-example {
    width: 100px;
    height: 100px;
    background-color: lightgreen;
    transition: background-color 2s 1s; /* duration and delay */
}

.transition-delay-example:hover {
    background-color: green;
}

/* Transition Duration */
.transition-duration-example {
    width: 100px;
    height: 100px;
    background-color: lightcoral;
    transition: background-color 3s; /* duration */
}

.transition-duration-example:hover {
    background-color: red;
}

/* Transition Property */
.transition-property-example {
    width: 100px;
    height: 100px;
    background-color: lightgoldenrodyellow;
    transition-property: background-color;
    transition-duration: 2s;
}

.transition-property-example:hover {
    background-color: gold;
}

/* Transition Timing Function */
.transition-timing-function-example {
    width: 100px;
    height: 100px;
    background-color: lightpink;
    transition: background-color 2s ease-in-out; /* timing function */
}

.transition-timing-function-example:hover {
    background-color: deeppink;
}
```

analisis
Analisis
Basic Transition:

transition: background-color 2s;
Properti ini mengatur transisi perubahan warna latar belakang selama 2 detik. Saat pengguna mengarahkan kursor ke elemen div, warna latar belakang akan berubah dari lightblue menjadi blue dengan transisi yang halus.
Hasil: Transisi halus warna latar belakang selama 2 detik.

Transition Delay:

transition: background-color 2s 1s;
Properti ini mengatur transisi perubahan warna latar belakang selama 2 detik dengan penundaan 1 detik. Saat pengguna mengarahkan kursor ke elemen div, transisi akan dimulai setelah 1 detik.
Hasil: Transisi halus warna latar belakang dimulai setelah penundaan 1 detik dan berlangsung selama 2 detik.

Transition Duration:

transition: background-color 3s;
Properti ini mengatur durasi transisi selama 3 detik. Saat pengguna mengarahkan kursor ke elemen div, warna latar belakang akan berubah dari lightcoral menjadi red selama 3 detik.
Hasil: Transisi halus warna latar belakang selama 3 detik.

Transition Property:

transition-property: background-color;
transition-duration: 2s;
Properti ini mengatur transisi hanya untuk perubahan warna latar belakang selama 2 detik. Saat pengguna mengarahkan kursor ke elemen div, hanya perubahan warna latar belakang yang akan ditransisikan.
Hasil: Transisi halus warna latar belakang selama 2 detik.
Transition Timing Function:
# transform
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Transform Properties Example</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <h1>Transform Properties Example</h1>
    
    <div class="scale-example">Scale(0.5)</div>
    <br>
    <div class="scalex-example">ScaleX(0.5)</div>
    <br>
    <div class="rotate-example">Rotate(45deg)</div>
    <br>
    <div class="skewx-example">SkewX(-25deg)</div>
    <br>
    <div class="skew-example">Skew(25deg, 5deg)</div>
    <br>
    <div class="translate-example">Translate(50px, 52px)</div>
    <br>
    <div class="matrix-example">Matrix(0.7, -0.5, 0.5, 0.4, 0.5, 0.7)</div>
</body>
</html>
```

```css
/* Transform: Scale(0.5) */
.scale-example {
    width: 100px;
    height: 100px;
    background-color: lightblue;
    transform: scale(0.5);
}

/* Transform: ScaleX(0.5) */
.scalex-example {
    width: 100px;
    height: 100px;
    background-color: lightgreen;
    transform: scaleX(0.5);
}

/* Transform: Rotate(45deg) */
.rotate-example {
    width: 100px;
    height: 100px;
    background-color: lightcoral;
    transform: rotate(45deg);
}

/* Transform: SkewX(-25deg) */
.skewx-example {
    width: 100px;
    height: 100px;
    background-color: lightgoldenrodyellow;
    transform: skewX(-25deg);
}

/* Transform: Skew(25deg, 5deg) */
.skew-example {
    width: 100px;
    height: 100px;
    background-color: lightpink;
    transform: skew(25deg, 5deg);
}

/* Transform: Translate(50px, 52px) */
.translate-example {
    width: 100px;
    height: 100px;
    background-color: lightskyblue;
    transform: translate(50px, 52px);
}

/* Transform: Matrix(0.7, -0.5, 0.5, 0.4, 0.5, 0.7) */
.matrix-example {
    width: 100px;
    height: 100px;
    background-color: lightseagreen;
    transform: matrix(0.7, -0.5, 0.5, 0.4, 0.5, 0.7);
}
```

analisis
Analisis
Transform: Scale(0.5):

transform: scale(0.5);
Properti ini mengubah ukuran elemen menjadi setengah dari ukuran aslinya, baik dalam arah horizontal maupun vertikal.
Contoh: Elemen dengan kelas .scale-example akan memiliki ukuran 50% dari ukuran aslinya.

Transform: ScaleX(0.5):

transform: scaleX(0.5);
Properti ini mengubah ukuran elemen hanya dalam arah horizontal (sumbu X) menjadi setengah dari ukuran aslinya.
Contoh: Elemen dengan kelas .scalex-example akan memiliki lebar 50% dari lebar aslinya, tetapi tingginya tetap sama.

Transform: Rotate(45deg):

transform: rotate(45deg);
Properti ini memutar elemen sebesar 45 derajat searah jarum jam dari posisi awalnya.
Contoh: Elemen dengan kelas .rotate-example akan diputar sebesar 45 derajat.

Transform: SkewX(-25deg):

transform: skewX(-25deg);
Properti ini memiringkan elemen sepanjang sumbu X (horizontal) sebesar -25 derajat (miring ke kiri).
Contoh: Elemen dengan kelas .skewx-example akan miring ke kiri sebesar 25 derajat.

Transform: Skew(25deg, 5deg):

transform: skew(25deg, 5deg);
Properti ini memiringkan elemen sepanjang sumbu X (horizontal) sebesar 25 derajat dan sepanjang sumbu Y (vertikal) sebesar 5 derajat.
Contoh: Elemen dengan kelas .skew-example akan miring sebesar 25 derajat ke kanan dan 5 derajat ke bawah.

Transform: Translate(50px, 52px):

transform: translate(50px, 52px);
Properti ini menggeser (menerjemahkan) elemen sejauh 50 piksel ke kanan dan 52 piksel ke bawah dari posisi awalnya.
Contoh: Elemen dengan kelas .translate-example akan digeser ke kanan sejauh 50 piksel dan ke bawah sejauh 52 piksel.

Transform: Matrix(0.7, -0.5, 0.5, 0.4, 0.5, 0.7):

transform: matrix(0.7, -0.5, 0.5, 0.4, 0.5, 0.7);
Properti ini menggunakan nilai matriks untuk melakukan transformasi yang kompleks, termasuk skala, rotasi, dan translasi.
Contoh: Elemen dengan kelas .matrix-example akan mengalami transformasi sesuai dengan matriks yang diberikan.

Setiap transformasi memberikan kemampuan untuk mengubah posisi, bentuk, dan orientasi elemen dengan cara yang sangat fleksibel. Transformasi ini dapat meningkatkan pengalaman pengguna dengan menambahkan animasi dan interaktivitas pada elemen-elemen dalam halaman web.
# flex container

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Flexbox Properties Example</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <h1>Flexbox Properties Example</h1>

    <div class="flex-container">
        <div class="item">1</div>
        <div class="item">2</div>
        <div class="item">3</div>
        <div class="item">4</div>
    </div>
</body>
</html>
```

```css
/* Flex Container */
.flex-container {
    display: flex;
    background-color: lightgray;
    height: 200px;
    width: 80%;
    margin: 20px auto;
    border: 1px solid darkgray;

    /* Flex Direction */
    flex-direction: row; /* default value */

    /* Justify Content */
    justify-content: space-between;

    /* Align Items */
    align-items: center;
}

/* Flex Items */
.item {
    background-color: lightblue;
    width: 50px;
    height: 50px;
    margin: 10px;
    display: flex;
    justify-content: center;
    align-items: center;
}
```

Analisis
Display: flex:

display: flex;
Properti ini mengubah elemen induk (container) menjadi flex container, yang memungkinkan penggunaan fleksibilitas dari CSS Flexbox. Elemen di dalam flex container dapat diatur ulang untuk menanggapi ukuran layar dan kebutuhan desain yang berbeda.

Flex Direction:

flex-direction: row;
Properti ini mengatur arah tata letak elemen-elemen anak (items) di dalam flex container. Nilai defaultnya adalah row, yang berarti elemen anak akan tersusun secara horizontal dari kiri ke kanan.
Contoh: Elemen .flex-container memiliki flex-direction: row;, sehingga elemen anaknya (.item) tersusun secara horizontal.

Justify Content:

justify-content: space-between;
Properti ini mengatur cara menempatkan elemen anak di dalam flex container sepanjang sumbu utama (sesuai dengan flex-direction). Nilai space-between akan membuat ruang kosong di antara elemen-elemen anak, sehingga elemen anak berada di ujung kiri dan kanan container.
Contoh: Elemen .flex-container memiliki justify-content: space-between;, sehingga elemen anaknya (.item) ditempatkan dengan jarak yang sama di antara mereka di dalam container.

Align Items:

align-items: center;
Properti ini mengatur cara menempatkan elemen anak di dalam flex container sepanjang sumbu lintang (berlawanan dengan flex-direction). Nilai center akan membuat elemen anak berada di tengah-tengah container secara vertikal.
Contoh: Elemen .flex-container memiliki align-items: center;, sehingga elemen anaknya (.item) ditempatkan di tengah-tengah container secara vertikal.
Flexbox adalah teknik tata letak yang kuat dalam CSS untuk mengatur tata letak elemen-elemen dalam sebuah kontainer secara fleksibel. 

Dengan menggunakan properti seperti flex-direction, justify-content, dan align-items, Anda dapat dengan mudah mengatur tata letak elemen dan menyesuaikannya dengan desain yang diinginkan, baik untuk responsif web atau aplikasi.

# position

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Position Properties Example</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <h1>Position Properties Example</h1>

    <div class="relative-example">
        <p>Relative Position</p>
    </div>

    <div class="absolute-example">
        <p>Absolute Position</p>
    </div>

    <div class="fixed-example">
        <p>Fixed Position</p>
    </div>

    <div class="sticky-example">
        <p>Sticky Position</p>
    </div>
</body>
</html>
```

```css
/* Base Styles */
body {
    font-family: Arial, sans-serif;
    margin: 20px;
    padding: 0;
}

/* Relative Position */
.relative-example {
    position: relative;
    background-color: lightblue;
    width: 200px;
    height: 100px;
    margin-bottom: 20px;
}

/* Absolute Position */
.absolute-example {
    position: absolute;
    background-color: lightgreen;
    width: 200px;
    height: 100px;
    top: 50px;
    left: 50px;
}

/* Fixed Position */
.fixed-example {
    position: fixed;
    background-color: lightcoral;
    width: 200px;
    height: 100px;
    top: 20px;
    right: 20px;
}

/* Sticky Position */
.sticky-example {
    position: sticky;
    background-color: lightskyblue;
    width: 200px;
    height: 100px;
    top: 20px;
    margin-top: 20px;
}
```

analisis
Analisis
Position: Relative:

position: relative;
Elemen tetap berada dalam aliran dokumen normal, tetapi pengaturan properti top, right, bottom, atau left akan memindahkan elemen relatif terhadap posisi normalnya.
Contoh: Elemen dengan kelas .relative-example memiliki position: relative;, sehingga perubahan pada properti top, right, bottom, atau left akan memindahkan elemen relatif terhadap posisi normalnya.
Position: Absolute:

position: absolute;
Elemen dihapus dari aliran dokumen normal dan ditempatkan relatif terhadap elemen yang terdeklarasi sebagai relatif atau viewport. Ini berarti elemen tersebut dapat ditempatkan di lokasi tertentu di halaman web.
Contoh: Elemen dengan kelas .absolute-example memiliki position: absolute;, sehingga properti top, right, bottom, atau left menempatkan elemen ini di lokasi yang spesifik di dalam viewport atau dalam elemen induk yang memiliki posisi relatif.
Position: Fixed:

position: fixed;
Elemen ini ditempatkan relatif terhadap viewport, yang berarti elemen tersebut tetap berada di posisi yang sama di layar saat pengguna menggulir halaman.
Contoh: Elemen dengan kelas .fixed-example memiliki position: fixed;, sehingga elemen ini akan tetap di tempatnya di layar saat pengguna menggulir halaman.
Position: Sticky:

position: sticky;
Elemen ini berperilaku seperti relative sampai mereka melewati ambang batas tertentu, setelah itu elemen tersebut akan 'melekat' di tempatnya relatif terhadap viewport.
Contoh: Elemen dengan kelas .sticky-example memiliki position: sticky;, dan pada contoh di atas, ketika pengguna menggulir halaman, elemen tersebut akan 'melekat' di bagian atas viewport sampai konten berikutnya melewati elemen tersebut.
Analisis Singkat:

Relative: Menggeser elemen relatif terhadap posisi normalnya dalam aliran dokumen.

Absolute: Membuat elemen dihapus dari aliran dokumen normal dan memposisikannya relatif terhadap viewport atau elemen induk yang memiliki posisi relatif.

Fixed: Membuat elemen tetap terlihat di lokasi yang sama di layar saat pengguna menggulir halaman.

Sticky: Memungkinkan elemen untuk tetap di tempatnya sampai mencapai batas tertentu di mana ia 'melekat' dan berhenti menggulir bersama dengan halaman.

Setiap properti position memiliki kegunaan dan keunggulan tertentu tergantung pada kebutuhan desain dan interaksi pengguna yang diinginkan. Dengan memahami perbedaan dan penggunaan properti ini, Anda dapat mengontrol tata letak dan interaksi elemen di halaman web secara efektif.
