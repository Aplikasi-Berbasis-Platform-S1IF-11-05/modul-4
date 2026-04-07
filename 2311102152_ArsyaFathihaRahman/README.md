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
    <strong>Arsya Fathiha Rahman</strong>
    <br>
    <strong>2311102152</strong>
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
  <strong>Apri Pandu Wicaksono </strong>
  <br>
  <strong>Hamka Zaenul Ardi</strong>
  <br />
  <h3>LABORATORIUM HIGH PERFORMANCE <br>FAKULTAS INFORMATIKA <br>UNIVERSITAS TELKOM PURWOKERTO <br>2026 </h3>
</div>

<hr>

# Dasar Teori
Bootstrap merupakan framework CSS yang digunakan untuk mempermudah pengembangan tampilan website agar lebih cepat dan responsif. Bootstrap menyediakan berbagai class siap pakai seperti layout grid, komponen UI, serta utility class yang dapat langsung digunakan tanpa harus menulis CSS dari awal.

Dengan Bootstrap, pengembang dapat membuat tampilan website yang rapi dan konsisten hanya dengan menambahkan class tertentu pada elemen HTML. Sistem grid pada Bootstrap memungkinkan pembagian layout menjadi beberapa kolom yang fleksibel sehingga tampilan dapat menyesuaikan berbagai ukuran layar.

Selain itu, Bootstrap juga menyediakan berbagai komponen seperti navbar, card, button, dan lain-lain yang sudah memiliki desain standar. Hal ini membuat proses pembuatan antarmuka menjadi lebih efisien dan mengurangi kebutuhan penulisan CSS secara manual.

Dalam pengembangan halaman bertema Ramadan, Bootstrap dimanfaatkan untuk membangun tampilan yang terstruktur dan menarik dengan memanfaatkan warna, komponen, serta tata letak yang sudah tersedia. Penggunaan class bawaan seperti container, row, dan card membantu menghasilkan tampilan yang modern tanpa perlu banyak konfigurasi tambahan.

