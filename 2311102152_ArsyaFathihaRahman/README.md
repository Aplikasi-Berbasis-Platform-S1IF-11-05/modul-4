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
    <title>Ramadan Kareem</title>

    <!-- Bootstrap -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet">
</head>

<body class="bg-dark text-light">

    <!-- Navbar -->
    <nav class="navbar navbar-dark bg-success shadow">
        <div class="container">
            <span class="navbar-brand fw-bold">🌙 Ramadan Kareem</span>
        </div>
    </nav>

    <!-- Hero -->
    <div class="container text-center py-5">
        <h1 class="display-4 fw-bold text-warning">Selamat Menjalankan Ibadah Puasa</h1>
        <p class="lead">
            Semoga Ramadan ini membawa ketenangan, keberkahan, dan hati yang lebih baik.
        </p>
    </div>

    <!-- Card Section -->
    <div class="container pb-5">
        <div class="row g-4">

            <div class="col-md-4">
                <div class="card bg-success text-light shadow h-100 text-center">
                    <div class="card-body">
                        <h5 class="card-title">🌙 Sahur</h5>
                        <p class="card-text">
                            Memulai hari dengan niat dan energi untuk beribadah.
                        </p>
                    </div>
                </div>
            </div>

            <div class="col-md-4">
                <div class="card bg-warning text-dark shadow h-100 text-center">
                    <div class="card-body">
                        <h5 class="card-title">🕌 Ibadah</h5>
                        <p class="card-text">
                            Memperbanyak doa dan mendekatkan diri kepada Tuhan.
                        </p>
                    </div>
                </div>
            </div>

            <div class="col-md-4">
                <div class="card bg-success text-light shadow h-100 text-center">
                    <div class="card-body">
                        <h5 class="card-title">🍽️ Berbuka</h5>
                        <p class="card-text">
                            Menikmati waktu berbuka dengan penuh rasa syukur.
                        </p>
                    </div>
                </div>
            </div>

        </div>
    </div>

    <!-- Ornamen -->
    <div class="container text-center py-4">
        <div class="d-flex justify-content-center gap-4 fs-1">
            <span>🌙</span>
            <span>⭐</span>
            <span>🕌</span>
            <span>✨</span>
        </div>
    </div>

    <!-- Footer -->
    <footer class="bg-success text-center py-3">
        <p class="mb-0">✨ Ramadan Mubarak ✨</p>
    </footer>

</body>
</html>
```

Output:

# Penjelasan
Program ini dibuat menggunakan HTML dengan bantuan framework Bootstrap untuk menghasilkan tampilan halaman web bertema Ramadan. Struktur utama terdiri dari beberapa bagian yaitu navbar, bagian pembuka (hero), konten utama, ornamen, dan footer.

Pada bagian navbar digunakan class bawaan Bootstrap seperti navbar dan bg-success untuk menampilkan header dengan warna hijau yang identik dengan nuansa Islami. Selanjutnya, bagian hero digunakan untuk menampilkan judul utama dan deskripsi menggunakan class seperti display-4, fw-bold, dan text-warning agar terlihat menonjol.

Bagian konten utama menggunakan sistem grid Bootstrap yaitu row dan col-md-4 untuk membagi tampilan menjadi tiga kolom. Di dalamnya terdapat komponen card yang digunakan untuk menampilkan informasi terkait aktivitas selama Ramadan seperti sahur, ibadah, dan berbuka. Setiap card memanfaatkan class bawaan seperti bg-success, bg-warning, dan shadow untuk memberikan variasi warna dan efek visual.

Selain itu, ditambahkan juga ornamen berupa emoji yang disusun menggunakan d-flex dan gap agar tampil rapi di tengah halaman. Bagian footer menggunakan class bg-success untuk menjaga konsistensi warna dengan bagian navbar.

Secara keseluruhan, penggunaan Bootstrap pada program ini mempermudah dalam membangun tampilan yang rapi, responsif, dan menarik tanpa perlu menambahkan CSS secara manual. Desain yang dihasilkan tetap sesuai dengan tema Ramadan melalui pemilihan warna dan elemen visual yang digunakan.
