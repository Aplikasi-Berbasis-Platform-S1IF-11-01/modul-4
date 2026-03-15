

<div align="center">
  <br />
  <h1>LAPORAN PRAKTIKUM <br>APLIKASI BERBASIS PLATFORM</h1>
  <br />
  <h3>MODUL 4 <br> BOOTSTRAP</h3>
  <br />
  <img src="https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2F1.bp.blogspot.com%2F-vb7jyBjK-sM%2FXXfKp51LrjI%2FAAAAAAAACts%2FEjcXzlgZwSswNWXsBHMyX-6aav1mjA77QCPcBGAYYCw%2Fs1600%2FLogo_Telkom_University_potrait.png&f=1&nofb=1&ipt=9d030d54102ea96369d39fe491220e0536195abc8ee443279c1a420302206400" alt="Logo Telkom" width="300"> 
  <br /><br /><br />
  
  <h3>Disusun Oleh :</h3>
  <p>
    <strong>Didik Setiawan</strong><br>
    <strong>2311102030</strong><br>
    <strong>IF-11-REG-01</strong>
  </p>
  <br />
  
  <h3>Dosen Pengampu :</h3>
  <p><strong>Dimas Fanny Hebrasianto Permadi, S.ST., M.Kom</strong></p>
  <br />
  
  <h4>Asisten Praktikum :</h4>
  <strong>Apri Pandu Wicaksono</strong> <br>
  <strong>Rangga Pradarrell Fathi</strong>
  <br />
  
  <h3>LABORATORIUM HIGH PERFORMANCE<br>FAKULTAS INFORMATIKA<br>UNIVERSITAS TELKOM PURWOKERTO<br>2026</h3>
</div>

---

## DASAR TEORI

Bootstrap adalah *framework front-end* gratis dan *open-source* yang dikembangkan oleh Mark Otto dan Jacob Thornton dari tim pengembang Twitter pada tahun 2011, sehingga pada awalnya dikenal dengan julukan *Twitter Blueprint*. Framework ini dibangun di atas tiga teknologi dasar web, yaitu HTML untuk struktur, CSS untuk tampilan dan tata letak, serta JavaScript untuk interaktivitas, sehingga memungkinkan para pengembang membangun antarmuka website yang modern dan responsif tanpa harus menulis kode dari awal. Salah satu fitur unggulan Bootstrap adalah sistem grid 12 kolom yang memungkinkan tata letak halaman menyesuaikan diri secara otomatis pada berbagai ukuran layar, mulai dari smartphone, tablet, hingga desktop, sesuai dengan prinsip *mobile-first design*. Selain itu, Bootstrap menyediakan berbagai komponen antarmuka siap pakai seperti navbar, tombol, modal, carousel, dan formulir yang dapat langsung diimplementasikan hanya dengan menambahkan *class* tertentu pada elemen HTML, sehingga mempercepat proses pengembangan web secara signifikan. Bootstrap juga mendukung kustomisasi tampilan melalui variabel Sass dan kompatibilitas lintas browser seperti Chrome, Firefox, dan Internet Explorer, menjadikannya salah satu framework front-end paling populer dan banyak digunakan dalam pengembangan web saat ini.



## UNGUIDED

### kode html



