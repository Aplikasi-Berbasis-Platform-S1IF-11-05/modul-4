<div align="center">
  <br />
  <h1>LAPORAN PRAKTIKUM <br> APLIKASI BERBASIS PLATFORM </h1>
  <br />
  <h3>MODUL 4 <br> BOOTSTRAP </h3>
  <br />
  <img width="512" height="512" alt="telyu" src="https://github.com/user-attachments/assets/724a3291-bcf9-448d-a395-3886a8659d79" />
  <br />
  <br />
  <br />
  <h3>Disusun Oleh :</h3>
  <p>
    <strong>Rakha Yudhistira</strong>
    <br>
    <strong>2311102010</strong>
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

<p align="justify">
Bootstrap adalah framework open-source berbasis HTML, CSS, dan JavaScript yang digunakan untuk membangun antarmuka web responsif secara cepat. Mengusung konsep mobile-first, framework ini mengandalkan sistem grid 12 kolom untuk mengatur tata letak agar otomatis menyesuaikan berbagai ukuran layar.

Pada versi terbarunya, Bootstrap 5 beralih sepenuhnya ke JavaScript murni dan mengedepankan penggunaan utility classes. Fitur ini memungkinkan pengembang mengatur desain seperti spacing, warna, dan flexbox langsung melalui atribut class di HTML tanpa perlu menulis CSS kustom. Hal ini menjamin efisiensi kerja serta hasil tampilan yang konsisten dan modern.
</p>


