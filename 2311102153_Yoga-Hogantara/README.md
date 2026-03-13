<div align="center">
  <br />
  <h1>LAPORAN PRAKTIKUM <br>APLIKASI BERBASIS PLATFORM</h1>
  <br />
  <h3>MODUL 4 <br> BOOTSTRAP</h3>
  <br />
  <br />
  <img src="logo.jpeg" alt="Logo" width="300"> 
  <br />
  <br />
  <br />
  <br />
  <h3>Disusun Oleh :</h3>
  <p>
    <strong>Yoga Hogantara</strong><br>
    <strong>2311102153</strong><br>
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

**Bootstrap** merupakan sebuah kerangka kerja (*framework*) *front-end* gratis dan terbuka yang paling banyak digunakan untuk mempercepat pembuatan desain website. Jika biasanya kita harus menulis kode CSS satu per satu secara manual, Bootstrap sudah menyediakan "cetakan" siap pakai berbasis HTML, CSS, dan JavaScript. Komponen seperti tombol, menu navigasi, hingga kolom formulir bisa langsung kita gunakan tanpa harus membuat desainnya dari nol.

Salah satu alasan utama Bootstrap sangat disukai adalah **Sistem Grid Responsif**-nya. Dengan menggunakan aturan *container*, *row*, dan *column*, kita bisa mengatur tata letak halaman yang secara otomatis menyesuaikan diri dengan ukuran layar, baik itu di monitor komputer yang lebar maupun layar *smartphone* yang kecil.

Beberapa kelebihan utama dari penggunaan Bootstrap antara lain:

1. **Efisiensi Waktu**  
  Pengembang tidak perlu lagi dipusingkan dengan pengaturan dasar seperti margin, *padding*, atau struktur *flexbox*. Semuanya sudah disediakan dalam bentuk *class* siap panggil.

2. **Konsistensi Tampilan**  
   Bootstrap menjamin tampilan website tetap terlihat rapi dan konsisten meskipun dibuka di berbagai jenis peramban (*browser*) yang berbeda.

3. **Responsif Secara Default**  
   Sejak awal, komponen di dalamnya sudah dirancang agar pas untuk tampilan ponsel, sehingga website kita otomatis menjadi responsif tanpa perlu banyak modifikasi tambahan.

Bootstrap bisa digunakan secara **offline** dengan mengunduh filenya langsung, atau secara **online** yang lebih praktis lewat jalur **CDN (Content Delivery Network)**.

## 2. Penjelasan Kode HTML

### Kode HTML

```html
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Marhaban Ya Ramadan</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body class="bg-success text-white vh-100 d-flex justify-content-center align-items-center">
    
    <div class="container text-center">
        <div class="row justify-content-center">
            <div class="col-12 col-md-8 col-lg-6">
                <div class="p-5 bg-dark bg-opacity-50 rounded-4 shadow-lg border border-2 border-light">
                    
                    <h1 class="display-4 fw-bold mb-3 text-warning">Marhaban Ya Ramadan</h1>
                    <p class="lead fs-5 mb-4">Selamat menunaikan ibadah puasa. </p>
                    
                    <hr class="border-light border-2 opacity-75 mb-4">
                    
                    <div class="d-flex justify-content-center gap-5 my-4">
                        <div class="text-center">
                            <div class="display-2 mb-2">🍲🍗</div>
                            <span class="badge bg-warning text-dark fs-6 rounded-pill">أطباق الدجاج</span>
                        </div>
                        
                        <div class="text-center">
                            <div class="display-2 mb-2">✉️💵</div>
                            <span class="badge bg-warning text-dark fs-6 rounded-pill">THR Cik</span>
                        </div>
                    </div>

                    <p class="fst-italic fs-6 text-light opacity-75 mt-4">"Yoga Hogantara-2311102153"</p>
                </div>
            </div>
        </div>
    </div>

</body>
</html>
```

### Hasil Tampilan (Screenshot)

![Hasil Tampilan Bootstrap](1.PNG)

### Penjelasan Code

### A. Integrasi dan Struktur Dasar
* **Bootstrap CDN**: Di dalam bagian `<head>`, saya menggunakan elemen `<link>` untuk menghubungkan dokumen dengan pustaka Bootstrap eksternal. Hal ini memungkinkan saya menggunakan fitur desain modern tanpa harus menulis banyak kode CSS manual.
* **Viewport & Layout**: Pengaturan `meta viewport` memastikan kartu ucapan tampil rapi di layar ponsel maupun komputer. Seluruh elemen dibungkus menggunakan sistem **Grid** (`container`, `row`, `col`) agar tata letaknya tetap presisi.

### B. Analisis Styling via Utility Classes
Dalam kode ini, saya menggunakan teknik *utility-first* yang disediakan oleh Bootstrap untuk mengatur tampilan:

* **Pusat Tata Letak (Centering)**: Pada bagian `body`, saya menggunakan kombinasi *class* `d-flex`, `justify-content-center`, dan `align-items-center`. Ditambah dengan `vh-100`, ini memastikan kartu ucapan tampil tepat di tengah layar secara vertikal dan horizontal.
* **Visual Kartu**: 
    * **Background & Warna**: Latar belakang utama menggunakan warna hijau (`bg-success`) khas nuansa Ramadan, sementara kartu utama diberikan efek transparan dengan `bg-dark bg-opacity-50`.
    * **Estetika**: Saya menambahkan `rounded-4` untuk sudut kartu yang sangat melengkung (modern), `shadow-lg` untuk memberikan efek bayangan yang dalam, serta `border-light` untuk mempertegas batas kartu.
* **Tipografi**:
    * Judul utama menggunakan `display-4` untuk ukuran teks yang besar namun tetap proporsional, serta warna `text-warning` (kuning/emas) untuk memberikan kesan cerah dan mewah.
    * Identitas saya (**Yoga Hogantara-2311102153**) menggunakan *class* `fst-italic` agar terlihat lebih personal dan estetis di bagian bawah kartu.

### C. Komponen Dekoratif
* **Badge & Icon**: Saya menggunakan emoji sebagai representasi visual yang diletakkan di dalam sistem Flexbox (`gap-5`) untuk memberikan jarak yang pas.
* **Pill Badges**: Untuk teks "أطباق الدجاج" dan "THR Cik", saya menggunakan *class* `badge rounded-pill` dengan warna `bg-warning` agar terlihat menonjol dan menyerupai label modern.

## Refrensi

- [Materi Modul 4](https://drive.google.com/file/d/1TW5Y0AdzkVk24ThPUf1OQNs2Mnw3XNO5/view?usp=sharing)