# Tugas 4
## 1. Source Kode HTML
```
 //2311102152
 //Arsya Fathiha Rahman

<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ramadan Kareem Estetik | By Arsya</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.11.3/font/bootstrap-icons.min.css">
</head>
<body class="bg-light pb-0 mb-0">

    <div class="fixed-top text-end m-3" style="z-index: 2000;">
        <span class="badge bg-warning bg-opacity-25 text-success rounded-pill fw-lighter tracking-wider p-2 px-3 fs-7 shadow-sm">
            <i class="bi bi-code-slash me-1"></i> BY ARSYA
        </span>
    </div>

    <nav class="navbar navbar-expand-lg navbar-light bg-white rounded-pill shadow-lg mx-md-5 my-4 sticky-top px-4 border border-warning border-opacity-10">
        <div class="container-fluid">
            <a class="navbar-brand fs-4 fw-bolder text-success" href="#">
                <i class="bi bi-moon-stars-fill text-warning me-2 fs-3"></i>Ramadan<span class="text-warning">Kareem</span>
            </a>
            <button class="navbar-toggler border-0 shadow-none" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav ms-auto fw-medium gap-3">
                    <li class="nav-item"><a class="nav-link text-success" href="#">Beranda</a></li>
                    <li class="nav-item"><a class="nav-link" href="#">Jadwal</a></li>
                    <li class="nav-item"><a class="nav-link" href="#">Kajian</a></li>
                    <li class="nav-item ms-md-2">
                        <a class="btn btn-success rounded-pill px-4 fw-bold shadow-sm" href="#">
                            <i class="bi bi-person-circle me-1"></i> Masuk
                        </a>
                    </li>
                </ul>
            </div>
        </div>
    </nav>

    <div class="container my-5 py-5">
        <div class="bg-success bg-gradient text-white rounded-5 shadow-lg p-5 text-center position-relative overflow-hidden border border-5 border-white">
            <i class="bi bi-lantern position-absolute top-0 start-0 opacity-10 text-warning" style="font-size: 15rem; transform: translate(-30%, -20%);"></i>
            <i class="bi bi-moon-stars position-absolute bottom-0 end-0 opacity-10 text-white" style="font-size: 12rem; transform: translate(30%, 30%);"></i>

            <div class="position-relative z-1 py-4">
                <span class="badge bg-light text-success bg-opacity-75 rounded-pill px-4 py-2 mb-4 fw-bold shadow-sm tracking-wide">EDISI 1447H / 2026</span>
                <h1 class="display-1 fw-bolder mb-3 mt-2 tracking-tighter">
                    <span class="text-warning">Marhaban</span><br>Ya Ramadan
                </h1>
                <p class="lead fw-normal mb-5 px-md-5 mx-md-5 text-white-50">
                    Sucikan hati, jernihkan pikiran, perbanyak amalan. Selamat menunaikan ibadah puasa di bulan yang penuh berkah.
                </p>
                <div class="d-flex flex-column flex-md-row gap-3 justify-content-center">
                    <a href="#" class="btn btn-warning btn-lg rounded-pill fw-bold shadow-sm px-5 py-3 text-success">
                        <i class="bi bi-calendar-check me-2"></i> Jadwal Imsakiyah
                    </a>
                    <a href="#" class="btn btn-outline-light btn-lg rounded-pill fw-semibold px-5 py-3 shadow-sm">
                        <i class="bi bi-play-circle me-2"></i> Kultum Hari Ini
                    </a>
                </div>
            </div>
        </div>
    </div>

    <div class="container mb-5 pb-5">
        <div class="row g-4 align-items-stretch">
            <div class="col-md-4">
                <div class="card h-100 border-0 bg-white rounded-5 shadow-lg text-center p-4">
                    <div class="card-body d-flex flex-column justify-content-center align-items-center pt-5">
                        <div class="rounded-pill bg-success bg-opacity-10 border border-success border-opacity-10 shadow-sm p-4 text-success display-5 mb-4">
                            <i class="bi bi-droplet-half"></i>
                        </div>
                        <h3 class="fw-bolder text-success mb-3">Panduan Puasa</h3>
                        <p class="text-secondary mb-4 px-3">Tata cara, niat, doa buka puasa, dan hal yang membatalkan puasa.</p>
                        <a href="#" class="btn btn-success btn-sm rounded-pill mt-auto fw-semibold shadow-sm px-4 py-2">Pelajari</a>
                    </div>
                </div>
            </div>
            <div class="col-md-4">
                <div class="card h-100 border-0 bg-warning bg-opacity-10 rounded-5 shadow-lg text-center p-4 border-2 border border-warning border-opacity-25">
                    <div class="card-body d-flex flex-column justify-content-center align-items-center pt-5">
                        <div class="rounded-pill bg-warning shadow-sm p-4 text-success display-5 mb-4">
                            <i class="bi bi-alarm-fill"></i>
                        </div>
                        <h3 class="fw-bolder text-success mb-3">Waktu Salat</h3>
                        <p class="text-secondary mb-4 px-3">Pantau waktu Salat 5 waktu dan Imsak untuk area Jakarta & sekitarnya.</p>
                        <a href="#" class="btn btn-warning rounded-pill mt-auto fw-bolder shadow-sm px-4 py-2 text-success">Lihat Jadwal</a>
                    </div>
                </div>
            </div>
            <div class="col-md-4">
                <div class="card h-100 border-0 bg-white rounded-5 shadow-lg text-center p-4">
                    <div class="card-body d-flex flex-column justify-content-center align-items-center pt-5">
                        <div class="rounded-pill bg-success bg-opacity-10 border border-success border-opacity-10 shadow-sm p-4 text-success display-5 mb-4">
                            <i class="bi bi-wallet2"></i>
                        </div>
                        <h3 class="fw-bolder text-success mb-3">Donasi & Zakat</h3>
                        <p class="text-secondary mb-4 px-3">Salurkan zakat fitrah dan sedekahmu dengan mudah dan transparan.</p>
                        <a href="#" class="btn btn-success btn-sm rounded-pill mt-auto fw-semibold shadow-sm px-4 py-2">Bantu Sesama</a>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <div class="container mb-5 pb-5">
        <div class="bg-white rounded-pill shadow-lg p-5 d-flex flex-column flex-md-row align-items-center justify-content-between border border-success border-opacity-10">
            <div class="ms-md-4 text-center text-md-start mb-4 mb-md-0">
                <h2 class="fw-bolder text-success mb-1">Dapatkan Notifikasi Jadwal</h2>
                <p class="mb-0 text-secondary fs-5">Jangan terlewat waktu sahur dan berbuka puasa.</p>
            </div>
            <button class="btn btn-warning btn-lg rounded-pill fw-bolder shadow-sm px-5 py-3 me-md-4 text-success">
                <i class="bi bi-bell-fill me-2"></i>Aktifkan Alarm
            </button>
        </div>
    </div>

    <footer class="bg-success text-white text-center py-5 rounded-top-5 shadow-lg">
        <div class="container mt-4 mb-3">
            <h4 class="fw-bold text-warning mb-2">
                <i class="bi bi-moon-stars-fill me-2 fs-5"></i>RamadanKareem
            </h4>
            <p class="mb-3 text-white-50 fw-light">Coded with <i class="bi bi-heart-fill text-warning mx-1"></i> using 100% Bootstrap 5.</p>
            
            <p class="mt-4 mb-0 fw-lighter fs-7 text-white text-opacity-75 tracking-wider">
                &copy; 2026 Edisi Suci | <span class="fw-bold">Designed & Coded By Arsya</span>
            </p>
        </div>
    </footer>

    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
```

