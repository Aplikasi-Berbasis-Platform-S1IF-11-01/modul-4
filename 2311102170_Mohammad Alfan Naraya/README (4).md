<div align="center">
  <br />
  <h1>LAPORAN PRAKTIKUM <br>APLIKASI BERBASIS PLATFORM</h1>
  <br />
  <h3>MODUL 4 <br> BOOTSTRAP</h3>
  <br />
  <br />
  <img src="assets/logo.jpeg" alt="Logo" width="300"> 
  <br />
  <br />
  <br />
  <br />
  <h3>Disusun Oleh :</h3>
  <p>
    <strong>Mohammad Alfan Naraya</strong><br>
    <strong>2311102170</strong><br>
    <strong>S1 IF-11-01</strong>
  </p>
  <br />
  <h3>Dosen Pengampu :</h3>
  <p>
    <strong>Dimas Fanny Hebrasianto Permadi, S.ST., M.Kom</strong>
  </p>
  <br />
  <br />
    <h4>Asisten Praktikum :</h4>
    <strong> Apri Pandu Wicaksono </strong> <br>
    <strong>Rangga Pradarrell Fathi</strong>
  <br />
  <h3>LABORATORIUM HIGH PERFORMANCE
 <br>FAKULTAS INFORMATIKA <br>UNIVERSITAS TELKOM PURWOKERTO <br>2026</h3>
</div>

---

## 1. Dasar Teori

**Bootstrap**
adalah salah satu framework CSS paling populer di dunia yang digunakan untuk mengembangkan situs web yang responsif (responsive) dan mengutamakan perangkat seluler (mobile-first).

Secara sederhana, Bootstrap adalah kumpulan "potongan kode" siap pakai (CSS dan JavaScript) yang memungkinkan pengembang membangun antarmuka web dengan cepat tanpa harus menulis kode dari nol.

Beberapa keunggulan utama dari penggunaan Bootstrap antara lain:

1. **Efisiensi Waktu**  
   Tidak perlu menulis ribuan baris CSS secara manual.

2. **Konsistensi Tampilan**  
   Menjamin tampilan elemen tetap sama di berbagai browser (Chrome, Safari, Firefox).

3. **Responsif Secara Default**  
   Sebagian besar komponen Bootstrap dirancang dengan pendekatan **mobile-first**, Strategi desain yang memprioritaskan perangkat layar kecil terlebih dahulu, kemudian ditingkatkan untuk layar besar. sehingga tampilan sudah responsif sejak awal pengembangan.

Bootstrap dapat digunakan secara **offline** dengan mengunduh _source file_ dari situs resminya, atau secara **online** melalui layanan **Content Delivery Network (CDN)**.

## 2. Penjelasan Kode HTML

Berikut merupakan implementasi kartu ucapan Ramadhan berbasis _Bootstrap 5 Utility-First, di mana hampir semua pengaturan tampilan dilakukan langsung di dalam atribut class_tanpa menyertakan dokumen CSS tambahan apa pun, beserta hasil eksekusinya.

### Kode HTML (`modul4.html`)

```html
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ucapan Ramadan 1447H</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.11.2/font/bootstrap-icons.css">
</head>
<body class="bg-success bg-gradient vh-100 d-flex align-items-center">

    <div class="container">
        <div class="row justify-content-center">
            <div class="col-11 col-sm-9 col-md-7 col-lg-5 text-center">
                
                <div class="card shadow-lg border-0 rounded-5 overflow-hidden">
                    
                    <div class="card-header bg-white border-0 pt-5">
                        <i class="bi bi-moon-stars-fill text-warning display-2"></i>
                        <h2 class="fw-bold text-success mt-3 mb-0">RAMADAN KAREEM</h2>
                        <small class="text-muted fw-light">1447 HIJRIAH</small>
                    </div>

                    <div class="card-body px-4 px-md-5 pb-5 bg-white">
                        <hr class="w-25 mx-auto mb-4 text-success border-2 opacity-50">
                        
                        <h1 class="h4 fw-bold text-dark mb-3">Selamat Menunaikan Ibadah Puasa</h1>
                        
                        <p class="card-text text-secondary lh-lg mb-4">
                            Semoga di bulan yang penuh cahaya ini, setiap langkah kita diberkahi, 
                            setiap doa didengarkan, dan hati kita dipenuhi dengan kedamaian 
                            serta rasa syukur yang mendalam.
                        </p>

                        <div class="mt-4 pt-4 border-top">
                            <p class="small text-muted mb-1 text-uppercase" style="letter-spacing: 2px;">Salam Hangat</p>
                            <h5 class="fw-bold text-success mb-0">Mohammad Alfan Naraya</h5>
                        </div>
                    </div>
                    
                    <div class="card-footer bg-warning border-0 py-2"></div>
                </div>

                <p class="mt-4 text-white opacity-75 small">
                    <i class="bi bi-geo-alt-fill me-1"></i> Purwokerto, 2026
                </p>

            </div>
        </div>
    </div>

    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
```

