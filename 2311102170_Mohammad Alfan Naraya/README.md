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

![Hasil Tampilan Bootstrap](assets/output.png)

### Penjelasan Code

### 1. Struktur Pembungkus Utama (Layout)

* **`vh-100`**: (**Vertical Height 100%**) Memastikan tinggi halaman tepat memenuhi satu layar penuh tanpa terpotong.
* **`d-flex align-items-center`**: (**Flexbox**) Berfungsi untuk menempatkan kartu ucapan tepat di tengah layar secara vertikal (atas-bawah).
* **`bg-success bg-gradient`**: (**Background**) Memberikan warna dasar hijau khas Ramadan dengan sentuhan gradasi halus bawaan Bootstrap.
* **`container`**: (**Wrapper**) Menjaga agar konten kartu tidak melebar hingga menyentuh pinggir layar dan tetap rapi di tengah secara responsif.

### 2. Komponen Kartu (The Card)
* **`card shadow-lg`**: Memberikan efek bayangan tebal agar kartu terlihat menonjol/melayang.
* **`border-0 rounded-5`**: Menghilangkan garis tepi dan memberikan lengkungan sudut yang modern.
* **`overflow-hidden`**: Memastikan konten di dalam kartu mengikuti bentuk lengkungan sudut kartu.

### 3. Header & Ikon
* **`card-header bg-white border-0`**: Header bersih tanpa garis pembatas yang menyatu dengan badan kartu.
* **`bi-moon-stars-fill`**: Menggunakan ikon bulan bintang dari *Bootstrap Icons*.
* **`text-warning`**: Memberikan warna kuning/emas cerah pada ikon.
* **`display-2`**: Ukuran tipografi ekstra besar untuk fokus utama pada ikon.

### 4. Tipografi & Isi (Typography)
* **`fw-bold` & `fw-light`**: Memberikan kontras ketebalan teks untuk hirarki informasi yang jelas.
* **`text-success`**: Mengharmonisasikan warna teks dengan tema latar belakang.
* **`lh-lg`**: (*Line Height Large*) Memberikan spasi antar baris kalimat agar pesan lebih nyaman dibaca.
* **`hr w-25 mx-auto`**: Garis pemisah minimalis yang berada tepat di tengah.

### 5. Bagian Penutup (Footer & Nama)
* **`mt-4 pt-4 border-top`**: Memberikan pemisah visual antara pesan ucapan dan nama pengirim.
* **`text-uppercase`**: Memberikan kesan estetik minimalis pada teks "Salam Hangat".
* **`card-footer bg-warning`**: Aksen warna kuning di bagian bawah sebagai penyeimbang visual.

---

## Refrensi

- [Materi Modul 4](https://drive.google.com/file/d/1TW5Y0AdzkVk24ThPUf1OQNs2Mnw3XNO5/view?usp=sharing)
