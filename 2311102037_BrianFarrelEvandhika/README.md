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
    <strong>Brian Farrel Evandhika</strong>
    <br>
    <strong>2311102037</strong>
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

# Dasar Teori Bootstrap

<p align="justify">
Bootstrap dikategorikan sebagai salah satu kerangka kerja (framework) front-end CSS yang paling tepercaya di dunia pengembangan web untuk membangun antarmuka yang modern dan adaptif secara cepat. Inti dari Bootstrap adalah koleksi ekstensif komponen berbasis HTML, CSS, dan JavaScript yang meliputi sistem navigasi, tombol, formulir, hingga tata letak kartu yang siap pakai. Hal ini memungkinkan developer untuk menciptakan situs web berkualitas tinggi tanpa harus membangun setiap elemen visual secara manual.
</p>

<p align="justify">
Salah satu pilar utama Bootstrap adalah sistem grid 12 kolom yang fleksibel dan pendekatan "mobile-first", yang menjamin bahwa setiap elemen halaman akan menyesuaikan diri secara elegan pada berbagai resolusi layar, baik itu smartphone maupun monitor desktop. Selain komponen visual, Bootstrap juga menyediakan berbagai utility classes untuk memanipulasi margin, padding, tipografi, dan warna secara instan langsung dari tag HTML. Pendekatan ini tidak hanya mempercepat waktu produksi, tetapi juga memastikan struktur kode tetap bersih, konsisten, dan mudah dipelihara.
</p>



## Task 4: Mode Suci (Edisi Ramadan)
### Source Code - HTML
```html
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ramadan Kareem - 2311102037</title>
    <!-- Bootstrap 5 CSS -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
    <!-- FontAwesome for Icons -->
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css" rel="stylesheet">
    <!-- Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600;800&family=Playfair+Display:ital,wght@0,400;0,700;1,400&display=swap" rel="stylesheet">
    <style>
        body { font-family: 'Outfit', sans-serif; background-color: #f8f9fa; }
        .header-font { font-family: 'Playfair Display', serif; }
        .ramadan-gradient { background: linear-gradient(135deg, #064e3b, #059669, #10b981); }
    </style>
</head>
<body class="bg-light">

    <nav class="navbar navbar-expand-lg navbar-dark bg-dark sticky-top shadow-sm">
        <div class="container">
            <a class="navbar-brand header-font fw-bold" href="#">
                <i class="fas fa-moon me-2 text-success"></i>Ramadan Kareem
            </a>
            <button class="navbar-toggler border-0" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav ms-auto text-uppercase small fw-semibold">
                    <li class="nav-item"><a class="nav-link px-3" href="#home">Beranda</a></li>
                    <li class="nav-item"><a class="nav-link px-3" href="#jadwal">Jadwal</a></li>
                    <li class="nav-item"><a class="nav-link px-3" href="#keutamaan">Keutamaan</a></li>
                    <li class="nav-item"><a class="nav-link px-3 btn btn-success text-white ms-lg-3 rounded-pill" href="#">Daftar Mualaf</a></li>
                </ul>
            </div>
        </div>
    </nav>

    <header id="home" class="ramadan-gradient text-white py-5 mb-5 shadow">
        <div class="container py-5 text-center">
            <div class="row justify-content-center py-5">
                <div class="col-lg-8">
                    <div class="mb-4">
                        <div class="ketupat-wrapper"><span class="ketupat"></span><div class="ketupat-tail"></div></div>
                        <div class="ketupat-wrapper"><span class="ketupat"></span><div class="ketupat-tail"></div></div>
                        <div class="ketupat-wrapper"><span class="ketupat"></span><div class="ketupat-tail"></div></div>
                    </div>
                    <h5 class="text-uppercase tracking-widest text-white mb-3 fw-bold shadow-sm">Selamat Datang di Bulan Suci</h5>
                    <h1 class="display-2 header-font fw-bold mb-4">Marhaban Ya Ramadan</h1>
                    <p class="lead mb-5 opacity-75">Bulan penuh berkah, rahmat, dan ampunan. Mari perbanyak ibadah dan raih kemenangan di hari yang fitri.</p>
                </div>
            </div>
        </div>
    </header>

    <main class="container py-5">
        <div class="row g-4 mb-5 text-center">
            <div class="col-md-3">
                <div class="card h-100 border-0 shadow-sm p-4 rounded-4">
                    <div class="display-6 text-primary mb-2"><i class="fas fa-clock"></i></div>
                    <h4 class="fw-bold mb-1">04:30</h4>
                    <p class="text-muted small mb-0">Imsak (Jakarta)</p>
                </div>
            </div>
            <!-- Additional Cards for Prayer Times -->
        </div>
    </main>

    <footer class="bg-dark text-light py-5 mt-5">
        <div class="container text-center">
            <p class="mb-2">&copy; 2026 Ramadan Kareem Application. All Rights Reserved.</p>
            <div class="badge bg-success border border-light p-2 mb-4">
                <i class="fas fa-id-card me-2"></i>2311102037_Brian Farrel Evandhika
            </div>
        </div>
    </footer>

    <style>
        .hover-shadow { transition: all 0.3s ease; }
        .hover-shadow:hover { 
            transform: translateY(-10px);
            box-shadow: 0 1rem 3rem rgba(0,0,0,0.1) !important;
        }
        .ketupat {
            width: 25px; height: 25px;
            background: #198754; border: 2px solid #fff;
            transform: rotate(45deg); margin: 0 15px;
            display: inline-block; position: relative;
        }
        .ketupat-tail {
            position: absolute; width: 2px; height: 15px;
            background: #fff; left: 50%; bottom: -15px;
            transform: translateX(-50%) rotate(-45deg);
        }
    </style>
</body>
</html>
```
### Screenshots Output
<img src="ss-modul4.png" alt="preview" style="width:100%; max-width:900px;">

# Penjelasan Program
<p align="justify">
Aplikasi berbasis web ini merupakan sebuah perwujudan tema Ramadan yang memadukan keindahan visual dengan performa yang optimal melalui framework Bootstrap 5. Secara arsitektural, halaman ini menggunakan sistem navigasi yang lengket di bagian atas (<i>sticky-top</i>) dan latar belakang gradien hijau emerald yang mendalam untuk menciptakan suasana spiritual yang tenang. Salah satu elemen estetika yang menonjol adalah hiasan ornamen ketupat yang dirancang sedemikian rupa menggunakan murni manipulasi CSS, sehingga situs tetap ringan tanpa perlu memuat file gambar eksternal.
</p>

<p align="justify">
Untuk menyajikan informasi secara terstruktur, proyek ini memanfaatkan komponen kartu (<i>card</i>) Bootstrap untuk menampilkan ringkasan waktu ibadah harian serta kolom edukatif mengenai keutamaan bulan suci. Seluruh elemen tata letak dikelola menggunakan sistem grid Bootstrap yang responsif, memastikan aksesibilitas yang sempurna baik saat diakses melalui perangkat seluler maupun komputer meja. Penggunaan utility classes untuk bayangan halus (<i>shadow</i>) dan sudut membulat (<i>rounded-4</i>) turut memberikan sentuhan desain yang premium dan modern pada keseluruhan antarmuka.
</p>