### Hasil Tampilan (Screenshot)

![Hasil Tampilan Bootstrap](assets/1.jpg)

### Penjelasan Code

- Pada bagian **head**, dilakukan pemanggilan _library_ **Bootstrap 5** melalui metode **Content Delivery Network (CDN)** menggunakan tag `<link>`. Library ini menyediakan berbagai komponen UI, sistem grid, serta _utility class_ yang digunakan untuk membangun tampilan tanpa perlu menambahkan file CSS tambahan.

- Pada tag **`<body>`**, digunakan class `bg-dark` untuk memberikan latar belakang halaman berwarna gelap. Hal ini bertujuan agar kartu ucapan yang berada di tengah halaman terlihat lebih menonjol secara visual.

- Pada elemen **`container`**, digunakan kombinasi _utility class_ `d-flex vh-100 justify-content-center align-items-center`.

  - `d-flex` mengaktifkan **Flexbox layout**.
  - `vh-100` membuat tinggi elemen menjadi **100% tinggi viewport**.
  - `justify-content-center` memposisikan konten ke **tengah secara horizontal**.
  - `align-items-center` memposisikan konten ke **tengah secara vertikal**.  
    Dengan kombinasi ini, kartu ucapan akan selalu berada tepat di tengah halaman.

- Pada elemen **`.card`**, digunakan komponen kartu bawaan Bootstrap untuk membentuk struktur utama kartu ucapan. Beberapa _utility class_ ditambahkan untuk meningkatkan tampilan visual, antara lain:

  - `text-center` untuk membuat seluruh teks rata tengah.
  - `shadow-lg` untuk memberikan efek bayangan yang lebih tegas pada kartu.
  - `rounded-4` untuk membuat sudut kartu lebih melengkung.
  - `border-0` untuk menghilangkan garis batas default pada kartu.

- Pada bagian **`.card-body`**, digunakan beberapa _utility class_ untuk mempercantik tampilan kartu, yaitu:

  - `bg-success` untuk memberikan warna latar belakang hijau.
  - `text-light` agar warna teks menjadi terang sehingga kontras dengan latar.
  - `rounded-4` untuk menjaga sudut dalam kartu tetap melengkung.
  - `p-5` untuk memberikan jarak **padding** yang cukup di dalam kartu agar isi tidak terlalu rapat.

- Pada elemen teks di dalam kartu, beberapa _utility class_ Bootstrap dimanfaatkan:

  - `fw-bold` untuk membuat judul tampil lebih tebal.
  - `mb-3` dan `mb-4` untuk mengatur **jarak antar elemen** menggunakan margin bawah.
  - `fw-semibold` untuk menegaskan teks pada bagian identitas.

- Elemen **`<hr>`** digunakan sebagai pemisah visual antara pesan ucapan Ramadhan dan informasi identitas pembuat kartu, dengan tambahan class `border-light` agar garis pemisah tetap terlihat jelas di atas latar belakang hijau.

Secara keseluruhan, seluruh desain kartu ucapan dibuat hanya dengan memanfaatkan **komponen dan _utility class_ Bootstrap 5**, tanpa menambahkan file CSS eksternal atau stylesheet khusus.

## Refrensi

- [Materi Modul 4](https://drive.google.com/file/d/1TW5Y0AdzkVk24ThPUf1OQNs2Mnw3XNO5/view?usp=sharing)
