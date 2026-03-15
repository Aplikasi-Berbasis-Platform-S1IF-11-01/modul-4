<div align="center">

# LAPORAN PRAKTIKUM
# APLIKASI BERBASIS PLATFORM

---

## MODUL 4
## HALAMAN RAMADAN DENGAN BOOTSTRAP

---

<img src="Logo_Telkom_University_potraitt.png" width="200">

---

**Disusun Oleh :**

**ANNISA AL JAUHAR**

**2311102014**

**S1 IF-11-REG01**

---

**Dosen Pengampu :**

Dimas Fanny Hebrasianto Permadi, S.ST., M.Kom

---

**PROGRAM STUDI S1 INFORMATIKA**

**FAKULTAS INFORMATIKA**

**UNIVERSITAS TELKOM PURWOKERTO**

**2025/2026**

</div>

---

## 1. Dasar Teori

Bootstrap merupakan framework CSS open-source yang paling banyak digunakan dalam pengembangan web. Bootstrap menyediakan berbagai komponen siap pakai seperti tombol, kartu, navigasi, modal, dan grid system yang memudahkan pembuatan tampilan website yang responsif dan konsisten di berbagai ukuran layar.

Bootstrap bekerja dengan cara menyediakan class-class CSS yang sudah didefinisikan sebelumnya. Developer cukup menambahkan class tersebut ke elemen HTML tanpa perlu menulis CSS dari awal. Bootstrap dapat digunakan dengan cara mengunduh filenya atau menggunakan CDN (Content Delivery Network) yang langsung di-link dari internet.

**Grid System** merupakan salah satu fitur utama Bootstrap yang menggunakan sistem 12 kolom untuk mengatur tata letak halaman. Dengan menggunakan class seperti `col-md-4`, elemen akan menempati 4 dari 12 kolom yang tersedia pada layar berukuran medium ke atas.

**Utility Classes** adalah class-class pembantu yang disediakan Bootstrap untuk mengatur tampilan elemen secara cepat tanpa menulis CSS. Beberapa utility classes yang digunakan pada praktikum ini antara lain:

- `bg-dark` dan `bg-secondary` untuk mengatur warna background
- `text-white`, `text-warning`, `text-light` untuk mengatur warna teks
- `d-flex`, `flex-column`, `align-items-center`, `justify-content-center` untuk mengatur layout menggunakan Flexbox
- `min-vh-100` untuk membuat elemen memenuhi tinggi layar penuh
- `display-3`, `fw-bold`, `lead`, `fs-1`, `fs-5` untuk mengatur ukuran dan ketebalan teks
- `mb-4`, `mt-5`, `py-5`, `g-4` untuk mengatur jarak antar elemen

**Card** merupakan komponen Bootstrap yang digunakan untuk menampilkan konten dalam sebuah kotak dengan tampilan yang rapi. Card terdiri dari beberapa bagian yaitu `card`, `card-body`, `card-title`, dan `card-text`.

---

## 2. Penjelasan Kode

Berikut adalah implementasi halaman Ramadan menggunakan Bootstrap 5 semaksimal mungkin dengan meminimalkan penggunaan native CSS.

### Kode HTML (index.html)
```html
<!-- 
    Nama  : Annisa Al Jauhar
    NIM   : 2311102014
    Kelas : S1 IF-11-REG01
-->
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ramadan Kareem</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body class="bg-dark text-white">

    <div class="min-vh-100 d-flex flex-column align-items-center justify-content-center text-center py-5">

        <!-- Header -->
        <div class="mb-4">
            <p style="font-size:100px">🌙</p>
            <h1 class="display-3 fw-bold text-warning">Ramadan Kareem</h1>
            <p class="lead text-light">Marhaban Ya Ramadan 1446 H</p>
        </div>

        <!-- Cards -->
        <div class="container">
            <div class="row justify-content-center g-4">
                <div class="col-md-4">
                    <div class="card bg-secondary text-white h-100">
                        <div class="card-body text-center">
                            <p class="fs-1">🕌</p>
                            <h5 class="card-title text-warning">Perbanyak Ibadah</h5>
                            <p class="card-text">Bulan penuh berkah untuk memperbanyak sholat, dzikir, dan membaca Al-Quran.</p>
                        </div>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="card bg-secondary text-white h-100">
                        <div class="card-body text-center">
                            <p class="fs-1">⭐</p>
                            <h5 class="card-title text-warning">Malam Lailatul Qadar</h5>
                            <p class="card-text">Malam yang lebih baik dari seribu bulan, raihlah di 10 malam terakhir Ramadan.</p>
                        </div>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="card bg-secondary text-white h-100">
                        <div class="card-body text-center">
                            <p class="fs-1">🤲</p>
                            <h5 class="card-title text-warning">Perbanyak Sedekah</h5>
                            <p class="card-text">Ramadan adalah bulan berbagi, perbanyak sedekah dan bantu sesama.</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>

        <!-- Quote -->
        <div class="container mt-5">
            <div class="card bg-secondary text-white mx-auto" style="max-width:600px">
                <div class="card-body">
                    <p class="text-warning fst-italic fs-5">"Barang siapa yang berpuasa di bulan Ramadan dengan penuh keimanan dan mengharap pahala, maka dosa-dosanya yang telah lalu akan diampuni."</p>
                    <p class="text-light small">- HR. Bukhari & Muslim</p>
                </div>
            </div>
        </div>

        <!-- Footer -->
        <div class="mt-5">
            <p class="text-warning fs-5">✨ Selamat Menunaikan Ibadah Puasa dari Nisa ✨</p>
            <p class="text-light small">Semoga amal ibadah kita diterima Allah SWT</p>
        </div>

    </div>

    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
```

### Penjelasan Kode

Bootstrap di-import menggunakan CDN melalui tag `<link>` di bagian `<head>`, sehingga tidak perlu mengunduh file Bootstrap secara manual.

Pada bagian `<body>`, class `bg-dark` memberikan background gelap dan `text-white` membuat semua teks berwarna putih secara default.

Div utama menggunakan class `min-vh-100 d-flex flex-column align-items-center justify-content-center text-center py-5` yang membuat seluruh konten berada di tengah layar secara vertikal dan horizontal menggunakan Flexbox Bootstrap.

Bagian cards menggunakan Grid System Bootstrap dengan class `row` dan `col-md-4` sehingga 3 kartu ditampilkan sejajar pada layar medium ke atas. Setiap kartu menggunakan komponen `card` Bootstrap dengan class `bg-secondary` untuk warna background abu-abu gelap.

Native CSS yang digunakan hanya `font-size:100px` pada emoji bulan dan `max-width:600px` pada card quote, karena Bootstrap tidak menyediakan ukuran tersebut secara langsung.

---

## 3. Hasil

![Hasil Halaman Ramadan](screenshot-modul-4.png)

---

<div align="center">

</div>