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
    <strong>Kartika Pringgo Hutomo</strong>
    <br>
    <strong>2311102196</strong>
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
Berikut **dasar teori dalam bentuk paragraf** untuk Task 4:

Dasar teori dalam pembuatan halaman “Mode Suci (Edisi Ramadan)” ini menggunakan framework CSS yaitu Bootstrap sebagai alat utama dalam mendesain tampilan web. Bootstrap merupakan framework front-end yang menyediakan kumpulan class siap pakai untuk mempermudah proses pembuatan antarmuka yang responsif dan konsisten tanpa harus menulis CSS secara manual. Dengan menggunakan Bootstrap, pengembang dapat memanfaatkan sistem grid, komponen, serta utility class untuk mengatur layout, warna, tipografi, dan elemen lainnya secara efisien. Pada proyek ini, seluruh tampilan dibuat menggunakan class bawaan Bootstrap seperti container, row, col, card, dan button, sehingga tidak diperlukan penulisan CSS tambahan.

Selain itu, Bootstrap memiliki sistem grid berbasis flexbox yang memungkinkan pembuatan layout responsif yang dapat menyesuaikan dengan berbagai ukuran layar, baik desktop maupun perangkat mobile. Komponen seperti card digunakan untuk menampilkan konten secara terstruktur, sedangkan utility class seperti text-center, bg-dark, text-warning, dan shadow digunakan untuk mempercantik tampilan dengan cepat. Penggunaan Bootstrap juga membantu dalam menjaga konsistensi desain karena seluruh elemen sudah memiliki standar styling yang seragam.

Dalam konteks desain, halaman ini mengusung tema Ramadan dengan nuansa warna gelap yang dipadukan dengan warna terang seperti kuning dan hijau untuk mencerminkan suasana yang tenang, religius, dan penuh kehangatan. Dengan memaksimalkan penggunaan Bootstrap tanpa CSS tambahan, proyek ini bertujuan untuk menunjukkan kemudahan dan efisiensi dalam membangun tampilan web modern secara cepat, responsif, dan tetap menarik secara visual.
</p>

# Tugas 4 - Mode Suci (Edisi Ramadan)
## 1. Source code index.html
```
<!-- 2311102196
Kartika Pringgo Hutomo
S1IF-11-05 -->
<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Ramadan Mode Suci</title>
  <!-- Bootstrap CSS -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body class="bg-dark text-light">

  <div class="container py-5">
    <div class="text-center mb-5">
      <h1 class="display-4 text-warning">Ramadan Kareem 🌙</h1>
      <p class="lead">Semoga ibadah kita diterima dan hati kita semakin bersih</p>
    </div>

    <div class="row justify-content-center">
      <div class="col-md-6">
        <div class="card text-center shadow-lg">
          <div class="card-body">
            <h5 class="card-title text-success">Pesan Spesial</h5>
            <p class="card-text">
              Selamat menjalankan ibadah puasa 🤍<br>
              Semoga kita selalu diberi kesehatan, keberkahan,
              dan dipertemukan dengan kemenangan di hari yang fitri.
            </p>
            <a href="#" class="btn btn-warning">Kirim Doa ✨</a>
          </div>
        </div>
      </div>
    </div>

    <div class="row mt-5 text-center">
      <div class="col-md-4">
        <div class="p-3 border rounded">
          <h5>Sahur</h5>
          <p>Jangan lupa niat dan makan yang cukup</p>
        </div>
      </div>
      <div class="col-md-4">
        <div class="p-3 border rounded">
          <h5>Puasa</h5>
          <p>Jaga hati, lisan, dan perbuatan</p>
        </div>
      </div>
      <div class="col-md-4">
        <div class="p-3 border rounded">
          <h5>Berbuka</h5>
          <p>Awali dengan yang manis dan penuh syukur</p>
        </div>
      </div>
    </div>

    <footer class="text-center mt-5">
      <p class="text-secondary">Dibuat dalam Mode Suci 🕌</p>
    </footer>
  </div>

  <!-- Bootstrap JS -->
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
```

# Output
![alt text](<image.png>)

# Penjelasan
<p align="justify">
Berikut **penjelasan kode dalam bentuk paragraf**:

Kode pada halaman “Mode Suci (Edisi Ramadan)” menggunakan Bootstrap sebagai framework utama untuk mengatur tampilan tanpa penambahan CSS manual. Pada bagian awal terdapat deklarasi DOCTYPE html yang menandakan penggunaan HTML5. Elemen html menggunakan atribut lang sama dengan id untuk menunjukkan bahasa yang digunakan. Pada bagian head terdapat meta charset untuk encoding karakter dan meta viewport agar halaman dapat tampil responsif di berbagai perangkat. Selain itu, terdapat link yang menghubungkan ke CDN Bootstrap sehingga seluruh class bawaan Bootstrap dapat digunakan dalam halaman.

Pada bagian body, digunakan class bg-dark dan text-light untuk memberikan latar belakang gelap dengan teks berwarna terang. Seluruh konten dibungkus dalam container dengan tambahan padding menggunakan class py-5 agar tampilan tidak terlalu rapat. Bagian header dibuat menggunakan div dengan class text-center dan margin bawah, yang berisi judul dengan class display-4 dan text-warning untuk memberikan ukuran besar serta warna kuning, serta paragraf dengan class lead untuk menampilkan teks pembuka yang lebih menonjol.

Selanjutnya terdapat sistem grid Bootstrap menggunakan row dan col-md-6 yang dipadukan dengan justify-content-center untuk memposisikan card di tengah halaman. Komponen card digunakan untuk menampilkan pesan utama, dengan tambahan class text-center dan shadow-lg agar terlihat rapi dan memiliki efek bayangan. Di dalam card terdapat card-body, card-title, dan card-text yang masing-masing berfungsi untuk mengatur struktur isi card. Tombol dibuat menggunakan class btn dan btn-warning yang memberikan tampilan tombol berwarna kuning khas Bootstrap.

Pada bagian berikutnya terdapat tiga kolom yang dibuat menggunakan row dan col-md-4 untuk menampilkan informasi Sahur, Puasa, dan Berbuka. Masing-masing kolom menggunakan class p-3, border, dan rounded untuk memberikan padding, garis tepi, serta sudut melengkung tanpa perlu CSS tambahan. Terakhir, bagian footer dibuat menggunakan class text-center dan margin atas, dengan tambahan text-secondary agar warna teks terlihat lebih lembut. Di bagian bawah halaman juga terdapat script Bootstrap bundle yang berfungsi untuk mengaktifkan komponen interaktif Bootstrap jika diperlukan. Secara keseluruhan, kode ini memanfaatkan class bawaan Bootstrap secara maksimal untuk menghasilkan tampilan yang responsif, rapi, dan menarik tanpa penulisan CSS manual.

</p>