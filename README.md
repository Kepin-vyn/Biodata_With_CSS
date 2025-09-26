<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>README - Biodata Website</title>
</head>
<body>
  <h1>📖 README - Biodata Website</h1>

  <h2>1. Deskripsi Umum</h2>
  <p>
    Proyek ini adalah <strong>website biodata pribadi</strong> sederhana yang dibuat menggunakan 
    <em>HTML</em> dan <em>CSS</em>. Tujuan dari proyek ini adalah untuk:
  </p>
  <ul>
    <li>Mempelajari struktur dasar dokumen HTML.</li>
    <li>Menerapkan konsep <em>CSS Box Model</em> pada layout halaman.</li>
    <li>Membuat desain sederhana dengan <em>Flexbox</em> agar lebih rapi dan seimbang.</li>
    <li>Menampilkan informasi biodata pribadi seperti pendidikan, keterampilan, bahasa, dan hobi.</li>
  </ul>
  <p>
    Website ini terdiri dari dua halaman utama: <code>index.html</code> (homepage) dan 
    <code>aboutme.html</code> (halaman biodata lengkap) dengan satu file <code>style.css</code> 
    sebagai pengatur tampilan.
  </p>

  <h2>2. Struktur File & Direktori</h2>
  <pre>
  📂 Project Folder
  ├── index.html        → Halaman utama (homepage)
  ├── aboutme.html      → Halaman biodata lengkap
  ├── style.css         → File CSS untuk styling
  ├── LOGO1.png         → Logo untuk navbar
  └── HM.jpg            → Foto profil
  </pre>

  <h2>3. Penjelasan Tiap Bagian</h2>

  <h3>a. index.html</h3>
  <ul>
    <li><strong>&lt;head&gt;</strong> → Berisi metadata, judul halaman, dan link ke file CSS.</li>
    <li><strong>&lt;div class="main"&gt;</strong> → Wadah utama halaman, terdiri dari:
      <ul>
        <li><strong>Navbar</strong> (<code>&lt;div class="navbar"&gt;</code>) → berisi logo dan menu navigasi 
          (<code>Home</code>, <code>About Me</code>).</li>
        <li><strong>Info</strong> (<code>&lt;div class="info"&gt;</code>) → sapaan singkat, nama, 
          dan deskripsi diri.</li>
        <li><strong>Image</strong> (<code>&lt;div class="image"&gt;</code>) → menampilkan foto profil.</li>
      </ul>
    </li>
  </ul>

  <h3>b. aboutme.html</h3>
  <ul>
    <li><strong>&lt;div class="aboutme"&gt;</strong> → Kontainer utama halaman biodata.</li>
    <li><strong>Top Section</strong> → berisi:
      <ul>
        <li><strong>Education</strong> → daftar riwayat sekolah dari SD hingga perguruan tinggi.</li>
        <li><strong>Technical Skills</strong> → software yang dikuasai (Ps, Ai, Id, Xd, Pr) dan 
          bahasa pemrograman (HTML, CSS).</li>
      </ul>
    </li>
    <li><strong>Bottom Section</strong> → berisi:
      <ul>
        <li><strong>Language</strong> → bahasa yang dikuasai (English, Indonesia).</li>
        <li><strong>Hobbies</strong> → minat seperti musik, digital art, dan merawat kucing.</li>
      </ul>
    </li>
  </ul>

  <h3>c. style.css</h3>
  <ul>
    <li><strong>Reset</strong> → <code>* { margin:0; padding:0; box-sizing:border-box; }</code></li>
    <li><strong>.main</strong> → mengatur ukuran penuh layar dan warna background.</li>
    <li><strong>.navbar</strong> → menggunakan Flexbox agar logo dan menu sejajar.</li>
    <li><strong>.info</strong> → mengatur teks sambutan (ukuran font, margin, warna).</li>
    <li><strong>.image</strong> → menempatkan foto di kanan bawah halaman.</li>
    <li><strong>.aboutme .section</strong> → menggunakan Flexbox agar box berdampingan secara horizontal.</li>
    <li><strong>.box</strong> → setiap bagian biodata memakai padding, margin, dan border-radius sesuai konsep box model.</li>
  </ul>

  <h2>4. Konsep Box Model</h2>
  <p>
    Setiap elemen di halaman menggunakan konsep <strong>CSS Box Model</strong>, 
    yang terdiri dari:
  </p>
  <ol>
    <li><strong>Content</strong> → isi berupa teks, daftar, atau gambar.</li>
    <li><strong>Padding</strong> → ruang di dalam box agar teks tidak mepet ke tepi.</li>
    <li><strong>Border</strong> → garis pembatas di luar padding, pada kode ini berupa border-radius untuk sudut melengkung.</li>
    <li><strong>Margin</strong> → jarak antar box agar tata letak lebih lega.</li>
  </ol>
  <p>
    Dengan penggunaan <code>box-sizing: border-box;</code> seluruh ukuran width/height sudah 
    termasuk padding dan border, sehingga tata letak lebih stabil.
  </p>

  <h2>5. Fungsi & Kelebihan</h2>
  <ul>
    <li>Menyajikan biodata dengan tampilan <strong>rapi, sederhana, dan informatif</strong>.</li>
    <li>Menunjukkan <strong>penerapan Flexbox</strong> untuk mengatur tata letak konten.</li>
    <li>Memisahkan <strong>struktur (HTML)</strong> dan <strong>tampilan (CSS)</strong> agar lebih terorganisir.</li>
    <li>Menerapkan <strong>konsep Box Model</strong> untuk setiap elemen utama.</li>
    <li>Dapat dijadikan <strong>portofolio sederhana</strong> untuk memperkenalkan diri.</li>
  </ul>


  <h2>6. Kesimpulan</h2>
  <p>
    Website biodata ini berhasil menampilkan <strong>informasi personal</strong> dengan 
    struktur yang jelas. Penerapan <em>box model</em> memperlihatkan bagaimana padding, margin, 
    dan border bekerja dalam membentuk tampilan yang rapi. Dengan pengembangan lebih lanjut, 
    website ini dapat ditingkatkan menjadi <strong>portofolio profesional</strong> yang responsif 
    dan menarik.
  </p>
</body>
</html>
