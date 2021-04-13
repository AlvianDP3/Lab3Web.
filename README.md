# Pemrograman Web

```
ALVIAN DWI PRAMONO
TI.19.C1
```
# Ordered List
Digunakan untuk membuat daftar dimana tiap bagiannya ditandai dengan sebuah simbol. Ordered
list dibuat dengan tag <ol>. Lalu di dalamnya diisi dengan item-item yang akan dimasukkan ke
dalam list. Item dibuat dengan tag <li> (list item).
Contoh Ordered List

Secara default ordered list akan diurutkan berdasarkan angka 1,2,3,...dst. Angka tersebut dapat
diubah sesuai dengan kebutuhan, misalnya ingin menampilkan urutan berdasarkan angka romawi
atau huruf abjad seperti a,b,c,...dst. Untuk merubah jenis tampilan list tersebut dengan
menambahkan atribut type pada tag ol dan berikan nilainya sesuai dengan yang diinginkan.
• a untuk alfabet a, b, c, dan seterusnya;
• A untuk alfabet A, B, C, dan seterusnya;
• i untuk angka romwari i, ii, iii, dan seterusnya;
• I untuk angka romwari I, II, III, dan seterusnya.
Dan untuk mengatur awal dari penomoran menggunakan atribut start dengan nilai disesuaikan
dengan jenis dan bermulanya.

```
<ul>
<li>Jaringan Komputer</li>
<li>Sistem Multimedia</li>
<li>Basis Data</li>
<li>Sistem Operasi</li>
</ul>
```

Dan untuk mengatur awal dari penomoran menggunakan atribut start dengan nilai disesuaikan
dengan jenis dan bermulanya.

```
<ul>
<li>Jaringan Komputer</li>
<li>Sistem Multimedia</li>
<li>Basis Data</li>
<li>Sistem Operasi</li>
</ul>

<ol type="A" start="D">
<li>Pemrograman Web</li>
<li>Sistem Informasi</li>
<li>Rekayasa Perangkat Lunak</li>
</ol>
```

# ordered List
Digunakan untuk membuat daftar dimana tiap bagiannya memiliki nomor secara terurut.
Unordered list dibuat dengan tag <ul> dan untuk item-nya dibuat juga dengan tag <li>.
Contoh Unordered List

Secara default simbol yang digunakan oleh unordered list adalah lingkaran kecil (disc). Simbol
tersebut dapat diubah sesuai dengan kebutuhannya, seperti kotak, lingkaran, atau tanpa simbol.
Untuk mengubahnya dengan menambahkan atribut type pada tag ul dan berikan nilainya sesuai
dengan yang diinginkan.
• square untuk simbol persegi;
• disc (default) untuk simbol lingkaran disc;
• none tidak memakai simbol;
• circle untuk simbol lingkaran;
Selain menggunakan atribut type, dapat juga diubah dengan nilai lainnya menggunakan gambar
atau icon. Untuk merubahnya menggunakan CSS dengan property list-style-image.

# scription List
Digunakan untuk membuat daftar dimana tiap daftar tersebut memiliki penjelasan (sub-bagian).
Ada tiga tag yang digunakan untuk membuat description list, yaitu:
• <dl> (description list) tag untuk memulai description list;
• <dt> (description term) tag untuk membuat kata yang akan dideskripsikan;
• <dd> (description description) tag untuk membuat penjelasan dari kata.



# Contoh Description List

Nested List (List didalam list)
List dapat ditulis didalam list lainnya, atau sub bagian dari list yang lain. Contoh penggunaannya
seperti berikut.

```
<ul>
<li>Pemrograman Web</li>
<li>Sistem Informasi</li>
<li>Rekayasa Perangkat Lunak</li>
</ul>
```

# Nested List (List didalam list)
List dapat ditulis didalam list lainnya, atau sub bagian dari list yang lain. Contoh penggunaannya
seperti berikut.

```
<ul>
<li>Makanan
<ol>
<li>Nasi Padang</li>
<li>Ayam Bakar</li>
</ol>
</li>
<li>Minuman
<ol>
<li>Jus Mangga</li>
<li>Es Teh</li>
</ol>
</li>
</ul>
```

# Contoh Pembuatan Tabel.

```
<table boder="1">
<tr>
<td>Baris 1 kolom 1</td>
<td>baris 1 kolom 2</td>
</tr>
<tr>
<td>Baris 2 kolom 1</td>
<td>baris 2 kolom 2</td>
</tr>
</table>
```
# Menggabungkan Sel Data
Sel data pada tabel dapat digambugkan untuk keperluan tertentu. Untuk menggabungkan sel secara
vertikal menggunakan atribut rowspan dan untuk menggabungkan sel secara horizontal
menggunakan atribut colspan. Atribut tersebut dapat ditambahkan pada tag td (tabel data) dengan
nilai atributnya adalah jumlah sel yang akan digabungkan.

