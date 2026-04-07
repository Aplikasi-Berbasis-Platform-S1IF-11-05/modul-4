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
    <strong>Adrian Basari Rhesa</strong>
    <br>
    <strong>2311102105</strong>
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
<!-- 2311102105-Adrian Basari Rhesa -->
<!DOCTYPE html>
<html lang="id">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>Mode Suci - Ramadan</title>

    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">

    <style>
        /* Variabel Tema Premium Ramadan */
        :root {
            --gold: #FFD700;
            --dark-blue: #0A1128;
            --card-glass: rgba(255, 255, 255, 0.05);
            --border-glass: rgba(255, 255, 255, 0.1);
        }

        body {
            font-family: 'Poppins', sans-serif;
            background: linear-gradient(135deg, var(--dark-blue), #1C2541, #3A506B);
            color: #fff;
            min-height: 100vh;
            display: flex;
            flex-direction: column;
        }

        /* Custom Navbar with Glassmorphism */
        .navbar {
            background: rgba(10, 17, 40, 0.8) !important;
            backdrop-filter: blur(15px);
            -webkit-backdrop-filter: blur(15px);
            border-bottom: 1px solid var(--border-glass);
        }

        .navbar-brand {
            color: var(--gold) !important;
            font-size: 1.5rem;
        }

        .nav-link {
            color: #ddd !important;
            transition: color 0.3s;
        }

        .nav-link:hover,
        .nav-link.active {
            color: var(--gold) !important;
        }

        /* Hero Section */
        .hero-section {
            padding: 80px 0 50px;
        }

        .text-gold {
            color: var(--gold);
        }

        .moon-icon {
            display: inline-block;
            font-size: 3.5rem;
            margin-bottom: 15px;
            animation: float 3s ease-in-out infinite;
        }

        /* Keyframe untuk animasi mengambang */
        @keyframes float {
            0% {
                transform: translateY(0px);
            }

            50% {
                transform: translateY(-15px);
            }

            100% {
                transform: translateY(0px);
            }
        }

        /* Custom Cards */
        .ramadan-card {
            background: var(--card-glass);
            border: 1px solid var(--border-glass);
            border-radius: 20px;
            backdrop-filter: blur(10px);
            -webkit-backdrop-filter: blur(10px);
            transition: transform 0.3s ease, box-shadow 0.3s ease, border-color 0.3s;
        }

        .ramadan-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(255, 215, 0, 0.15);
            border-color: rgba(255, 215, 0, 0.5);
        }

        .card-title {
            font-size: 1.5rem;
            color: var(--gold);
        }

        /* Custom Button */
        .btn-custom {
            background-color: var(--gold);
            color: #000;
            font-weight: 600;
            border: none;
            border-radius: 30px;
            padding: 10px 25px;
            transition: all 0.3s ease;
        }

        .btn-custom:hover {
            background-color: #fff;
            color: #000;
            transform: scale(1.05);
            box-shadow: 0 5px 15px rgba(255, 215, 0, 0.4);
        }

        /* Custom Table */
        .table-container {
            background: var(--card-glass);
            border-radius: 20px;
            padding: 20px;
            border: 1px solid var(--border-glass);
            backdrop-filter: blur(10px);
        }

        .table {
            color: #fff;
            margin-bottom: 0;
        }

        .table th {
            border-bottom: 2px solid var(--gold);
            color: var(--gold);
            background: transparent;
        }

        .table td {
            border-bottom: 1px solid rgba(255, 255, 255, 0.05);
            background: transparent;
            color: #e0e0e0;
            padding: 15px;
        }

        .table-striped>tbody>tr:nth-of-type(odd)>* {
            background-color: rgba(255, 255, 255, 0.02);
            color: #fff;
        }

        /* Footer */
        footer {
            margin-top: auto;
            background: rgba(10, 17, 40, 0.9);
            border-top: 1px solid var(--border-glass);
            color: #aaa;
        }
    </style>
</head>

