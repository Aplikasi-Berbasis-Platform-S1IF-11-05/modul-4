<div align="center">
  <br />
  <h1>LAPORAN PRAKTIKUM <br> APLIKASI BERBASIS PLATFORM </h1>
  <br />
  <h3>MODUL 4 <br> CSS </h3>
  <br />
  <img width="512" height="512" alt="telyu" src="https://github.com/user-attachments/assets/724a3291-bcf9-448d-a395-3886a8659d79" />
  <br />
  <br />
  <br />
  <h3>Disusun Oleh :</h3>
  <p>
    <strong>Amelia Azmi</strong>
    <br>
    <strong>2311102135</strong>
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

CSS (Cascading Style Sheets) adalah bahasa yang digunakan untuk mengatur tampilan sebuah halaman web agar terlihat lebih menarik dan rapi. Dengan CSS, kita bisa mengubah berbagai aspek visual seperti warna, ukuran teks, jarak antar elemen, hingga tata letak halaman.

Secara sederhana, HTML berfungsi sebagai struktur atau kerangka dari sebuah website, sedangkan CSS berperan dalam memperindah tampilannya. Jadi, tanpa CSS, halaman web hanya akan terlihat polos tanpa desain.

Dalam penggunaannya, CSS bekerja dengan cara memilih elemen HTML tertentu menggunakan selector, lalu memberikan aturan gaya (style) pada elemen tersebut. Misalnya, kita bisa mengatur warna teks menjadi merah, menambahkan background, atau mengubah posisi elemen di halaman.

CSS juga memungkinkan kita untuk membuat tampilan yang konsisten di seluruh halaman website. Artinya, kita tidak perlu mengatur satu per satu setiap elemen secara manual, cukup dengan satu aturan CSS saja, banyak elemen bisa langsung mengikuti gaya tersebut.

Bootstrap adalah sebuah framework front-end yang dirancang untuk mempercepat proses pembuatan tampilan website. Framework ini menyediakan kumpulan class siap pakai yang dapat digunakan untuk membangun layout, mengatur responsivitas, serta mempercantik tampilan tanpa harus menulis CSS dari nol.

Konsep utama dari Bootstrap adalah kemudahan dan konsistensi. Dengan menggunakan sistem grid, halaman web dapat dibagi menjadi beberapa kolom yang fleksibel sehingga dapat menyesuaikan berbagai ukuran layar, mulai dari desktop hingga perangkat mobile.


# Tugas 4
## 1. Source Kode HTML
```
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mode Suci Ramadan</title>

    <!-- Bootstrap -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
</head>

<body class="bg-success-subtle text-dark">

    <!-- NAVBAR -->
    <nav class="navbar navbar-expand-lg navbar-dark bg-success shadow">
        <div class="container">
            <a class="navbar-brand fw-bold text-warning" href="#">🌙 Ramadan Mode</a>
        </div>
    </nav>

    <!-- HERO -->
    <div class="container text-center py-5">
        <h1 class="display-4 fw-bold text-success-emphasis">
            ✨ Mode Suci (Edisi Ramadan)
        </h1>
        <p class="lead text-secondary">
            Mari tingkatkan ibadah dan berbagi di bulan penuh berkah
        </p>
        <button class="btn btn-success btn-lg mt-3 shadow">
            Mulai Sekarang
        </button>
    </div>

    <!-- DESKRIPSI -->
    <div class="container mb-5">
        <div class="card shadow border-0">
            <div class="card-body">
                <h4 class="card-title text-success">📖 Deskripsi Tugas</h4>
                <p>
                    Buatlah halaman web bertema <b>Ramadan</b> dengan memanfaatkan 
                    <b>Bootstrap secara maksimal</b>. Pada tugas ini, mahasiswa tidak diperbolehkan 
                    menggunakan CSS custom dan wajib menggunakan class bawaan Bootstrap.
                </p>
            </div>
        </div>
    </div>

    <!-- KETENTUAN -->
    <div class="container mb-5">
        <div class="card border-success shadow">
            <div class="card-body">
                <h4 class="text-success">📌 Ketentuan</h4>
                <ul class="list-group list-group-flush">
                    <li class="list-group-item">Menggunakan class Bootstrap</li>
                    <li class="list-group-item">Tidak menggunakan CSS tambahan</li>
                    <li class="list-group-item">Menggunakan komponen seperti Grid, Card, Button, Navbar</li>
                </ul>
            </div>
        </div>
    </div>

    <!-- FITUR -->
    <div class="container mb-5">
        <div class="row g-4">

            <div class="col-md-4">
                <div class="card text-center shadow h-100 border-success">
                    <div class="card-body">
                        <h5 class="card-title text-success">🌙 Ibadah</h5>
                        <p class="card-text">Pantau ibadah harianmu</p>
                        <button class="btn btn-outline-success">Mulai</button>
                    </div>
                </div>
            </div>

            <div class="col-md-4">
                <div class="card text-center shadow h-100 border-success">
                    <div class="card-body">
                        <h5 class="card-title text-success">⏰ Jadwal</h5>
                        <p class="card-text">Waktu sahur & berbuka</p>
                        <button class="btn btn-outline-success">Cek</button>
                    </div>
                </div>
            </div>

            <div class="col-md-4">
                <div class="card text-center shadow h-100 border-success">
                    <div class="card-body">
                        <h5 class="card-title text-success">💰 Donasi</h5>
                        <p class="card-text">Salurkan zakat & sedekah</p>
                        <button class="btn btn-outline-success">Donasi</button>
                    </div>
                </div>
            </div>

        </div>
    </div>

    <!-- UCAPAN LEBARAN -->
    <div class="container text-center mb-5">
        <div class="alert alert-success fw-bold shadow">
            🌙 Selamat Hari Raya Idul Fitri 1447 H 🌙 <br>
            Mohon Maaf Lahir dan Batin
        </div>
    </div>

    <!-- FOOTER -->
    <footer class="text-center py-4 text-success-emphasis border-top border-success">
        © 2026 Mode Suci Ramadan | Bootstrap Edition
    </footer>

</body>
</html>
```

Output:
<img width="1919" height="939" alt="Screenshot 2026-04-06 025710" src="https://github.com/user-attachments/assets/c9d2dfd4-bb3e-4606-b12a-98bfa53d8af4" />


# Penjelasan
Program ini merupakan halaman web bertema Ramadan yang dibuat menggunakan Bootstrap tanpa menggunakan CSS tambahan. Semua tampilan diatur menggunakan class bawaan Bootstrap.

Bagian awal berisi struktur dasar HTML dan link Bootstrap. Pada bagian body, digunakan warna hijau agar sesuai dengan nuansa Ramadan.

Terdapat navbar sebagai header, kemudian hero section yang menampilkan judul dan tombol utama. Selanjutnya ada bagian deskripsi dan ketentuan yang ditampilkan menggunakan card dan list.

Bagian fitur menggunakan grid Bootstrap yang berisi tiga card, yaitu Ibadah, Jadwal, dan Donasi. Setiap card memiliki tombol aksi.

Di bagian bawah terdapat ucapan Lebaran menggunakan alert, dan terakhir footer sebagai penutup.

Secara keseluruhan, program ini memanfaatkan komponen Bootstrap seperti navbar, card, button, grid, dan alert untuk membuat tampilan yang rapi dan menarik.
