<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>README - Biodata Website</title>
</head>
<body>
  <h1>README - Biodata Website</h1>

  <h2>1. Pendahuluan</h2>
  <p>
    Website ini dirancang untuk menampilkan biodata pribadi dengan struktur yang rapi dan visual menarik. Website terdiri dari dua halaman utama :
  </p>
  <ul>
    <li>Homepage (index.html) yang berisi perkenalan singkat berupa teks dan foto.</li>
    <li>About Me (aboutme.html) yang menampilkan detail pendidikan, keterampilan, bahasa, serta hobi dan minat.</li>
  </ul>
  <p>
    Agar tampilan lebih estetik, digunakan CSS eksternal (style.css) yang mengatur tata letak, warna, tipografi, serta responsivitas. Dalam perancangan ini, saya menerapkan :
  </p>
  <ul>
    <li>Semantic HTML untuk membangun struktur halaman yang mudah dipahami baik oleh manusia maupun mesin (search engine, screen reader).</li>
    <li>Berbagai selektor CSS seperti class selector, element selector, pseudo-class selector (hover), dan descendant selector.</li>
    <li>Properti CSS visual seperti background, font-size, color, padding, margin, flexbox, dan box-shadow.</li>
    <li>Konsep Box Model (content, padding, border, margin) dalam setiap elemen, agar desain konsisten dan mudah diatur.</li>
  </ul>
  <hr>
  <h2>2. Penjelasan Struktur index.html</h2>
  
```
<!DOCTYPE html>
<html lang="en">
```
  <ul>
    <li>!DOCTYPE html menandakan bahwa dokumen ini menggunakan standar HTML5.</li>
    <li>html lang="en" memberi tahu browser dan mesin pencari bahwa bahasa utama halaman ini adalah bahasa Inggris.</li>
  </ul>

```
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
```
  <ul>
    <li> "meta charset="UTF-8"" agar semua karakter (termasuk simbol dan bahasa non-Inggris) bisa ditampilkan.</li>
    <li> meta name="viewport" penting untuk responsive design, memastikan halaman menyesuaikan ukuran layar perangkat (desktop maupun mobile).</li>
  </ul>

  ```
    <link rel="stylesheet" href="style.css">
    <title>Homepage</title>
</head>
```
  <ul>
    <li>link rel="stylesheet" href="style.css" menghubungkan file HTML dengan file CSS eksternal.</li>
    <li>title menentukan judul yang akan muncul di tab browser.</li>
  </ul>

```
<body>
    <div class="main">
```
  <ul>
    <li>body adalah area utama tempat konten ditampilkan.</li>
    <li>div class="main" membungkus seluruh isi halaman agar lebih mudah diatur dengan CSS.</li>
  </ul>

```
        <div class="navbar">
            <img src="LOGO1.png" class="logo">
            <ul>
                <li><a href="index.html">Home</a></li>
                <li><a href="aboutme.html">About Me</a></li>
            </ul>
        </div>
```

  <ul>
    <li>div class="navbar" berfungsi sebagai header navigasi.</li>
    <li>img menampilkan logo, diberi class logo untuk styling khusus.</li>
    <li>ul adalah unordered list untuk menampung menu navigasi.</li>
    <li>li a, setiap item list mengandung tautan (link) ke halaman lain (Home & About Me).</li>
  </ul>

```
        <div class="info">
            <h1> Hi, I'm Cevyn!</h1>
            <h3>
                Hello, my name is Cevyn. I am a student at Undiknas University, <br>
                studying web programming. I am also interested in digital art, <br>
                which allows me to explore creativity alongside technology.
            </h3>
        </div>
```
  <ul>
    <li>div class="info" menyimpan teks perkenalan.</li>
    <li>h1 digunakan untuk judul utama.</li>
    <li>h3 digunakan untuk teks deskriptif. Disisipkan <br> untuk pindah baris.</li>
  </ul>

```
        <div class="image">
            <img src="HM.jpg" class="me">
        </div>
    </div>
</body>
</html>
```
  <ul>
    <li>div class="image" menampilkan gambar pribadi (HM.jpg).</li>
    <li>Class me digunakan agar styling foto dapat diatur di CSS.</li>
    <li>Penutup /div, /body, dan /html menandakan akhir halaman.</li>
  </ul>
  <hr>

  <h2>3. Penjelasan Struktur aboutme.html</h2>
  <p>Halaman ini lebih panjang karena berisi detail biodata.</p>
  <h3>a. Header & Navigasi</h3>

  ```
<body class="about-page">
    <div class="main">
        <div class="navbar">
            <img src="LOGO1.png" class="logo">
            <ul>
                <li><a href="index.html">Home</a></li>
                <li><a href="aboutme.html">About Me</a></li>
            </ul>
        </div>
    </div>
```
  <ul>
    <li>Sama seperti halaman index, terdapat navbar dengan logo dan menu navigasi.</li>
    <li>class="about-page" dipasang di body>agar CSS bisa membedakan styling khusus halaman ini.</li>
  </ul>

  <h3>b. Bagian Pendidikan (Timeline)</h3>

  ```
<div class="timeline">
    <h2>Education</h2>
    <div class="timeline-item">
        <div class="timeline-date">2010 - 2016</div>
        <div class="timeline-content">
            <h3>SDK Ruteng IV</h3>
        </div>
    </div>
    ...
</div>
```
  <ul>
    <il>Menggunakan struktur timeline dengan tahun dan sekolah.</il>
    <il>Semantic heading <h2> digunakan untuk judul bagian.</il>
    <il>Tiap pengalaman pendidikan disusun dalam .timeline-item dengan tahun (timeline-date) dan isi (timeline-content).</il>
  </ul>

  <h3>c. Bagian Skills</h3>

