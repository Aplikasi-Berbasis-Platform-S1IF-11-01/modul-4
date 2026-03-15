<div align="center">
  <br />
  <h1>LAPORAN PRAKTIKUM <br>APLIKASI BERBASIS PLATFORM</h1>
  <br />
  <h3>MODUL 4 <br> BOOTSTRAP</h3>
  <br />
  <br />
  <img src="assets/logo.jpg" alt="Logo" width="300"> 
  <br />
  <br />
  <br />
  <br />
  <h3>Disusun Oleh :</h3>
  <p>
    <strong>Agnes Refilina Fiska</strong><br>
    <strong>2311102126</strong><br>
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

**Bootstrap** merupakan kerangka kerja (framework) CSS sumber terbuka yang paling banyak diadopsi secara global untuk menciptakan situs web modern yang adaptif dan mengutamakan aksesibilitas pada perangkat seluler (mobile-first).

Secara teknis, Bootstrap adalah pustaka besar berisi komponen kode CSS dan JavaScript yang sudah matang. Hal ini memungkinkan para pengembang untuk menyusun antarmuka pengguna (UI) dengan sistem bongkar-pasang komponen siap pakai, tanpa harus membangun setiap elemen visual dari titik nol.

Beberapa keunggulan utama dari penggunaan Bootstrap antara lain:

1. **Efisiensi Waktu**  
   Memangkas waktu pengerjaan secara signifikan karena pengembang tidak perlu lagi menyusun ribuan baris kode CSS manual untuk elemen dasar.

2. **Konsistensi Tampilan**  
   Memastikan elemen visual seperti tombol, navigasi, dan formulir memiliki tampilan yang konsisten saat diakses melalui berbagai peramban (browser) populer.

3. **Responsif Secara Default**  
   Karena mengusung filosofi mobile-first—yaitu memprioritaskan desain untuk layar kecil sebelum menyesuaikannya ke layar lebar—seluruh komponen di dalamnya sudah memiliki kemampuan responsif secara bawaan.

Bootstrap dapat digunakan secara **offline** dengan mengunduh _source file_ dari situs resminya, atau secara **online** melalui layanan **Content Delivery Network (CDN)**.

## 2. Penjelasan Kode HTML

Berikut merupakan implementasi kartu ucapan Ramadhan berbasis _Bootstrap 5 Utility-First, di mana hampir semua pengaturan tampilan dilakukan langsung di dalam atribut class_tanpa menyertakan dokumen CSS tambahan apa pun, beserta hasil eksekusinya.

### Kode HTML (`Tugas4.html`)

```html
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ramadan Hub - Bright Edition</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.11.1/font/bootstrap-icons.css">
    <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@300;400;700&family=Amiri:ital@1&display=swap" rel="stylesheet">
    
    <style>
        body { 
            font-family: 'Plus Jakarta Sans', sans-serif; 
            background: radial-gradient(circle at top right, #0f172a, #020617);
            color: #f8fafc;
            min-height: 100vh;
        }
        .arabic { font-family: 'Amiri', serif; }
        .glass-card {
            background: rgba(255, 255, 255, 0.05);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.1);
        }
        /* Efek hover halus untuk kartu putih */
        .card-bright:hover {
            transform: translateY(-5px);
            transition: 0.3s;
        }
    </style>
</head>
<body>

    <nav class="navbar navbar-expand-lg navbar-dark pt-4">
        <div class="container">
            <a class="navbar-brand fw-bold fs-4 text-warning" href="#">
                <i class="bi bi-moon-stars-fill me-2"></i>RAMADAN<span class="text-white">1447</span>
            </a>
            <div class="ms-auto">
                <span class="badge rounded-pill bg-warning text-dark px-3 py-2 fw-bold">
                    7 Maret 2026
                </span>
            </div>
        </div>
    </nav>

    <main class="container py-5">
        <div class="row align-items-center mb-5">
            <div class="col-lg-6">
                <h1 class="display-3 fw-bold mb-3">Waktunya <span class="text-warning">Berbenah Diri</span></h1>
                <p class="lead opacity-75 mb-4">Manfaatkan setiap detik di bulan suci ini untuk meraih keberkahan yang tak terhingga.</p>
            </div>
            <div class="col-lg-5 offset-lg-1">
                <div class="p-4 glass-card rounded-4 border-start border-warning border-4 shadow-lg">
                    <i class="bi bi-quote fs-1 text-warning"></i>
                    <p class="fs-4 text-white fw-medium italic">
                        "Barangsiapa yang berpuasa Ramadan karena iman dan mengharap pahala, maka diampuni dosa-dosanya yang telah lalu."
                    </p>
                    <footer class="blockquote-footer text-warning-emphasis mt-2">HR. Bukhari & Muslim</footer>
                </div>
            </div>
        </div>

        <h4 class="mb-4 fw-bold"><i class="bi bi-clock-history me-2 text-warning"></i>Jadwal Sholat Hari Ini</h4>
        <div class="row g-4 mb-5 text-center">
            <div class="col-6 col-md-3">
                <div class="card bg-white text-dark shadow h-100 border-0 rounded-4 card-bright">
                    <div class="card-body py-4">
                        <p class="text-muted mb-1 small fw-bold">SUBUH</p>
                        <h2 class="fw-bold mb-0 text-primary">04:35</h2>
                    </div>
                </div>
            </div>
            <div class="col-6 col-md-3">
                <div class="card bg-white text-dark shadow h-100 border-0 rounded-4 card-bright">
                    <div class="card-body py-4">
                        <p class="text-muted mb-1 small fw-bold">DZUHUR</p>
                        <h2 class="fw-bold mb-0 text-primary">12:01</h2>
                    </div>
                </div>
            </div>
            <div class="col-6 col-md-3">
                <div class="card bg-white text-dark shadow h-100 border-0 rounded-4 card-bright">
                    <div class="card-body py-4">
                        <p class="text-muted mb-1 small fw-bold text-uppercase">ASHAR</p>
                        <h2 class="fw-bold mb-0 text-primary">15:12</h2>
                    </div>
                </div>
            </div>
            <div class="col-6 col-md-3">
                <div class="card bg-warning text-dark h-100 rounded-4 border-0 shadow-lg card-bright">
                    <div class="card-body py-4">
                        <p class="mb-1 small fw-bold text-uppercase">MAGHRIB</p>
                        <h2 class="fw-bold mb-0">18:05</h2>
                        <span class="badge bg-dark text-warning mt-2">Waktunya Buka</span>
                    </div>
                </div>
            </div>
        </div>

        <div class="bg-primary bg-gradient p-4 rounded-4 text-center shadow">
            <p class="mb-0 text-white">"Semoga Allah menerima amal ibadah kita semua di bulan yang mulia ini."</p>
        </div>
    </main>

    <footer class="container py-5 mt-5 text-center text-white-50">
        <p class="small">© 2026 Ramadan Kareem • Developed with ✨</p>
    </footer>

    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
```

