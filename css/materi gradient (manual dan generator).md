# kelas Xl RPL 1
anggota :
Jordan
Rayhan juli saputra

## pengertian gradient
Gradient CSS adalah teknik yang digunakan untuk membuat latar belakang bergradasi atau beralih secara mulus dari satu warna ke warna lainnya. Ini memungkinkan desainer web untuk membuat efek visual menarik dan dinamis pada elemen HTML seperti latar belakang elemen, teks, atau border.

## kegunaan gradient pada web
Gradient adalah perpaduan transisi warna yang digunakan pada desain web untuk menciptakan efek visual yang menarik dan estetis. Beberapa kegunaan utama dari gradient pada web adalah:

1. Mempercantik Desain: Gradients digunakan untuk meningkatkan tampilan visual elemen-elemen seperti latar belakang, tombol, dan elemen dekoratif lainnya, sehingga membuat desain web lebih menarik dan modern.

2. Memperbaiki Keterbacaan: Dengan menggunakan gradient pada teks atau latar belakang, Anda dapat meningkatkan kontras antara teks dan latar belakangnya, sehingga meningkatkan keterbacaan konten.

3. Membuat Efek Tiga Dimensi: Gradient sering digunakan untuk menciptakan efek tiga dimensi pada elemen-elemen seperti tombol, kotak, atau gambar, yang membuat tampilan lebih hidup dan realistis.

4. Membuat Fokus: Gradients dapat digunakan untuk mengarahkan perhatian pengguna ke suatu bagian tertentu pada halaman web, misalnya, dengan menggunakan gradient yang lebih terang di area fokus.

5. Branding: Gradients dapat menjadi bagian dari identitas visual suatu merek atau situs web, sehingga membantu memperkuat citra merek dan menciptakan konsistensi visual.

6. Peningkatan Responsif: Gradients dapat disesuaikan secara responsif untuk beradaptasi dengan berbagai ukuran layar dan perangkat, sehingga tetap terlihat baik tanpa mengorbankan performa desain.

Dengan berbagai kegunaan ini, gradient telah menjadi salah satu elemen desain yang sangat populer dalam pengembangan web modern.

## jenis-jenis gradient css
Ada dua jenis utama gradient CSS: linear gradient dan radial gradient.

1. Linear Gradient:
- Linear gradient digunakan untuk membuat gradasi linier dari satu warna ke warna lainnya sepanjang sebuah garis.
-  Properti utama yang digunakan adalah background-image dengan nilai linear-gradient.
   Contoh kode CSS untuk linear gradient
   ```css
   linear-gradient(0deg, rgba(242,242,242,1) 0%, rgba(255,0,0,1) 100%);

```

hasil:
![img](aset/IMG20.jpg)
- Pada contoh di atas, gradient akan bergerak dari warna merah (red) ke putih (white) dari atas ke bawah.

2. Radial Gradient:
- Radial gradient digunakan untuk membuat gradasi berbentuk radial (bulat) dari satu warna ke warna lainnya.
- Properti yang digunakan mirip dengan linear gradient, menggunakan background-image dengan nilai radial-gradient.
- ​Contoh kode CSS untuk radial gradient
   ```css
   radial-gradient(circle, rgba(252,0,0,1) 0%, rgba(255,255,255,1) 100%);
```

hasil:
![img](aset/IMG13.jpg)- Pada contoh ini, gradient akan memiliki bentuk lingkaran (circle) dengan gradasi dari warna merah (red) ke putih(white) dari dalam ke luar.
- Selain itu, dalam CSS gradient, Anda juga dapat mengatur arah, titik awal dan akhir (pada linear gradient), dan bentuk (pada radial gradient) sesuai kebutuhan desain Anda. Gradient CSS adalah salah satu cara yang populer digunakan untuk memberikan tampilan modern dan kreatif pada halaman web.
## Penjelasan gradient manual:
Gradient manual adalah proses menciptakan gradient secara langsung dengan menentukan warna dan lokasi tertentu dari warna-warna tersebut.Anda dapat mengubah warna atau arah gradiennya dengan mengedit nilai-nilai pada properti `background` di file `styles.css`.
contoh program:
```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Gradient Box</title>
<link rel="stylesheet" href="styles.css">
</head>
<body>
  <div class="gradient-box"></div>
</body>
</html>
```

<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Gradient Box</title>
<link rel="stylesheet" href="styles.css">
</head>
<body>
  <div class="gradient-box"></div>
</body>
</html>
```css
body {
  margin: 0;
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
}

.gradient-box {
  width: 200px;
  height: 200px;
  background: linear-gradient(to right, red, yellow);
  border-radius: 10px;
}

```

hasil:![img](aset/img18.jpg)
## cara pengunaan gradient generator 
 1. tekan ling ini https://cssgradient.io/
 2. setelah masuk pilih salah satu yang ada di bawah ini![img](aset/img14.jpg)
    jika memilih linier maka gradient akan bergerak dari atas ke bawah
    jika memilih radial maka gradient akan memiliki bentuk lingkaran 
3. jika sudah memilih maka atur lah warna di sini
![img](aset/img19.jpg)
4. setelah sudah memilih warna maka salin lah kode program di bawak ini lalu tempel di background program anda
    ![img](aset/img15.jpg)