```bash
<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Ramadan 1447 H</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body class="bg-dark text-light">

<nav class="navbar navbar-dark bg-success border-bottom border-warning px-3">
  <span class="navbar-brand fw-bold text-warning">🌙 Ramadan 1447 H — Banjarnegara</span>
  <span class="badge bg-warning text-dark">Hari ke-24</span>
</nav>

<div class="container py-4">

  <!-- HERO -->
  

  <div class="row g-4">

    <!-- JADWAL -->
    <div class="col-md-5">
      <h6 class="text-warning fw-bold mb-3">📅 Jadwal Sholat</h6>
      <div class="row g-2 mb-3">
        <div class="col-6 border border-warning rounded-3 text-center py-2">
          <div class="small text-secondary">🌙 Imsak</div><div class="fw-bold text-warning">04:21</div>
        </div>
        <div class="col-6 border border-success rounded-3 text-center py-2">
          <div class="small text-secondary">🌇 Buka</div><div class="fw-bold text-success">17:58</div>
        </div>
      </div>
      <ul class="list-group">
        <li class="list-group-item bg-dark text-light border-secondary d-flex justify-content-between"><span>🌄 Subuh</span><strong class="text-warning">04:31</strong></li>
        <li class="list-group-item bg-dark text-light border-secondary d-flex justify-content-between"><span>🌤️ Dzuhur</span><strong class="text-warning">11:54</strong></li>
        <li class="list-group-item bg-dark text-light border-secondary d-flex justify-content-between"><span>🌅 Ashar</span><strong class="text-warning">15:02</strong></li>
        <li class="list-group-item bg-success bg-opacity-25 border-warning d-flex justify-content-between"><span>🌇 Maghrib <span class="badge bg-warning text-dark">Buka</span></span><strong class="text-warning">17:58</strong></li>
        <li class="list-group-item bg-dark text-light border-secondary d-flex justify-content-between"><span>🌃 Isya</span><strong class="text-warning">19:07</strong></li>
        <li class="list-group-item bg-dark text-light border-secondary d-flex justify-content-between"><span>🕌 Tarawih</span><strong class="text-warning">±19:30</strong></li>
      </ul>
    </div>

    <!-- DOA + PROGRESS -->
    <div class="col-md-7">
      <h6 class="text-warning fw-bold mb-3">🤲 Doa Berbuka</h6>
      <div class="card bg-dark border-success mb-3">
        <div class="card-body">
          <p class="text-warning text-end fs-5 mb-1" dir="rtl">اللَّهُمَّ لَكَ صُمْتُ وَبِكَ آمَنْتُ وَعَلَى رِزْقِكَ أَفْطَرْتُ</p>
          <p class="small fst-italic text-secondary mb-1">"Allahumma laka shumtu wa bika aamantu wa 'ala rizqika afthartu"</p>
          <p class="small text-light mb-0">Ya Allah, untuk-Mu aku berpuasa, kepada-Mu aku beriman, dan dengan rezeki-Mu aku berbuka.</p>
        </div>
      </div>

      <h6 class="text-warning fw-bold mb-2">📊 Progress Ibadah</h6>
      <div class="small d-flex justify-content-between mb-1"><span>🌙 Puasa</span><span class="text-warning">24/30</span></div>
      <div class="progress mb-2" style="height:8px"><div class="progress-bar bg-success" style="width:80%"></div></div>
      <div class="small d-flex justify-content-between mb-1"><span>📖 Tadarus</span><span class="text-warning">24/30</span></div>
      <div class="progress mb-2" style="height:8px"><div class="progress-bar bg-warning" style="width:80%"></div></div>
      <div class="small d-flex justify-content-between mb-1"><span>🕌 Tarawih</span><span class="text-warning">22/30</span></div>
      <div class="progress mb-3" style="height:8px"><div class="progress-bar bg-info" style="width:73%"></div></div>

      <div class="alert alert-warning bg-warning bg-opacity-10 border-warning text-light py-2">
        <strong class="text-warning">⭐ 10 Malam Terakhir!</strong><br>
        <small>Malam ke-4 dari 10 malam terakhir. Cari Lailatul Qadar di malam ganjil! 🌙</small>
      </div>
    </div>
  </div>
</div>

<footer class="bg-success border-top border-warning text-center py-3">
  <p class="text-warning mb-1">✨ تَقَبَّلَ اللهُ مِنَّا وَمِنْكُم ✨</p>
  <small class="text-light">© 2026 Ramadan Kareem · Banjarnegara · Made with ❤️ for the Ummah</small>
</footer>

<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js"></script>
<script>
  function tick(){const n=new Date(),t=new Date();t.setHours(17,58,0,0);let d=Math.max(0,t-n);document.getElementById('j').textContent=String(Math.floor(d/3600000)).padStart(2,'0');document.getElementById('m').textContent=String(Math.floor(d%3600000/60000)).padStart(2,'0');document.getElementById('s').textContent=String(Math.floor(d%60000/1000)).padStart(2,'0');}
  tick();setInterval(tick,1000);
</script>
</body>
</html>
```



##### penjelasan
dibuat menggunakan Bootstrap 5.3.2. Halaman terdiri dari navbar yang menampilkan judul Ramadan dan badge hari ke-24, lalu container utama dengan dua kolom menggunakan grid Bootstrap. Kolom kiri menampilkan jadwal sholat dalam list-group dengan highlight pada waktu Maghrib sebagai waktu berbuka, sedangkan kolom kanan berisi doa berbuka dalam card, progress ibadah (Puasa, Tadarus, Tarawih) dengan progress-bar, serta alert pengingat 10 malam terakhir Ramadan.



![Alt 1](https://raw.githubusercontent.com/didiksetia1/asset/refs/heads/main/Screenshot%202026-03-14%20212106.png)