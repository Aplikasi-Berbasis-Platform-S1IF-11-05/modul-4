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
    <strong>Sya'bananta Faqih M Lizbar</strong>
    <br>
    <strong>2311102097</strong>
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

## Pengertian Bootstrap
Bootstrap adalah framework CSS (dan JavaScript) open-source yang digunakan untuk membangun antarmuka website yang responsive, cepat, dan konsisten. Bootstrap menyediakan kumpulan class siap pakai seperti layout grid, typography, button, form, dan komponen UI lainnya sehingga developer tidak perlu menulis CSS dari nol.

Bootstrap merupakan framework front-end yang dikembangkan untuk mempermudah proses pembuatan tampilan website yang responsif dan mobile-first. Dengan menggunakan sistem grid berbasis 12 kolom serta berbagai komponen siap pakai seperti navbar, card, button, dan alert, Bootstrap memungkinkan pengembang untuk membangun antarmuka pengguna secara cepat dan konsisten tanpa harus menulis banyak kode CSS secara manual. Selain itu, Bootstrap juga mendukung kompatibilitas lintas browser dan menyediakan utilitas class untuk pengaturan layout, warna, dan spacing.

## Contoh Implementasi
```html
<button class="btn btn-primary">Klik Saya</button>
```

### Source code - html
```html
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <title>Ramadan Kareem 🌙</title>

    <!-- Bootstrap CDN -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body class="bg-dark text-light">

<!-- NAVBAR -->
<nav class="navbar navbar-expand-lg navbar-dark bg-success">
    <div class="container">
        <a class="navbar-brand" href="#">Ramadan Mubarak 🌙</a>
    </div>
</nav>

<!-- HERO -->
<div class="container text-center mt-5">
    <h1 class="display-4 fw-bold text-warning">Marhaban Ya Ramadan ✨</h1>
    <p class="lead">
        Semoga Ramadan kali ini penuh berkah, ampunan, dan rezeki yang melimpah 🤲
    </p>
    <button class="btn btn-warning btn-lg">Aamiin 🤍</button>
</div>

<!-- CARD SECTION -->
<div class="container mt-5">
    <div class="row g-4">

        <!-- Card 1 -->
        <div class="col-md-4">
            <div class="card text-dark">
                <div class="card-body text-center">
                    <h5 class="card-title">Puasa</h5>
                    <p class="card-text">
                        Menahan lapar dan hawa nafsu dari subuh hingga maghrib.
                    </p>
                    <button class="btn btn-success">Semangat 💪</button>
                </div>
            </div>
        </div>

        <!-- Card 2 -->
        <div class="col-md-4">
            <div class="card text-dark">
                <div class="card-body text-center">
                    <h5 class="card-title">Tarawih</h5>
                    <p class="card-text">
                        Sholat malam untuk menambah pahala di bulan suci.
                    </p>
                    <button class="btn btn-success">Gas Masjid 🕌</button>
                </div>
            </div>
        </div>

        <!-- Card 3 -->
        <div class="col-md-4">
            <div class="card text-dark">
                <div class="card-body text-center">
                    <h5 class="card-title">Sedekah</h5>
                    <p class="card-text">
                        Berbagi dengan sesama untuk keberkahan hidup.
                    </p>
                    <button class="btn btn-success">Berbagi ❤️</button>
                </div>
            </div>
        </div>

    </div>
</div>

<!-- FOOTER -->
<footer class="text-center mt-5 mb-3">
    <p class="text-secondary">Selamat menjalankan ibadah puasa 🌙</p>
</footer>

</body>
</html>
```

Output:
<img src="Screenshot (1194).png" alt="preview" style="width:100%; max-width:900px;">

## Penjelasan
Halaman ini dibuat menggunakan Bootstrap dengan memanfaatkan class bawaan seperti navbar, container, card, dan btn untuk membangun tampilan Ramadan yang responsif tanpa CSS custom. Struktur layout menggunakan sistem grid Bootstrap sehingga desain tetap rapi dan konsisten di berbagai ukuran layar.