<body>

    <nav class="navbar navbar-expand-lg sticky-top">
        <div class="container">
            <a class="navbar-brand fw-bold" href="#">Mode Suci 🌙</a>
            <button class="navbar-toggler border-0 shadow-none" type="button" data-bs-toggle="collapse"
                data-bs-target="#navbarNav">
                <span class="navbar-toggler-icon" style="filter: invert(1);"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav ms-auto">
                    <li class="nav-item"><a class="nav-link active fw-semibold" href="#">Beranda</a></li>
                    <li class="nav-item"><a class="nav-link" href="#kegiatan">Kegiatan</a></li>
                    <li class="nav-item"><a class="nav-link" href="#jadwal">Jadwal</a></li>
                    <li class="nav-item"><a class="nav-link" href="#">Kontak</a></li>
                </ul>
            </div>
        </div>
    </nav>

    <section class="container text-center hero-section">
        <span class="moon-icon">🌙</span>
        <h1 class="display-4 fw-bold mb-3">Selamat Menjalankan <br> <span class="text-gold">Ibadah Puasa</span></h1>
        <p class="lead text-light opacity-75 mb-4">Tingkatkan iman, perbanyak amal, dan raih keberkahan di bulan suci.
        </p>
        <span class="badge text-bg-warning fs-6 px-4 py-2 rounded-pill shadow-sm">#ModeSuciAktif ✨</span>
    </section>

    <section id="kegiatan" class="container py-5">
        <h2 class="text-center mb-5 fw-bold">Kegiatan <span class="text-gold">Ramadan</span></h2>
        <div class="row g-4">

            <div class="col-md-4">
                <div class="card ramadan-card h-100 p-3 text-center">
                    <div class="card-body">
                        <div class="mb-3" style="font-size: 3rem;">🕌</div>
                        <h5 class="card-title fw-bold">Tarawih</h5>
                        <p class="card-text text-light opacity-75 mb-4">Shalat malam yang memperkuat keimanan di bulan
                            penuh berkah.</p>
                        <a href="#" class="btn btn-custom">Ikuti Sekarang</a>
                    </div>
                </div>
            </div>

            <div class="col-md-4">
                <div class="card ramadan-card h-100 p-3 text-center">
                    <div class="card-body">
                        <div class="mb-3" style="font-size: 3rem;">📖</div>
                        <h5 class="card-title fw-bold">Tadarus</h5>
                        <p class="card-text text-light opacity-75 mb-4">Membaca, memahami, dan mengamalkan ayat suci
                            Al-Qur'an.</p>
                        <a href="#" class="btn btn-custom">Mulai Membaca</a>
                    </div>
                </div>
            </div>

            <div class="col-md-4">
                <div class="card ramadan-card h-100 p-3 text-center">
                    <div class="card-body">
                        <div class="mb-3" style="font-size: 3rem;">🤲</div>
                        <h5 class="card-title fw-bold">Sedekah</h5>
                        <p class="card-text text-light opacity-75 mb-4">Berbagi kebahagiaan kepada sesama untuk
                            menyucikan harta.</p>
                        <a href="#" class="btn btn-custom">Salurkan Donasi</a>
                    </div>
                </div>
            </div>

        </div>
    </section>

    <section id="jadwal" class="container py-5 mb-5">
        <h2 class="text-center mb-5 fw-bold">Jadwal <span class="text-gold">Harian</span></h2>
        <div class="row justify-content-center">
            <div class="col-lg-8">
                <div class="table-container">
                    <table class="table table-hover table-borderless text-center align-middle">
                        <thead>
                            <tr>
                                <th>Waktu</th>
                                <th>Kegiatan</th>
                            </tr>
                        </thead>
                        <tbody>
                            <tr>
                                <td class="fw-semibold text-gold fs-5">04:30</td>
                                <td class="fs-5">Sahur & Imsak</td>
                            </tr>
                            <tr>
                                <td class="fw-semibold text-gold fs-5">18:00</td>
                                <td class="fs-5">Buka Puasa & Maghrib</td>
                            </tr>
                            <tr>
                                <td class="fw-semibold text-gold fs-5">19:30</td>
                                <td class="fs-5">Isya & Tarawih berjamaah</td>
                            </tr>
                        </tbody>
                    </table>
                </div>
            </div>
        </div>
    </section>

    <footer class="text-center py-4">
        <p class="mb-0 fs-6">© 2026 Mode Suci Ramadan | Dirancang dengan ✨ Bootstrap 5</p>
    </footer>

    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>

</body>

</html>

```

## Output

<img width="1920" height="1080" alt="Screenshot (1066)" src="https://github.com/user-attachments/assets/ee27a2cc-af58-4adb-8427-d727addfe5fd" />
