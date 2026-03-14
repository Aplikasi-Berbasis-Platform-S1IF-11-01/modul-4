<div align="center">
  <br />

  <h1>LAPORAN PRAKTIKUM <br>
  APLIKASI BERBASIS PLATFORM
  </h1>

  <br />

  <h3>MODUL V <br>
 BOOTSTRAP
  </h3>

  <br />

  <img src="Images/Logo Telkom.png" alt="Logo" width="300">

  <br />
  <br />
  <br />

  <h3>Disusun Oleh :</h3>

  <p>
    <strong>Andreas Besar Wibowo</strong><br>
    <strong>2311102198</strong><br>
    <strong>S1 IF-11-REG01</strong>
  </p>

  <br />

  <h3>Dosen Pengampu :</h3>

  <p>
    <strong>Dimas Fanny Hebrasianto Permadi, S.ST., M.Kom</strong>
  </p>
  
  <br />
    <h4>Asisten Praktikum :</h4>
    <strong>Apri Pandu Wicaksono </strong> <br>
    <strong>Rangga Pradarrell Fathi</strong>
  <br />

  <h3>LABORATORIUM HIGH PERFORMANCE
 <br>FAKULTAS INFORMATIKA <br>UNIVERSITAS TELKOM PURWOKERTO <br>2026</h3>
</div>

<hr>

## Dasar Teori

### Pengenalan Bootstrap
Bootstrap merupakan sebuah front-end framework gratis untuk pengembangan antar muka web yang lebih cepat dan lebih mudah. Dikembangkan oleh Mark Otto dan Jacom Thornton di Twitter dan dirilis sebagai produk open source pada Agustus 2011 di GitHub. Bootstrap mencakup template desain berbasis HTML dan CSS untuk tipografi, form, button, navigasi, modal, image carousells dan masih banyak lagi, serta terdapat opsional plugin JavaScript. Selain itu, Bootstrap memiliki kemampuan untuk membuat desain responsif yang secara otomatis menyesuaikan diri agar terlihat baik di segala perangkat, mulai dari perangkat ponsel hingga desktop pc.

#### 1. Pemasangan Bootstrap
Bootstrap merupakan produk yang mengusung konsep open source sehingga untuk pemasangannya dapat dilakukan dengan beberapa cara sebagai berikut:
- Unduh di http://getbootstrap.com, selanjutnya pasang pada project web kalian seperti memanggilExternal Style Sheet pada CSS.
- Memanggil Bootstrap CDN (Content Delivery Network), sehingga kita tidak perlu mengunduh dan memasangnya pada laman website, hanya memanggil source dari Bootstrap. Cara ini membutuhkan koneksi internet untuk menghasilkan perubahan tampilan CSS.
```html
<!-- Pemanggilan Bootstrap dengan CDN -->

<!-- CSS -->
<link 
    href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css"
    rel="stylesheet" 
    integrity="sha384-9ndCyUaIbzAi2FUVXJi0CjmCapSmO7SnpJef0486qhLnuZ2cdeRhO02iuK6FUUVM"
    crossorigin="anonymous"
>

<!-- jQuery library -->
<script 
    src="https://code.jquery.com/jquery-3.7.0.min.js" 
    integrity="sha256-2Pmvv0kuTBOenSvLm6bvfBSSHrUJ+3A7x6P5Ebd07/g=" 
    crossorigin="anonymous"
></script>

<!-- JavaScript -->
<script 
    src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"
    integrity="sha384-geWF76RCwLtnZ8qwWowPQNguL3RmwHVBC9FhGdlKrxdiJJigb/j/68SIy3Te4Bkz"
    crossorigin="anonymous"
></script>
```
### Bootstrap Container
Bootstrap container adalah elemen paling dasar yang dibutuhkan dalam layouting menggunakan Bootstrap Grid. Container berbentuk class CSS yang sisipkan pada elemen HTML `<div>`.
- Class `.container` menyediakan container yang responsive dengan lebar yang tetap.
- Class `.container-fluid` menyediakan container dengan lebar yang penuh mencakup seluruh area pandang.

### Bootstrap Grid