# vertikal menggunakan atribut rowspan dan untuk menggabungkan sel secara horizontal

```
<table border="1">
<tr>
<td colspan="2">Baris 1 kolom 1</td>
</tr>
<tr>
<td>Baris 2 kolom 1</td>
<td>baris 2 kolom 2</td>
</tr>
<tr>
<td>Baris 3 kolom 1</td>
<td>baris 3 kolom 2</td>
</tr>
<tr>
<td rowspan="2">Baris 4 kolom 1</td>
<td>baris 4 kolom 2</td>
</tr>
<tr>
<td>baris 5 kolom 2</td>
</tr>
</table>
```

# form
Web tidak hanya berfungsi untuk menampilkan informasi, namun dapat juga menerima data dari
pengunjungnya. Salah satu cara untuk mengambil data dari pengunjung adalah dengan
menggunakan form. Form pada web berlaku sama halnya dengan formulir di dunia nyata. Form
dapat diisi kemudian diproses dengan program tertentu, baik dari sisi server ataupun dari sisi
client.
Untuk membuat form digunakan tag <form> dengan atribut action dan method. Atribut action
untuk menentukan aksi yang akan digunakan pada saat form dikirim. Dan method adalah untuk
menentukan metode yang digunakan dalam mengirimkan data.

• Atribut action dapat diisi dengan url endpoint yang akan memproses data.
• Atribut enctype: Mendefinsikan cara encoding data sebelum dikirimkan. Biasanya digunakan
jika ingin meng-upload file.
• Atribut method: Metode pengiriman data.
o GET: Data dikirimkan bersama URL.
o POST: Data dikirimkan terpisah dari URL.
Elemen atau field pada form dapat dibuat dengan tag berikut.
Element Keterangan

```
<input type="text"> Displays a single-line text input field
<input type="radio"> Displays a radio button (for selecting one of many choices)
<input type="checkbox"> Displays a checkbox (for selecting zero or more of many choices)
<input type="submit"> Displays a submit button (for submitting the form)
<select> Defines a drop-down list
<textarea> Defines a multi-line input field (a text area)
```
  
  
## Contoh pembuatan form login

```
<form action="proses.php" method="post">
<!--deklarasi field form disini-->
</form>
```

