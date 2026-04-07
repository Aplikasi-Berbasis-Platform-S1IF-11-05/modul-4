<div align="center">
  <br />
  <h1>LAPORAN PRAKTIKUM <br> APLIKASI BERBASIS PLATFORM </h1>
  <br />
  <h3>MODUL 4 <br> Bootstrap </h3>
  <br />
  <img width="512" height="512" alt="telyu" src="https://github.com/user-attachments/assets/724a3291-bcf9-448d-a395-3886a8659d79" />
  <br />
  <br />
  <br />
  <h3>Disusun Oleh :</h3>
  <p>
    <strong>Verdi Pangestu</strong>
    <br>
    <strong>2311102100</strong>
    <br>
    <strong>S1 IF-11-REG05</strong>
  </p>
  <br />
  <h3>Dosen Pengampu :</h3>
  <p>
    <strong>Dedi Agung Prabowo, S.Kom., M.Kom</strong>
  </p>
  <br />
  <br />
  <h4>Asisten Praktikum :</h4>
  <strong>Apri Pandu Wicaksono</strong>
  <br>
  <strong>Hamka Zaenul Ardi</strong>
  <br />
  <h3>LABORATORIUM HIGH PERFORMANCE <br>FAKULTAS INFORMATIKA <br>UNIVERSITAS TELKOM PURWOKERTO <br>2026 </h3>
</div>

<hr>

# Dasar Teori

## 1. Bootstrap

Bootstrap adalah framework CSS open-source yang paling banyak digunakan untuk membangun tampilan web yang responsif dan modern. Dengan Bootstrap, kita tidak perlu menulis CSS dari nol karena sudah tersedia class-class siap pakai yang tinggal diterapkan langsung ke elemen HTML.

Bootstrap pertama kali dikembangkan oleh Twitter pada tahun 2011 dan sekarang sudah masuk versi 5. Pada versi 5, Bootstrap tidak lagi bergantung pada jQuery sehingga lebih ringan dan cepat.

---

## 2. Cara Menggunakan Bootstrap

Bootstrap bisa digunakan dengan dua cara:

- **CDN** — Menghubungkan langsung via link dari internet, cara paling mudah dan tidak perlu install apapun.
- **Download** — Mengunduh file Bootstrap lalu menyimpannya secara lokal.

Pada praktikum ini digunakan metode **CDN**:

```html
<!-- CSS Bootstrap -->
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet"/>

<!-- JS Bootstrap (untuk komponen interaktif seperti navbar) -->
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
```

---

## 3. Grid System

Salah satu fitur utama Bootstrap adalah sistem grid 12 kolom yang memudahkan penataan layout halaman. Grid Bootstrap bekerja dengan class `row` dan `col`.

```html
<div class="row">
  <div class="col-md-6">Kolom kiri</div>
  <div class="col-md-6">Kolom kanan</div>
</div>
```

Breakpoint yang tersedia:

| Class | Breakpoint | Lebar Layar |
|-------|-----------|-------------|
| `col-` | xs | < 576px |
| `col-sm-` | Small | ≥ 576px |
| `col-md-` | Medium | ≥ 768px |
| `col-lg-` | Large | ≥ 992px |
| `col-xl-` | Extra large | ≥ 1200px |

---

## 4. Komponen Bootstrap yang Digunakan

### Navbar
Komponen navigasi responsif yang otomatis berubah menjadi hamburger menu di layar kecil.

```html
<nav class="navbar navbar-expand-lg navbar-dark bg-dark">
  <div class="container">
    <a class="navbar-brand" href="#">Brand</a>
  </div>
</nav>
```

### Card
Komponen kotak konten yang fleksibel dengan berbagai variasi tampilan.

```html
<div class="card">
  <div class="card-body">
    <h5 class="card-title">Judul</h5>
    <p class="card-text">Isi konten.</p>
  </div>
</div>
```

### Badge
Label kecil untuk menampilkan status atau kategori.

```html
<span class="badge bg-primary">Wajib</span>
```

### Table
Tabel dengan berbagai class untuk tampilan yang lebih menarik.

```html
<table class="table table-dark table-hover table-bordered">
  ...
</table>
```

### Progress Bar
Komponen untuk menampilkan progress dalam bentuk bar.

```html
<div class="progress">
  <div class="progress-bar" style="width: 70%">70%</div>
</div>
```

### Alert
Kotak pesan untuk menampilkan informasi atau notifikasi.

```html
<div class="alert alert-warning" role="alert">
  Pesan penting di sini.
</div>
```

---

## 5. Utility Classes

Bootstrap menyediakan banyak utility class untuk styling cepat tanpa perlu menulis CSS:

- `text-center`, `text-start`, `text-end` — Perataan teks
- `fw-bold`, `fw-semibold` — Ketebalan font
- `p-3`, `px-4`, `py-2` — Padding
- `m-3`, `mx-auto`, `mb-4` — Margin
- `d-flex`, `justify-content-center`, `align-items-center` — Flexbox
- `shadow`, `rounded`, `rounded-4` — Efek visual
- `gap-3`, `g-4` — Jarak antar elemen
- `fs-1` hingga `fs-6` — Ukuran font

---

# Tugas 4 — Mode Suci (Edisi Ramadan)

## Code