# Source Code HTML
```
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ramadan Hub - Mode Suci</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.11.0/font/bootstrap-icons.css">
</head>
<body class="bg-light">

    <nav class="navbar navbar-expand-lg navbar-dark bg-success shadow-sm sticky-top">
        <div class="container">
            <a class="navbar-brand fw-bold" href="#"><i class="bi bi-moon-stars-fill me-2"></i>Ramadan Hub</a>
            <button class="navbar-toggler border-0" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav ms-auto text-uppercase fw-semibold" style="font-size: 0.9rem;">
                    <li class="nav-item px-2"><a class="nav-link active" href="#">Beranda</a></li>
                    <li class="nav-item px-2"><a class="nav-link" href="#jadwal">Jadwal Sholat</a></li>
                    <li class="nav-item px-2"><a class="nav-link" href="#tadarus">Tadarus</a></li>
                    <li class="nav-item px-2"><a class="nav-link" href="#kebaikan">Kebaikan</a></li>
                </ul>
            </div>
        </div>
    </nav>

    <header class="bg-white py-5 border-bottom">
        <div class="container">
            <div class="row align-items-center g-5">
                <div class="col-lg-7 text-center text-lg-start">
                    <span class="badge bg-success-subtle text-success rounded-pill px-3 py-2 mb-3 fw-bold">Ramadan 1447 H</span>
                    <h1 class="display-4 fw-bold text-dark mb-3">Sempurnakan Ibadah di <span class="text-success">Bulan Suci</span></h1>
                    <p class="lead text-secondary mb-4">Satu aplikasi untuk memantau jadwal sholat, target tadarus, dan penyaluran zakat Anda dengan lebih mudah.</p>
                    <div class="d-grid gap-2 d-md-flex justify-content-md-start">
                        <a href="#tadarus" class="btn btn-success btn-lg px-5 rounded-pill shadow-sm">Mulai Tadarus</a>
                        <a href="#jadwal" class="btn btn-outline-success btn-lg px-4 rounded-pill">Lihat Jadwal</a>
                    </div>
                </div>
                <div class="col-lg-5 text-center">
                    <img src="https://www.shutterstock.com/image-photo/samarinda-indonesia-march-21-2023-600nw-2279299667.jpg" 
                         class="img-fluid rounded-5 shadow-lg w-75 border border-5 border-white" 
                         alt="Ramadan Image">
                </div>
            </div>
        </div>
    </header>

    <main class="container py-5">
        
        <section id="jadwal" class="mb-5 py-4">
            <div class="row align-items-center mb-4">
                <div class="col-auto"><i class="bi bi-clock-fill text-success fs-2"></i></div>
                <div class="col"><h3 class="fw-bold mb-0">Jadwal Sholat Hari Ini</h3></div>
            </div>
            <div class="row g-3">
                <div class="col-6 col-md-4 col-lg-2">
                    <div class="card border-0 shadow-sm text-center p-3 rounded-4 bg-white">
                        <small class="text-muted fw-bold">SUBUH</small>
                        <h4 class="text-success mb-0">04:35</h4>
                    </div>
                </div>
                <div class="col-6 col-md-4 col-lg-2">
                    <div class="card border-0 shadow-sm text-center p-3 rounded-4 bg-white">
                        <small class="text-muted fw-bold">DZUHUR</small>
                        <h4 class="text-success mb-0">11:54</h4>
                    </div>
                </div>
                <div class="col-6 col-md-4 col-lg-2">
                    <div class="card border-0 shadow-sm text-center p-3 rounded-4 bg-white">
                        <small class="text-muted fw-bold">ASHAR</small>
                        <h4 class="text-success mb-0">15:10</h4>
                    </div>
                </div>
                <div class="col-6 col-md-4 col-lg-2">
                    <div class="card border-0 shadow-sm text-center p-3 rounded-4 bg-success text-white">
                        <small class="opacity-75 fw-bold">MAGHRIB</small>
                        <h4 class="mb-0">17:56</h4>
                    </div>
                </div>
                <div class="col-6 col-md-4 col-lg-2">
                    <div class="card border-0 shadow-sm text-center p-3 rounded-4 bg-white">
                        <small class="text-muted fw-bold">ISYA</small>
                        <h4 class="text-success mb-0">19:05</h4>
                    </div>
                </div>
                <div class="col-6 col-md-4 col-lg-2">
                    <div class="card border-0 shadow-sm text-center p-3 rounded-4 bg-white border-start border-success border-4">
                        <small class="text-muted fw-bold">IMSAK</small>
                        <h4 class="text-danger mb-0">04:25</h4>
                    </div>
                </div>
            </div>
        </section>

        <hr class="my-5 opacity-25">

        <section id="tadarus" class="mb-5 py-4">
            <div class="row align-items-center mb-4 text-center text-md-start">
                <div class="col-md-8">
                    <h3 class="fw-bold"><i class="bi bi-book-half text-success me-2"></i>Progres Tadarus</h3>
                    <p class="text-muted">Target harian: Menyelesaikan 1 Juz per malam.</p>
                </div>
                <div class="col-md-4 text-md-end">
                    <button class="btn btn-sm btn-success rounded-pill px-3">+ Catat Progress</button>
                </div>
            </div>
            
            <div class="row g-4">
                <div class="col-lg-4">
                    <div class="card border-0 shadow-sm rounded-4 p-4 h-100 bg-white">
                        <h5 class="fw-bold mb-4">Statistik</h5>
                        <div class="d-flex align-items-center mb-3">
                            <h2 class="display-5 fw-bold text-success mb-0 me-3">20%</h2>
                            <div class="flex-grow-1">
                                <div class="progress" style="height: 10px;">
                                    <div class="progress-bar bg-success" style="width: 20%"></div>
                                </div>
                            </div>
                        </div>
                        <p class="small text-muted mb-0">6 dari 30 Juz telah diselesaikan. Masih ada 24 Juz lagi menuju khatam!</p>
                    </div>
                </div>
                <div class="col-lg-8">
                    <div class="card border-0 shadow-sm rounded-4 overflow-hidden">
                        <table class="table table-hover mb-0 align-middle">
                            <thead class="table-light">
                                <tr class="small text-uppercase">
                                    <th class="ps-4 py-3">Hari</th>
                                    <th>Target Juz</th>
                                    <th>Status</th>
                                    <th class="pe-4 text-end">Aksi</th>
                                </tr>
                            </thead>
                            <tbody>
                                <tr>
                                    <td class="ps-4 fw-bold">Day 6</td>
                                    <td>Juz 6 (Al-Ma'idah)</td>
                                    <td><span class="badge bg-warning text-dark px-3 rounded-pill">Sedang Baca</span></td>
                                    <td class="pe-4 text-end"><button class="btn btn-sm btn-outline-success border-0"><i class="bi bi-check-circle-fill"></i> Selesai</button></td>
                                </tr>
                                <tr>
                                    <td class="ps-4 fw-bold">Day 7</td>
                                    <td>Juz 7 (Al-An'am)</td>
                                    <td><span class="badge bg-light text-muted border px-3 rounded-pill">Nanti Malam</span></td>
                                    <td class="pe-4 text-end"><button class="btn btn-sm btn-light text-muted border-0"><i class="bi bi-circle"></i> Tandai</button></td>
                                </tr>
                            </tbody>
                        </table>
                    </div>
                </div>
            </div>
        </section>

        <hr class="my-5 opacity-25">

        <section id="kebaikan" class="mb-5 py-4">
            <h3 class="fw-bold mb-4 text-center">Pojok Kebaikan</h3>
            <div class="row g-4">
                <div class="col-md-6">
                    <div class="card border-0 shadow-sm rounded-4 p-4 bg-success text-white">
                        <div class="d-flex align-items-center mb-3">
                            <i class="bi bi-heart-fill fs-1 me-3"></i>
                            <h4 class="mb-0 fw-bold">Zakat Fitrah</h4>
                        </div>
                        <p class="opacity-75">Sudahkah Anda membayar zakat? Hitung dan salurkan kewajiban Anda dengan aman di sini.</p>
                        <button class="btn btn-light text-success fw-bold rounded-pill w-100">Bayar Zakat Sekarang</button>
                    </div>
                </div>
                <div class="col-md-6">
                    <div class="card border-0 shadow-sm rounded-4 p-4 bg-white">
                        <div class="d-flex align-items-center mb-3 text-success">
                            <i class="bi bi-gift-fill fs-1 me-3"></i>
                            <h4 class="mb-0 fw-bold text-dark">Sedekah Buka Puasa</h4>
                        </div>
                        <p class="text-muted">Bantu sediakan paket takjil untuk mereka yang membutuhkan di jalanan atau panti asuhan.</p>
                        <button class="btn btn-success rounded-pill w-100">Donasi Takjil</button>
                    </div>
                </div>
            </div>
        </section>

    </main>

    <footer class="bg-dark text-white py-3 mt-2">
        <div class="container text-center">
            <h5 class="fw-bold mb-3">Ramadan Hub</h5>
            <p class="opacity-50 small mb-4">Mari raih keberkahan dengan teknologi yang memudahkan ibadah.</p>
            <p class="mb-0 x-small opacity-25" style="font-size: 0.7rem;">&copy; 2026 Ramadan Digital. Dibuat dengan Bootstrap 5.</p>
        </div>
    </footer>

    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>

```


# Screenshoot Program
![alt text](<assets/Screenshot (705).png>)
![alt text](<assets/Screenshot (706).png>)
![alt text](<assets/Screenshot (707).png>)



# Penjelasan
<p align="justify">

Program Ramadan Hub ini merupakan halaman web statis bertema "Mode Suci" yang dibangun menggunakan Bootstrap 5 secara maksimal melalui koneksi CDN. Program ini dirancang dengan pendekatan utility-first, di mana seluruh tata letak, warna, dan spasi diatur langsung menggunakan class bawaan Bootstrap tanpa menulis kode CSS kustom manual.

Fitur utama dalam program ini meliputi Navbar responsif, Jadwal Sholat harian, Tracker Tadarus untuk memantau progres khatam Al-Qur'an, serta Pojok Kebaikan untuk donasi. Secara teknis, program ini memanfaatkan sistem Grid 12 kolom dan komponen Card untuk menciptakan antarmuka yang bersih, modern, dan adaptif (responsive) saat dibuka di perangkat mobile maupun desktop.
</p>