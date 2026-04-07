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
    <strong>Ben Waiz Pintus Widyosaputro</strong>
    <br>
    <strong>2311102169</strong>
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
Pemanfaatan framework Bootstrap sebagai alat bantu dalam pengembangan antarmuka web yang cepat, konsisten, dan responsif. Bootstrap merupakan framework front-end berbasis CSS dan JavaScript yang menyediakan kumpulan class dan komponen siap pakai seperti navbar, card, button, serta sistem grid. Dengan adanya Bootstrap, pengembang tidak perlu membuat styling dari awal karena hampir seluruh kebutuhan tampilan sudah disediakan dalam bentuk class yang dapat langsung digunakan pada elemen HTML. Hal ini mempercepat proses pengembangan serta memastikan desain yang lebih rapi dan terstandarisasi.
</p>

<p align="justify">
Selain itu, Bootstrap juga menerapkan konsep responsive design melalui sistem grid yang fleksibel, seperti penggunaan container, row, dan col untuk mengatur tata letak halaman agar dapat menyesuaikan berbagai ukuran layar, baik desktop maupun mobile. Framework ini juga menyediakan utility class untuk mengatur warna, margin, padding, dan tipografi secara praktis tanpa perlu menulis CSS tambahan. Dalam konteks desain, penggunaan Bootstrap membantu meningkatkan aspek UI (User Interface) dan UX (User Experience) karena komponen yang digunakan sudah dirancang agar mudah digunakan, konsisten, dan nyaman bagi pengguna. Dengan demikian, Bootstrap menjadi solusi efektif dalam membangun tampilan web modern secara efisien dan terstruktur.
</p>

# Tugas 4 - Mode Suci (Edisi Ramadan)
## 1. Source code index.html
```
<!-- 2311102169
Ben Waiz Pintus W
S1IF-11-05 -->
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <title>Mode Suci Ramadan 🌙</title>

    <!-- Bootstrap CDN -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body class="bg-success bg-gradient text-light">

    <!-- Navbar -->
    <nav class="navbar navbar-expand-lg navbar-dark bg-dark shadow">
        <div class="container">
            <a class="navbar-brand fw-bold" href="#">🌙 Ramadan Kareem</a>
        </div>
    </nav>

    <!-- Content -->
    <div class="container text-center mt-5">

        <h1 class="fw-bold mb-3">Selamat Menjalankan Ibadah Puasa</h1>
        <p class="lead mb-4">
            Semoga Ramadan kali ini membawa berkah, ampunan, dan kedamaian 🌙✨
        </p>

        <!-- Card -->
        <div class="card mx-auto shadow-lg" style="max-width: 400px;">
            <div class="card-body text-dark">
                <h5 class="card-title">Untuk Kamu ❤️</h5>
                <p class="card-text">
                    Di bulan penuh berkah ini, aku cuma mau bilang...<br>
                    Semoga kita selalu diberi kesehatan,<br>
                    dan tetap saling menjaga satu sama lain 🤍
                </p>
                <a href="#" class="btn btn-success w-100">Aamiin 🤲</a>
            </div>
        </div>

        <!-- Extra Section -->
        <div class="row mt-5">
            <div class="col-md-4 mb-3">
                <div class="card text-dark shadow">
                    <div class="card-body">
                        <h5 class="card-title">🌙 Puasa</h5>
                        <p class="card-text">Menahan diri dari lapar dan hawa nafsu.</p>
                    </div>
                </div>
            </div>

            <div class="col-md-4 mb-3">
                <div class="card text-dark shadow">
                    <div class="card-body">
                        <h5 class="card-title">🕌 Tarawih</h5>
                        <p class="card-text">Sholat malam untuk mendekatkan diri.</p>
                    </div>
                </div>
            </div>

            <div class="col-md-4 mb-3">
                <div class="card text-dark shadow">
                    <div class="card-body">
                        <h5 class="card-title">🤲 Doa</h5>
                        <p class="card-text">Waktu terbaik untuk memohon ampunan.</p>
                    </div>
                </div>
            </div>
        </div>

    </div>

    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>

</body>
</html>
```

# Output
![alt text](<p1.png>)

# Penjelasan
<p align="justify">
Program ini dibuat menggunakan framework Bootstrap untuk membangun tampilan halaman bertema Ramadan tanpa menggunakan CSS tambahan. Pada bagian head, Bootstrap dihubungkan melalui CDN sehingga seluruh class bawaan dapat langsung digunakan. Di dalam body, digunakan class seperti bg-success, bg-gradient, dan text-light untuk memberikan tampilan latar belakang hijau dengan nuansa Ramadan serta teks yang kontras agar mudah dibaca.

Struktur halaman diawali dengan komponen navbar menggunakan class navbar, navbar-expand-lg, dan navbar-dark bg-dark yang berfungsi sebagai header. Selanjutnya, konten utama dibungkus dalam container dengan tambahan class seperti text-center, mt-5, dan mb-4 untuk mengatur posisi dan jarak antar elemen. Komponen card digunakan untuk menampilkan pesan utama dengan tampilan yang rapi, sedangkan sistem grid Bootstrap yaitu row dan col-md-4 dimanfaatkan untuk membagi konten menjadi beberapa bagian yang responsif. Tombol dibuat menggunakan class btn btn-success w-100 agar sesuai dengan tema dan mudah digunakan. Dengan memanfaatkan class Bootstrap secara maksimal, tampilan halaman menjadi lebih cepat dibuat, konsisten, dan responsif tanpa perlu styling manual.
</p>