![1](https://user-images.githubusercontent.com/56244029/114507819-dd158a00-9c5d-11eb-9a4a-d70cbe5c5f33.jpg)

Setiap elemen atau field form harus memiliki atribut name. Atribut name merupakan nama dari
field yang akan menjadi kunci dan variabel di dalam program. Sedangkan atribut id, sifatnya
opsional.

```
Instruksi Praktikum
1. Persiapkan text editor misalnya VSCode.
2. Buat folder baru dengan nama Lab3Web
3. Ikuti langkah-langkah praktikum yang akan dijelaskan berikutnya.
4. Lakukan validasi dokumen html dengan mengakses http://validator.w3.org
```

 # Langkah-langkah Praktikumkah Praktikum
Persiapan membuat dokumen HTML dengan nama file lab3web/html seperti berikut.

```
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>HTML Lanjutan</title>
</head>
<body>
<header>
<h1>Membuat List</h1>
</header>
</body>
</html>
```

# Membuat Ordered List
Kemudian tambahkan kode untuk membuat Ordered List seperti berikut.

```
<section id="order-list">
<h2>Ordered List</h2>
<ol>
<li>Pemrograman Web</li>
<li>Sistem Informasi</li>
<li>Basis Data 2</li>
</ol>
</section>
```

![2](https://user-images.githubusercontent.com/56244029/114508464-94aa9c00-9c5e-11eb-8fc4-99912ba49c8e.jpg)

# Membuat Unorderd List
Kemudian tambakan kode untuk membuat Unordered List, setelah deklarasi ordered list pada
section unordered-list, seperti berikut.

```
<section id="unorder-list">
<h2>Unordered List</h2>
<ul type="square">
<li>Jaringan Komputer</li>
<li>Struktur Data</li>
<li>Algoritma &amp; Pemrograman</li>
</ul>
</section>
```

![4](https://user-images.githubusercontent.com/56244029/114508777-f4a14280-9c5e-11eb-8fe5-d1d92ee11dc8.jpg)

# Membuat Description List
Kemudian tambahkan kode untuk membuat description list setelah deklarasi unorderd-list.

```
<section id="unorder-list">
<h2>Description List</h2>
<dl>
<dt>Fakultas Teknik</dt>
<dd>Teknik Industri</dd>
<dd>Teknik Informatika</dd>
<dd>Teknik Lingkungan</dd>
<dt>Fakultas Ekonomi dan Bisnis</dt>
<dd>Akuntansi</dd>
<dd>Manajemen</dd>
<dd>Bisnis Digital</dd>
</dl>
</section>
```

![5](https://user-images.githubusercontent.com/56244029/114509010-3d58fb80-9c5f-11eb-9cd4-a3eec1eb298c.jpg)

# Membuat Tabel
Buat file baru dengan nama lab3_tabel.html seperti berikut.

```
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>HTML Lanjutan</title>
</head>
<body>
<header>
<h1>Membuat Table</h1>
</header>
</body>
</html>
```
Kemudian selanjutnya tambahkan kode untuk membuat tabel sederhana seperti berikut:

```
<table border="1" cellpadding="4" cellspacing="0">
<thead>
<tr>
<th>No.</th>
<th>Fakultas</th>
<th>Program Studi</th>
</tr>
</thead>
<tbody>
<tr>
<td>1.</td>
<td>Teknik</td>
<td>Teknik Informatika</td>
</tr>
<tr>
<td>2.</td>
<td>Teknik</td>
<td>Teknik Industri</td>
</tr>
<tr>
<td>3.</td>
<td>Teknik</td>
<td>Teknik Lingkungan</td>
</tr>
</tbody>
</table>
```

![6](https://user-images.githubusercontent.com/56244029/114509488-bfe1bb00-9c5f-11eb-97dd-e14fa245cdc2.png)

# Mengatur Margin dan Padding
Untuk mengatur margin dan padding pada cel data, tambahkan atribut cellpadding dan
cellspacing pada tag table.
```
<table border="1" cellpadding="4" cellspacing="0">
```

![7](https://user-images.githubusercontent.com/56244029/114509688-020afc80-9c60-11eb-8873-463b89dc73f0.jpg)

# Menggabungkan Sel Data
Untuk menggabungkan sel data, gunakan atribut rowspan dan colspan. Atribut rowspan untuk
menggabungkan baris (secara vertikal) dan colspan untuk menggabungkan kolom (secara
horizontal).
```
<table border="1" cellpadding="6" cellspacing="0">
<thead>
<tr>
<th>No.</th>
<th>Fakultas</th>
<th>Program Studi</th>
</tr>
</thead>
<tbody>
<tr>
<td>1.</td>
<td rowspan="3">Teknik</td>
<td>Teknik Informatika</td>
</tr>
<tr>
<td>2.</td>
<td>Teknik Industri</td>
</tr>
<tr>
<td>3.</td>
<td>Teknik Lingkungan</td>
</tr>
</tbody>
</table>
```

![8](https://user-images.githubusercontent.com/56244029/114510014-5f9f4900-9c60-11eb-83a4-b5971ff58ef7.jpg)

# Membuat Form
Buat file baru dengan nama lab3web.html seperti berikut
```
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>HTML Lanjutan</title>
</head>
<body>
<header>
<h1>Membuat Form</h1>
</header>
</body>
</html>
```
Kemudian selanjutnya tambahkan kode untuk membuat tabel sederhana seperti berikut:
```
<form action="proses.php" method="post">
<fieldset>
<legend>Data Pelanggan</legend>
<p>
<label for="nama">Nama</label>
<input type="text" id="nama" name="nama">
</p>
<p>
<label for="alamat">Alamat</label>
<textarea id="alamat" name="alamat" cols="20" rows="3"></textarea>
</p>
<p>
<label>Jenis Kelamin</label>
<input id="jk_l" type="radio" name="kelamin" value="L" /><label
for="jk_l">Laki-laki</label>
<input id="jk_p" type="radio" name="kelamin" value="P" /><label
for="jk_p">Perempuan</label>
</p>
<p><input type="submit" value="Login"></p>
</fieldset>
</form>
```

![9](https://user-images.githubusercontent.com/56244029/114510383-d2102900-9c60-11eb-81fc-d5cab489808f.jpg)

# Menabahkan Style pada Form
Agar tampilan form lebih menarik, bisa ditambahkan CSS seperti berikut.

```
<style>
form p > label {
display: inline-block;
width: 100px;
}
form input[type="text"], form textarea {
border: 1px solid #197a43;
}
form input[type="submit"] {
border: 1px solid #197a43;
background-color: #197a43;
color: #ffffff;
font-weight: bold;
padding: 5px 15px;
}
</style>
```

![10](https://user-images.githubusercontent.com/56244029/114510705-2ddab200-9c61-11eb-838f-7f2b809256ee.jpg)

# Pertanyaan dan Tugas
1. Buatlah form yang menampilkan dropdown menu dan listbox dengan multiple selection.

![11](https://user-images.githubusercontent.com/56244029/114511286-eacd0e80-9c61-11eb-975a-965de552127f.jpg)






