### Hasil Tampilan (Screenshot)

![Hasil Tampilan Bootstrap](assets/1.png)

### Penjelasan Code

### 1. Sistem Warna & Latar Belakang
- Radial Gradient: Pada bagian <style>, membuat background yang tidak rata (gelap di tengah, agak terang di pojok). Ini memberikan kedalaman (depth) agar halaman tidak terlihat "flat".
- Contrast Play: Kita mencampurkan elemen gelap (#020617), elemen transparan (glass-card), dan elemen cerah (bg-white). Strategi ini memastikan informasi penting seperti jadwal sholat langsung terlihat oleh mata.

### 2. Komponen Utama
A. Header & Kutipan Hadits
- glass-card: Ini adalah kelas buatan kita yang memanfaatkan backdrop-filter: blur(10px). Efeknya seperti kaca buram yang tembus pandang ke background.
- border-start border-warning border-4: Ini cara Bootstrap memberikan garis vertikal di sebelah kiri kutipan. Angka 4 menentukan ketebalannya.
- text-white & fs-4: Menjamin kutipan hadits memiliki ukuran font yang pas dan warna putih cerah agar kontras dengan latar belakang.
B. Kartu Jadwal Sholat (Grid System)
- row g-4: Membuat baris untuk kartu dengan gutter (jarak antar kartu) sebesar 4 satuan.
- col-6 col-md-3: Ini fitur Responsive. Di HP (layar kecil), kartu akan tampil 2 kolom (6/12). Di laptop (layar sedang ke atas), kartu akan tampil 4 kolom (3/12).
- bg-white & text-dark: Digunakan pada Subuh, Dzuhur, dan Ashar untuk menciptakan tampilan yang bersih dan sangat mudah dibaca.
- bg-warning: Khusus untuk Maghrib, menggunakan warna kuning emas agar menjadi Call to Action (pusat perhatian) bagi pengguna yang sedang menunggu waktu berbuka.

C. Bootstrap Icons
- Menggunakan CDN bootstrap-icons. Contohnya:
- (i class="bi bi-moon-stars-fill"></i) untuk ikon bulan.
- (i class="bi bi-quote"></i) untuk ikon tanda kutip.
- Ini jauh lebih ringan daripada menggunakan file gambar asli (.png/.jpg).

### 3. Utility Classes yang Digunakan
Berikut adalah "mantra" Bootstrap yang paling sering muncul di kode tadi:
- shadow-lg: Memberikan bayangan besar agar elemen terlihat "melayang".
- rounded-4: Membuat sudut kotak menjadi sangat bulat (modern).
- fw-bold / fw-medium: Mengatur ketebalan tulisan.
- py-4 / mb-5: Mengatur jarak vertikal (padding top-bottom dan margin-bottom).

### Tips Modifikasi
Jika ingin mengubah waktu sholat secara dinamis di masa depan, tinggal memberikan id pada angka jamnya (misal: <h2 id="subuh-time">04:35</h2>) dan mengisinya menggunakan JavaScript.

---

## Refrensi

- [Materi Modul 4](https://drive.google.com/file/d/1TW5Y0AdzkVk24ThPUf1OQNs2Mnw3XNO5/view?usp=sharing)