Output:
<img width="1883" height="994" alt="ramadhan" src="https://github.com/user-attachments/assets/68c42da0-ae38-4aee-b148-f5d155019a47" />


# Penjelasan
Program ini dibuat menggunakan HTML dengan bantuan framework Bootstrap untuk menghasilkan tampilan halaman web bertema Ramadan yang modern dan estetik. Seluruh desain memanfaatkan class bawaan Bootstrap seperti layout, warna, dan komponen, sehingga tidak memerlukan banyak CSS tambahan.

Pada bagian awal, terdapat elemen <head> yang berisi metadata serta link ke Bootstrap dan Bootstrap Icons melalui CDN. Hal ini memungkinkan penggunaan berbagai komponen siap pakai seperti navbar, card, button, dan icon secara langsung.

Di bagian <body>, pertama terdapat badge kecil di pojok kanan atas yang berfungsi sebagai identitas pembuat. Badge ini dibuat menggunakan class Bootstrap seperti badge, rounded-pill, dan shadow-sm sehingga tampil ringan dan elegan.

Selanjutnya terdapat navbar yang menggunakan class seperti navbar, bg-white, dan rounded-pill. Navbar ini berisi logo, menu navigasi, serta tombol login. Penggunaan class Bootstrap membuat navbar terlihat modern tanpa perlu styling tambahan yang rumit.

Bagian utama halaman adalah hero section yang menggunakan container dengan background hijau (bg-success) dan efek gradasi. Pada bagian ini ditampilkan judul besar “Marhaban Ya Ramadan”, deskripsi singkat, serta dua tombol aksi. Elemen dekoratif seperti icon lampion dan bulan ditambahkan menggunakan Bootstrap Icons dengan posisi absolut untuk memberikan kesan visual yang lebih menarik.

Setelah itu, terdapat section berisi tiga card yang menjelaskan fitur utama seperti panduan puasa, waktu salat, dan donasi. Card dibuat menggunakan class card, shadow, dan rounded-5 sehingga tampil lebih halus dan tidak kaku. Setiap card juga dilengkapi icon, judul, deskripsi, dan tombol untuk memperjelas fungsi masing-masing.

Di bawahnya terdapat section notifikasi yang berbentuk horizontal dengan desain menyerupai pill. Bagian ini berisi ajakan untuk mengaktifkan pengingat jadwal, dengan tombol aksi di sebelah kanan. Layout dibuat menggunakan flexbox Bootstrap sehingga tetap rapi di berbagai ukuran layar.

Terakhir, bagian footer digunakan sebagai penutup halaman yang berisi nama website, deskripsi singkat, serta credit pembuat. Warna hijau tetap digunakan agar konsisten dengan tema Ramadan.

Secara keseluruhan, program ini menunjukkan bahwa dengan memanfaatkan Bootstrap secara maksimal, kita bisa membuat tampilan website yang rapi, responsif, dan menarik tanpa harus banyak menulis CSS sendiri. Struktur layout yang jelas serta penggunaan komponen yang tepat membuat halaman ini terlihat seperti website modern yang profesional.