Sistem grid pada Bootstrap menggunakan rangkaian container, rows dan column untuk tata letak dan keselarasan elemen atau konten. Dibangun dengan flexbox dan sangat responsif terhadap perangkat yang digunakan untuk menampilkan laman web. Struktur dasar grid pada Bootstrap sebagai berikut.
```html
<div class="row">
    <div class="col-*-#"></div>
    <div class="col-*-#"></div>
</div>
<div class="row">
    <div class="col-*-#"></div>
    <div class="col-*-#"></div>
    <div class="col-*-#"></div>
</div>
```
Pertama diawali dengan `<div class=”container”>`. Kemudian buat sebuah baris sebelum mendeklarasikan sebuah kolom dengan menggunakan `<div class=”row”>`. Terakhir buat elemen div dengan mendefinisikan class “col-*-#”. Tanda * dan # mewakili jenis dan ukuran column yang akan digunakan.

Contoh penerapannya sebagai berikut:
```css
<div class="container">
    <div class="row">
        <div class="col-12 col-md-8">.col-12 .col-md-8</div>
        <div class="col-6 col-md-4">.col-6 .col-md-4</div>
    </div>

    <div class="row">
        <div class="col-6 col-md-4">.col-6 .col-md-4</div>
        <div class="col-6 col-md-4">.col-6 .col-md-4</div>
        <div class="col-6 col-md-4">.col-6 .col-md-4</div>
    </div>

    <div class="row">
        <div class="col-6">.col-6</div>
        <div class="col-6">.col-6</div>
    </div>
</div>
```

### Text Style
Bootstrap menyediakan banyak class untuk mengatur style sebuah teks elemen HTML. Beberapa contohnya yaitu mulai dari `.text-left` sampai `.h1 s.d .h6`

### Bootstrap Table, Image & Button
Bootstrap menyediakan class untuk pengaturan style elemen tabel, gambar dan tombol menjadi lebih menarik.
- Bootstrap Table, Tabel pada Bootstrap dipanggil dengan class .table secara default, namun ada beberapa class tambahan yang dapat didefinisikan pada elemen tabel yang lain.
Contoh penerapannya sebagai berikut:
```html
<!-- Tabel Hover Style -->
<table class="table table-hover">
    <thead>
        <tr>
            <th scope="col">#</th>
            <th scope="col">Nama Lengkap</th>
            <th scope="col">Asal Kota</th>
            <th scope="col">Umur</th>
        </tr>
    </thead>

    <tbody>
        <tr>
            <th scope="row">1</th>
            <td>Budi Rojadi</td>
            <td>Semarang</td>
            <td>35 th</td>
        </tr>

        <tr>
            <th scope="row">2</th>
            <td>Yulia Santi</td>
            <td>Bekasi</td>
            <td>32</td>
        </tr>

        <tr>
            <th scope="row">3</th>
            <td>Fahri Abdilah</td>
            <td>Medan</td>
            <td>38 th</td>
        </tr>
    </tbody>
</table>
```

- Bootstrap Image, Bootstrap dapat menangani desain gambar agar responsif pada setiap perangkat yang menampilkan laman web. Dengan menambahkan class .img-fluid pada elemen tag `<img>` pada HTML maka gambar yang didefinisikan pada laman web akan memiliki ukuran yang responsif menyesuaikan ukuran layar perangkat. Class tersebut mengatur ukuran gambar dengan menyesuaikan ukuran dari parent element sebagai wadah atau container elemen gambar. Terdapat class .thumbnail yang berguna menjadikan gambar menjadi berukuran kecil dan sedikit memiliki border disekitarnya.
```html
<div class="container">
    <h2>Thumbnail & Fluid</h2>
    <img src="cinqueterre.jpg" class="img-thumbnail" alt="Cinque Terre">
    <img src="cinqueterre.jpg" class="img-fluid" alt="Responsive image">
</div>
```

