<div align="center">

# LAPORAN PRAKTIKUM

## APLIKASI BERBASIS PLATFORM

---

### MODUL 4

### Instalasi dan Git

<br>

<img src="https://github.com/user-attachments/assets/724a3291-bcf9-448d-a395-3886a8659d79" width="300"/>

<br><br><br>

### Disusun Oleh

**Aryo Tegar Sukarno**  
**2311102018**  
**S1 IF-11-REG05**

<br>

### Dosen Pengampu

**Dedi Agung Prabowo, S.Kom., M.Kom**

<br>

### Asisten Praktikum

Apri Pandu Wicaksono  
Hamka Zaenul Ardi

<br><br>

**LABORATORIUM HIGH PERFORMANCE**  
**FAKULTAS INFORMATIKA**  
**UNIVERSITAS TELKOM PURWOKERTO**  
**2026**

</div>

---

# 📚 Dasar Teori

CSS (Cascading Style Sheets) adalah bahasa stylesheet yang digunakan untuk mengatur tampilan dan desain halaman web yang dibuat menggunakan HTML. CSS berfungsi untuk mengatur warna, ukuran teks, tata letak, jarak antar elemen, animasi, serta tampilan responsif pada berbagai ukuran layar.

Dengan menggunakan CSS, struktur halaman (HTML) dapat dipisahkan dari desain visual sehingga kode menjadi lebih rapi, mudah dikelola, dan konsisten.

CSS dapat digunakan dalam tiga cara:

Inline CSS : langsung di dalam tag HTML
Internal CSS : ditulis pada tag <style> di file HTML
External CSS : menggunakan file .css terpisah

Framework seperti Bootstrap sebenarnya merupakan kumpulan CSS siap pakai yang mempercepat proses desain website.

---

# Tugas 4 — CSS

Task 4: Mode Suci (Edisi Ramadan)
Bikin halaman tema Ramadan. Kalau tadi dilarang pakai library, sekarang kebalikannya, gunain Bootstrap semaksimal mungkin. Dimana buat tampilan wajib gunakan class bawaan dari bootstrap yaa jangan pake styling pure CSS

---

# Source Code

```html
<!-- Aryo Tegar Sukarno - 2311102018 -->

<!-- index.html -->
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Ramadan Kareem · Mode Suci</title>
    <!-- Bootstrap 5 CSS only (no custom style) -->
    <link
      href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/css/bootstrap.min.css"
      rel="stylesheet"
    />
    <!-- optional: bootstrap icons for decoration -->
    <link
      rel="stylesheet"
      href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.11.3/font/bootstrap-icons.min.css"
    />
  </head>
  <body class="bg-dark bg-gradient">
    <!-- navbar ramadan -->
    <nav
      class="navbar navbar-expand-lg bg-success bg-opacity-75 shadow-sm"
      data-bs-theme="dark"
    >
      <div class="container">
        <span class="navbar-brand fs-3"
          ><i class="bi-moon-stars-fill"></i> Ramadan Suci</span
        >
        <div class="ms-auto">
          <span class="text-warning-emphasis fw-semibold"
            ><i class="bi-calendar-heart"></i> 1446 H</span
          >
        </div>
      </div>
    </nav>

    <!-- hero section -->
    <div class="container my-5 py-4 text-center text-white">
      <div class="row justify-content-center">
        <div class="col-lg-8">
          <h1 class="display-3 fw-bold text-warning">🌙 Ramadan Kareem 🌙</h1>
          <p class="lead fs-4 mt-3">
            Bulan penuh ampunan, rahmat, dan berkah. <br />
            Mari tingkatkan ibadah & ketakwaan.
          </p>
          <div class="mt-4">
            <button class="btn btn-outline-warning btn-lg px-4" disabled>
              <i class="bi-gem"></i> 30 Hari Mulia
            </button>
          </div>
        </div>
      </div>
    </div>

    <!-- 3 kartu amalan -->
    <div class="container mb-5">
      <div class="row g-4">
        <div class="col-md-4">
          <div
            class="card h-100 border-warning bg-dark text-white bg-opacity-90"
          >
            <div class="card-body text-center">
              <i class="bi-clock-history fs-1 text-warning"></i>
              <h5 class="card-title mt-3">Sahur & Berkah</h5>
              <p class="card-text">
                Jangan lupakan sahur, karena ada keberkahan di dalamnya.
                Perbanyak doa di sepertiga malam.
              </p>
            </div>
          </div>
        </div>
        <div class="col-md-4">
          <div
            class="card h-100 border-warning bg-dark text-white bg-opacity-90"
          >
            <div class="card-body text-center">
              <i class="bi-book-half fs-1 text-warning"></i>
              <h5 class="card-title mt-3">Tadarus Al-Qur'an</h5>
              <p class="card-text">
                Satu juz per hari, khatamkan Al-Qur'an di bulan mulia ini.
              </p>
            </div>
          </div>
        </div>
        <div class="col-md-4">
          <div
            class="card h-100 border-warning bg-dark text-white bg-opacity-90"
          >
            <div class="card-body text-center">
              <i class="bi-heart-handshake fs-1 text-warning"></i>
              <h5 class="card-title mt-3">Sedekah & Peduli</h5>
              <p class="card-text">
                Lipatgandakan pahala dengan berbagi kepada sesama.
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>

    <!-- jadwal buka puasa ilustrasi -->
    <div class="container text-white mb-5">
      <div class="p-4 rounded-4 bg-success bg-opacity-25 border border-warning">
        <div class="row align-items-center">
          <div class="col-md-8">
            <h3><i class="bi-sunset-fill"></i> Waktu Berbuka & Imsak</h3>
            <p class="mb-0">
              Maghrib: 18:03 WIB · Imsak: 04:25 WIB · Jadwal lengkap di masjid
              terdekat.
            </p>
          </div>
          <div class="col-md-4 text-md-end mt-3 mt-md-0">
            <span class="badge bg-warning text-dark fs-6 p-2"
              ><i class="bi-moon"></i> 10 Jam lagi</span
            >
          </div>
        </div>
      </div>
    </div>

    <!-- footer -->
    <footer class="bg-black bg-opacity-75 text-center text-white-50 py-4 mt-4">
      <p class="mb-0">
        <i class="bi-star-fill text-warning"></i> Mode Suci · Ramadan Penuh
        Berkah <i class="bi-star-fill text-warning"></i>
      </p>
      <small
        >“Ya Allah, berkahi kami di bulan Rajab & Sya'ban, sampaikan kami ke
        Ramadan”</small
      >
    </footer>

    <!-- Bootstrap JS (not used for styling, only optional but included to support potential future interactive) -->
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/js/bootstrap.bundle.min.js"></script>
  </body>
</html>

# Tugas 4 — CSS ![alt text](t4-2.jpeg)
```