```
<div class="skills-section">
    <h2>Technical Skills</h2>
    <div class="skills-box">
        <div class="software-skills">
            <h3>Software Skills</h3>
            <div class="icons">
                <span>Ps</span>
                <span>Ai</span>
            </div>
        </div>
```
  <ul>
    <li>Dibagi menjadi software skills dan coding skills.</li>
    <li>Ikon sederhana ditampilkan dengan span yang bisa di-styling CSS.</li>
  </ul>

  <h3>d. Bagian Bahasa</h3>

```
<div class="language-section">
    <h2>Language</h2>
    <div class="language-list">
        <div class="lang-item">
            <h3>Indonesia</h3>
            <p>Fluent</p>
        </div>
        <div class="lang-item">
            <h3>English</h3>
            <p>Intermediate</p>
        </div>
    </div>
</div>
```
  <ul>
    <li>Menampilkan daftar bahasa yang dikuasai dengan h3 sebagai nama bahasa dan <p> untuk tingkatannya.</li>
  </ul>

  <h3>d. Bagian Hobi</h3>
  
```
<div class="hobbies-section">
    <h2>Hobbies & Interests</h2>
    <div class="hobbies-list">
        <div class="hobby-item">
            <i class="fas fa-music"></i>
            <p>Jazz & Indie</p>
        </div>
```
  <ul>
    <li>Menggunakan Font Awesome Icon (i class="fas fa-music") untuk menampilkan ikon musik, buku, kuas, hingga kucing.</li>
    <li>Menunjukkan minat pemilik website secara visual.</li>
  </ul>
  <hr>

  <h2>4. Penjelasan CSS (style.css)</h2>
  <p>File CSS inilah yang membuat halaman tampak rapi dan aesthetic.</p>

  <h3>a. Reset & Dasar</h3>

```
*{
    padding: 0;
    margin: 0;
    box-sizing: border-box;
}
```
  <ul>
    <li>Reset default CSS agar konsisten di semua browser.</li>
    <li>box-sizing: border-box memastikan padding dan border termasuk ke dalam total ukuran box (penerapan langsung dari Box Model).</li>
  </ul>

  <h3>b. Navbar</h3>

```
.navbar{
    width: 86%;
    display: flex;
    margin: auto;
    padding: 15px 0;
    align-items: center;
    justify-content: space-between;
}
```
  <ul>
    <li>Menggunakan flexbox untuk meratakan logo dan menu secara horizontal.</li>
    <li>Memberi ruang (padding) dan mengatur posisi (justify-content)</li>
  </ul>

  <h3>c. Info Section</h3>

```
.info h1{
    color:#EFDCAB;
    font-size: 60px;
}
```
  <ul>
    <li>Selektor spesifik (.info h1) untuk judul utama.</li>
    <li>Warna (#EFDCAB) kontras dengan background gelap.</li>
    <li>Ukuran font besar untuk penekanan hierarki informasi.</li>
  </ul>

  <h3>d. Timeline</h3>

```
.timeline {
    flex: 1;
    position: relative;
    padding-left: 40px;
    border-left: 3px solid #443627;
}
```
  <ul>
    <li>Garis di sisi kiri dibuat dengan border-left sebagai elemen visual timeline.</li>
    <li>Memberi padding-left agar teks tidak menempel ke garis.</li>
  </ul>

  <h3>e. Skills & Icons</h3>

```
.icons span {
    display: inline-block;
    background-color: #D98324;
    color: #443627;
    font-weight: bold;
    padding: 10px 15px;
    border-radius: 8px;
    box-shadow: 0 2px 5px rgba(0,0,0,0.2);
}
```
  <ul>
    <li>Membuat badge-style untuk skill software (Ps, Ai).</li>
    <li>Menggunakan box-shadow agar ikon terlihat timbul (contoh nyata penerapan Box Model).</li>
  </ul>

  <h3>f. Hobbies Icons</h3>

```
.hobby-item i {
    font-size: 30px;
    color: #e67e22;
    margin-bottom: 10px;
}
```
  <ul>
    <li>Menentukan ukuran ikon dan warna agar konsisten.</li>
    <li>margin-bottom memberi jarak antar elemen (penerapan Box Model).</li>
  </ul>


    
  <h2>5. Kesimpulan</h2>
  <p>
    Website ini berhasil memenuhi kriteria tugas:
  </p>
  <ul>
    <li>Semantic HTML digunakan dengan header, h1, h2, ul, li, p yang jelas hierarkinya.</li>
    <li>Berbagai selektor CSS digunakan: universal selector (*), class selector (.info), element selector (h1, p), dan pseudo-class (a:hover).</li>
    <li>Properti CSS visual mencakup background, font-size, color, flexbox, box-shadow, border-radius, hingga hover effect.</li>
    <li>Box Model diterapkan pada hampir semua elemen dengan padding, margin, border, dan shadow untuk mengatur jarak dan ukuran.</li>
  </ul>
  <p>
    Secara keseluruhan, website ini bukan hanya biodata sederhana, melainkan representasi penerapan teori HTML dan CSS dasar dengan praktik nyata.
  </p>
</body>
</html>
