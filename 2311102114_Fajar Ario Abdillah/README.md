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
    <strong>Fajar Ario Abdillah</strong>
    <br>
    <strong>2311102114</strong>
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

Bootstrap adalah framework CSS yang digunakan untuk mempermudah pembuatan tampilan website secara cepat dan responsif tanpa harus menulis CSS dari nol. Bootstrap menyediakan berbagai class siap pakai seperti layout grid, navbar, button, card, form, dan komponen lainnya yang dapat langsung digunakan pada HTML. Dengan menggunakan Bootstrap, developer dapat membuat desain yang rapi, konsisten, dan menyesuaikan berbagai ukuran layar (mobile, tablet, desktop) hanya dengan memanfaatkan class bawaan tanpa perlu banyak styling manual.

---

## 2. Cara Menggunakan Bootstrap

Bootstrap dapat digunakan dengan cara menambahkan link CDN (Content Delivery Network) ke dalam file HTML. Dengan menggunakan CDN, kita tidak perlu mengunduh file Bootstrap secara manual karena sudah tersedia secara online. Setelah itu, kita bisa langsung menggunakan class bawaan Bootstrap pada elemen HTML untuk membuat tampilan yang menarik dan responsif.

---

### Langkah-langkah Menggunakan Bootstrap

1. Tambahkan link Bootstrap pada bagian `<head>` HTML:

```html
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
```

2. Tambahkan script Bootstrap sebelum penutup `</body>`:

```html
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
```

3. Gunakan class Bootstrap langsung pada elemen HTML.

### Contoh Penggunaan Bootstrap

```html
<!DOCTYPE html>
<html>
<head>
  <title>Contoh Bootstrap</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>

<div class="container mt-5">
  <h1 class="text-center text-primary">Hello Bootstrap</h1>

  <button class="btn btn-success mt-3">Klik Saya</button>

  <div class="card mt-4" style="width: 18rem;">
    <div class="card-body">
      <h5 class="card-title">Contoh Card</h5>
      <p class="card-text">Ini adalah contoh penggunaan card pada Bootstrap.</p>
      <a href="#" class="btn btn-primary">Selengkapnya</a>
    </div>
  </div>
</div>

</body>
</html>
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
Navbar digunakan sebagai menu navigasi pada bagian atas website.

```html
<nav class="navbar navbar-expand-lg navbar-dark bg-dark">
  <div class="container">
    <a class="navbar-brand" href="#">My Website</a>
  </div>
</nav>
```

### Button
Button digunakan untuk membuat tombol dengan berbagai variasi warna dan ukuran.

```html
<button class="btn btn-primary">Tombol Primary</button>
<button class="btn btn-success">Tombol Success</button>
```

### Card
Card digunakan untuk menampilkan konten dalam bentuk kotak yang rapi.

```html
<div class="card" style="width: 18rem;">
  <div class="card-body">
    <h5 class="card-title">Judul Card</h5>
    <p class="card-text">Isi dari card.</p>
  </div>
</div>
```

### Grid System
Grid digunakan untuk mengatur layout agar responsif.

```html
<div class="container">
  <div class="row">
    <div class="col-md-6">Kolom 1</div>
    <div class="col-md-6">Kolom 2</div>
  </div>
</div>
```

### Alert
Alert digunakan untuk menampilkan pesan atau notifikasi.

```html
<div class="alert alert-warning">
  Ini adalah pesan peringatan
</div>
```

### Table
Table digunakan untuk menampilkan data dalam bentuk tabel.

```html
<table class="table table-bordered">
  <tr>
    <th>Nama</th>
    <th>NIM</th>
  </tr>
  <tr>
    <td>Fajar</td>
    <td>123456</td>
  </tr>
</table>
```

### Form
Form digunakan untuk input data dari pengguna.

```html
<form>
  <input type="text" class="form-control" placeholder="Masukkan nama">
</form>
```

### Badge
Badge digunakan untuk memberi label kecil pada elemen.

```html
<span class="badge bg-success">Baru</span>
```

### Accordion
Accordion digunakan untuk menampilkan konten yang bisa dibuka/tutup.

```html
<div class="accordion">
  <div class="accordion-item">
    <button class="accordion-button">Klik di sini</button>
  </div>
</div>
```

### Modal
Modal digunakan untuk menampilkan pop-up.

```html
<button class="btn btn-primary" data-bs-toggle="modal" data-bs-target="#exampleModal">
  Buka Modal
</button>
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
<!DOCTYPE html>
<html lang="id">

<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Mode Suci - Edisi Ramadan</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet" />
</head>
<body class="bg-success-subtle">
  <!-- Lihat file index.html untuk kode lengkap -->
</body>
</html>
```

> Kode lengkap tersedia di file `index.html`

## Output

![Bukti](assets/Screenshot%202026-04-07%20130739.png)