```html
<!-- 2311102100-Verdi Pangestu -->
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ramadan Hub - Pure Bootstrap</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.11.0/font/bootstrap-icons.css">
    <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@300;400;700&display=swap" rel="stylesheet">
    <style>
        body { font-family: 'Plus Jakarta Sans', sans-serif; }
    </style>
</head>
<body class="bg-black min-vh-100 d-flex flex-column text-light">

    <nav class="navbar navbar-expand-lg navbar-dark py-4 container">
        <div class="container-fluid">
            <a class="navbar-brand fw-bold fs-4 tracking-wider text-info" href="#">
                <i class="bi bi-moon-stars-fill me-2"></i>RAMADAN<span class="text-light opacity-75">HUB</span>
            </a>
            <button class="navbar-toggler border-0" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav ms-auto gap-lg-4 text-center">
                    <li class="nav-item"><a class="nav-link active fw-semibold" href="#">BERANDA</a></li>
                    <li class="nav-item"><a class="nav-link text-white-50" href="#">IMSAYKIYAH</a></li>
                    <li class="nav-item"><a class="nav-link text-white-50" href="#">MUTABAAH</a></li>
                    <li class="nav-item"><a class="nav-link btn btn-primary rounded-pill px-4 ms-lg-2 text-info" href="#">DONASI</a></li>
                </ul>
            </div>
        </div>
    </nav>

    <main class="container my-auto py-5">
        <div class="row align-items-center g-5">
            
            <div class="col-lg-6 text-center text-lg-start">
                <h2 class="display-6 fw-light mb-0 text-white-50">Sambut Bulan Suci</h2>
                <h1 class="display-1 fw-bold mb-0">Ramadan</h1>
                <h1 class="display-3 fw-bold text-info mb-4">Kareem 1447 H</h1>
                
                <div class="bg-info bg-opacity-10 border-start border-info border-4 p-4 mb-5 rounded-end">
                    <p class="lead text-white-75 mb-0 fs-6 italic">
                        "Wahai orang-orang yang beriman! Diwajibkan atas kamu berpuasa sebagaimana diwajibkan atas orang sebelum kamu agar kamu bertakwa." (QS. Al-Baqarah: 183)
                    </p>
                </div>

                <div class="row g-3 mb-5">
                    <div class="col-6 col-md-4">
                        <div class="p-4 rounded-4 text-center border border-info border-opacity-25 bg-white bg-opacity-10 shadow-sm">
                            <i class="bi bi-clock-history text-info fs-2"></i>
                            <p class="small mb-0 mt-3 fw-medium">Jadwal Shalat</p>
                        </div>
                    </div>
                    <div class="col-6 col-md-4">
                        <div class="p-4 rounded-4 text-center border border-info border-opacity-25 bg-white bg-opacity-10 shadow-sm">
                            <i class="bi bi-book text-info fs-2"></i>
                            <p class="small mb-0 mt-3 fw-medium">Kajian Harian</p>
                        </div>
                    </div>
                    <div class="col-12 col-md-4">
                        <div class="p-4 rounded-4 text-center border border-info border-opacity-25 bg-white bg-opacity-10 shadow-sm">
                            <i class="bi bi-heart-pulse text-info fs-2"></i>
                            <p class="small mb-0 mt-3 fw-medium">Info Zakat</p>
                        </div>
                    </div>
                </div>

                <div class="d-flex flex-column flex-sm-row gap-3 justify-content-center justify-content-lg-start">
                    <a href="#" class="btn btn-info btn-lg rounded-pill px-5 py-3 fw-bold shadow">JADWAL IMSAK</a>
                    <a href="#" class="btn btn-outline-light btn-lg rounded-pill px-5 py-3 border-opacity-50 text-white-50">PANDUAN IBADAH</a>
                </div>
            </div>

            <div class="col-lg-6 position-relative text-center">
                <div class="position-absolute top-0 end-0 mt-n5 me-5 opacity-25 d-none d-lg-block">
                    <i class="bi bi-stars display-1 text-info"></i>
                </div>

                <div class="position-relative py-5">
                    <div class="position-absolute top-50 start-50 translate-middle rounded-circle bg-info opacity-10 shadow-lg" style="width: 300px; height: 300px; filter: blur(80px);"></div>
                    
                    <i class="bi bi-mosque text-info opacity-75 position-relative" style="font-size: 14rem; z-index: 2;"></i>
                    
                    <div class="mt-5">
                        <span class="badge rounded-pill bg-info bg-opacity-25 text-info px-4 py-3 border border-info border-opacity-25">
                            <i class="bi bi-geo-alt-fill me-2"></i>Waktu Indonesia Barat (WIB)
                        </span>
                    </div>
                </div>
            </div>
        </div>
    </main>

    <footer class="py-5 mt-auto bg-dark bg-opacity-25 border-top border-secondary border-opacity-10">
        <div class="container text-center text-md-start">
            <div class="row align-items-center">
                <div class="col-md-6 d-flex justify-content-center justify-content-md-start gap-4 mb-4 mb-md-0">
                    <a href="#" class="text-info opacity-75 fs-4"><i class="bi bi-facebook"></i></a>
                    <a href="#" class="text-info opacity-75 fs-4"><i class="bi bi-instagram"></i></a>
                    <a href="#" class="text-info opacity-75 fs-4"><i class="bi bi-youtube"></i></a>
                </div>
                <div class="col-md-6 text-center text-md-end">
                    <p class="small text-white-50 mb-0">Ramadan Hub &copy; 2026. Semoga keberkahan menyertai kita semua.</p>
                </div>
            </div>
        </div>
    </footer>

    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
```

## Output
<img width="1919" height="972" alt="Cuplikan layar 2026-04-07 115728" src="https://github.com/user-attachments/assets/cce4adf7-afef-4621-80e3-60af59c9e411" />