- Bootstrap Button, Tampilan button pada elemen HTML dapat dirubah dengan menambahkan beberapa class untuk button oleh Bootstrap. Bootstrap membuat tampilan button menjadi lebih menarik dan memberikan user experience yang baik. Class yang digunakan secara default adalah `.btn` namun dengan disertai class lain.
Contoh penerapan class button:
```html
<div class="container">
    <h4>Button Styles</h4>
    <button type="button" class="btn btn-secondary">Secondary</button>
    <button type="button" class="btn btn-primary btn-lg">Primary</button>
    <button type="button" class="btn btn-success w-100">Success</button>
    <button type="button" class="btn btn-info btn-sm">Info</button>
    <button type="button" class="btn btn-warning">Warning</button>
    <button type="button" class="btn btn-danger">Danger</button>
    <button type="button" class="btn btn-link">Link</button>
</div>
```

### Bootstrap Form
Bootstrap menyediakan perubahan elemen form pada HTML baik pada segi tata letak tampilan atau tampilan antarmuka elemen-elemen dalam form. Class .form-control digunakan untuk sebagian besar elemen input dalam tag `<form>` untuk memberikan styling yang konsisten. Ada beberapa cara untuk mengatur tata letak tampilan form di Bootstrap:
- Vertical Form (Default): Ini merupakan tampilan default saat tag form tidak didefinisikan class khusus. Setiap elemen form akan ditampilkan secara vertikal.
- Inline Form: Untuk membuat form inline di Bootstrap, Anda dapat menggunakan utility classes tertentu pada container form. Ini akan membuat elemen-elemen form berada dalam satu baris.
- Horizontal Form: Untuk membuat form horizontal di Bootstrap, Anda dapat menggunakan sistem grid Bootstrap. Gunakan class .row pada container dan .col-* untuk mengatur lebar kolom label dan input.
```html
<div class="container">
    <h3>Horizontal form</h3>
    <form action="/action_page.php">
        <div class="row mb-3">
            <label for="uname" class="col-sm-2"></label>
            <input type="text" class="form-control" id="uname" placeholder="Enter username" name="uname">
        </div>

        <div class="row mb-3">
            <label for="pwd" class="col-sm-2 col-form-label">Password:</label>
            <div class="col-sm-10">
                <input type="password" class="form-control" id="pwd" placeholder="Enter password" name="pwd">
            </div>
        </div>

        <div class="row">
            <div class="col-sm-10 offset-sm-2">
                <button type="submit" class="btn btn-success">Submit</button>
            </div>
        </div>
    </form>
</div>
```

## Tugas
### Buat halaman ramadan dan gunakan bootstrap (sebisa mungkin tanpa meggunakan native css full bootstap)
```html
<!-- Andreas Besar Wibowo -->
<!-- 2311102198 / IF - 11 - 01 -->

<!DOCTYPE html>
<html>

<head>
    <title>Ramadhan</title>

    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet">

</head>

<body class="bg-dark text-light">

    <!-- Navigatiom Bar -->
    <nav class="navbar navbar-dark bg-success">
        <span class="navbar-brand ms-3">Ramadhan</span>
    </nav>

    <div class="container text-center mt-5">

        <div class="d-flex justify-content-between align-items-center">

            <img src="Images/ketupat.png" width="120">

            <div>
                <h1 class="display-4 text-warning">Ramadhan</h1>
                <p class="lead">Selamat Menunaikan Ibadah Puasa</p>
            </div>

            <img src="Images/ketupat.png" width="120">

        </div>

        <div class="row justify-content-center mt-4">

            <div class="col-md-6">

                <div class="card shadow">

                    <div class="card-body">

                        <h3 class="text-success">Selamat Berpuasa</h3>

                        <p>
                            Semoga di bulan suci Ramadhan ini kita diberikan
                            kesehatan, keberkahan, dan kelancaran dalam
                            menjalankan ibadah puasa.
                        </p>


                    </div>

                </div>

            </div>

        </div>

    </div>

</body>

</html>
```
### Hasil
![Ouput 1](Images/Ouput%20Ramadhan%201.png)

Gambar diatas merupakan halaman website sederhana yang bertema Ramadhan. Halaman ini diberi sedikit dekorasi yaitu ketupat dan menampilkan pesan untuk dibulan suci Ramadhan.