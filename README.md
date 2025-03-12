PK   ؎lZ               js/PK            PK   ؎lZ               css/PK            PK   ؎lZ            
   index.html<!DOCTYPE html>
<html lang="id">

<head>
  <!-- Meta Data -->
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>SMK Wikrama 1 Banjarmasin</title>
  
  <!-- CSS -->
  <link rel="stylesheet" href="css/style.css">
</head>

<body>
  <!-- Navbar -->
  <header class="main-header">
    <div class="logo">
      <img src="https://smkwikrama1banjarmasin.sch.id/assets2/wk_bjm.png" alt="Logo SMK Wikrama 1 Banjarmasin" width="100">
    </div>
    <nav>
      <a href="#home">Home</a>
      <a href="#our-profile">Profil Kami</a>
      <a href="#vision-mission">Visi & Misi</a>
      <a href="#contact">Kontak</a>
    </nav>
  </header>
  
  <hr />
  
  <!-- Home Section -->
  <section id="home">
    <header>
      <h1>Hi <span id="username">User</span>, Welcome to SMK Wikrama 1 Banjarmasin</h1>
      <p><strong>"There is no Learning Community Without Vision School Leadership"</strong></p>
    </header>
  </section>
  
  <hr />
  
<!-- Profil Sekolah -->
<section id="profil">
    <h2>Profil SMK Wikrama 1 Banjarmasin</h2>
    
    <!-- Tentang Sekolah -->
    <div class="profil-box">
        <h3>Tentang Sekolah</h3>
        <p>SMK Wikrama 1 Banjarmasin merupakan sekolah yang berfokus pada pendidikan kejuruan dengan berbagai keunggulan dalam fasilitas, program keahlian, serta kegiatan ekstrakurikuler yang mendukung perkembangan siswa.</p>
    </div>

    <!-- Program Keahlian -->
    <div class="profil-box">
        <h3>Program Keahlian</h3>
        <ul>
            <li><strong>Teknik Komputer dan Jaringan (TKJ)</strong> - Mempelajari teknologi jaringan komputer, perakitan perangkat keras, serta keamanan sistem.</li>
            <li><strong>Otomatisasi Tata Kelola Perkantoran (OTKP)</strong> - Fokus pada administrasi perkantoran, pengelolaan dokumen, dan penggunaan teknologi perkantoran.</li>
        </ul>
    </div>

    <!-- Fasilitas Sekolah -->
    <div class="profil-box">
        <h3>Fasilitas Sekolah</h3>
        <p>Sekolah Kami dilengkapi dengan laboratorium komputer, perpustakaan, ruang praktik, serta fasilitas pendukung lainnya untuk menunjang pembelajaran.</p>
    </div>

    <!-- Ekstrakurikuler -->
    <div class="profil-box">
        <h3>Ekstrakurikuler</h3>
        <ul>
            <li>Pramuka</li>
            <li>Paskibra</li>
            <li>Futsal</li>
            <li>Musik</li>
            <li>Tari</li>
        </ul>
    </div>

    <!-- Lokasi dan Kontak -->
    <div class="profil-box">
        <h3>Lokasi & Kontak</h3>
        <p><strong>Alamat:</strong> Jalan Veteran Simp. SMP 7, No. 3, RT. 30, Kel. Sungai Bilu - Banjarmasin Timur</p>
        <p><strong>Telepon:</strong> 08876076843</p>

        <!-- Google Maps -->
        <iframe 
            src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d31868.47698770322!2d114.58645692761233!3d-3.3219544968664915!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x0%3A0xabc123456789!2sSMK%20Wikrama%201%20Banjarmasin!5e0!3m2!1sid!2sid!4v1234567890123" 
            width="100%" 
            height="300" 
            style="border:0;" 
            allowfullscreen="" 
            loading="lazy">
        </iframe>
    </div>
</section>
  
  <hr />
  
  <!-- Visi & Misi -->
  <section id="vision-mission">
    <h2>Visi & Misi</h2>
    <h3>Visi:</h3>
    <p>Menjadi sekolah terbaik dalam membentuk karakter dan prestasi.</p>
    <h3>Misi:</h3>
    <ul>
      <li>Memberikan pendidikan berkualitas.</li>
      <li>Mengembangkan potensi setiap siswa.</li>
      <li>Menanamkan nilai-nilai kejujuran dan disiplin.</li>
    </ul>
  </section>
  
  <hr />
  
  <!-- Formulir Kontak -->
  <section id="contact">
    <h2>Hubungi Kami</h2>
    <form id="contactForm">
      <label for="nama">Nama:</label>
      <input type="text" id="nama" name="nama" required>
      
      <label for="email">Email:</label>
      <input type="email" id="email" name="email" required>
      
      <label for="telepon">Nomor Telepon:</label>
      <input type="tel" id="telepon" name="telepon" required>
      
      <label for="pesan">Pesan:</label>
      <textarea id="pesan" name="pesan" required></textarea>
      
      <button type="submit">Kirim</button>
    </form>
    <p id="formOutput"></p>
  </section>
  
  <hr />
  
  <!-- PPDB Section -->
  <section id="ppdb">
    <h2>Pendaftaran PPDB</h2>
    <p><strong>Ayo! segera daftarkan dirimu ke SMK Wikrama 1 BANJARMASIN dengan cara klik tombol di bawah ini!</strong></p>
    <p>Ilmu yang Amaliah, Amal yang Ilmiah, Akhlakul Karimah.</p>
    <a href="https://smkwikrama1banjarmasin.sch.id/ppdb" target="_blank">
      <button>Daftar Sekarang</button>
    </a>
  </section>
  
  <!-- JavaScript -->
  <script src="js/script.js"></script>
</body>

</html>PKH�]�  �  PK   ؎lZ               js/script.js// Smooth Scroll untuk navigasi
document.querySelectorAll('a[href^="#"]').forEach(anchor => {
    anchor.addEventListener("click", function(e) {
        e.preventDefault();

        const target = document.querySelector(this.getAttribute("href"));
        if (target) {
            window.scrollTo({
                top: target.offsetTop - 50, // Sesuaikan dengan tinggi navbar
                behavior: "smooth"
            });
        }
    });
});PKy����  �  PK   ؎lZ               css/style.css/* Reset default */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: Arial, sans-serif;
}

body {
    background-color: #f8f9fa;
    color: #333;
    line-height: 1.6;
    text-align: center;
}

/* Navbar */
.main-header {
    background-color: #0077b6;
    padding: 15px;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.main-header .logo img {
    width: 80px;
}

nav a {
    color: white;
    text-decoration: none;
    margin: 0 15px;
    font-size: 16px;
    font-weight: bold;
}

nav a:hover {
    text-decoration: underline;
}

/* Home Section */
#home {
    padding: 50px;
    background: url('https://smkwikrama1banjarmasin.sch.id/assets2/wk_bjm.png') no-repeat center;
    background-size: contain;
    background-color: rgba(255, 255, 255, 0.5); /* Transparan 50% */
    min-height: 300px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    position: relative;
}

#home::before {
    content: "";
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: rgba(255, 255, 255, 0.6); /* Overlay putih transparan */
    z-index: 1;
}

#home header {
    position: relative;
    z-index: 2;
}

#home h1 {
    font-size: 28px;
    color: #0077b6;
}

#home p {
    font-size: 18px;
    font-weight: bold;
    color: #555;
}
/* Sections */
section {
    padding: 40px 20px;
    margin: 20px auto;
    background-color: white;
    border-radius: 8px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    max-width: 800px;
}
/* Profil Sekolah */
#profil {
    padding: 50px 20px;
    background-color: #f8f9fa;
    text-align: center;
}

.profil-box {
    background: white;
    margin: 20px auto;
    padding: 20px;
    max-width: 800px;
    border-radius: 8px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    text-align: left;
}

.profil-box h3 {
    color: #0077b6;
    margin-bottom: 10px;
}

.profil-box ul {
    list-style: none;
    padding: 0;
}

.profil-box ul li {
    margin: 5px 0;
}

.profil-box iframe {
    border-radius: 8px;
}

/* Visi & Misi */
#vision-mission h2, #our-profile h2, #contact h2, #ppdb h2 {
    color: #0077b6;
    margin-bottom: 10px;
}

#vision-mission ul {
    text-align: left;
    list-style: none;
    padding-left: 20px;
}

#vision-mission ul li {
    margin: 5px 0;
}

/* Formulir Kontak */
form {
    display: flex;
    flex-direction: column;
    gap: 10px;
    max-width: 500px;
    margin: 0 auto;
}

input, textarea {
    padding: 10px;
    border: 1px solid #ccc;
    border-radius: 5px;
    width: 100%;
}

button {
    background-color: #0077b6;
    color: white;
    padding: 10px 15px;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    font-size: 16px;
    margin-top: 10px;
}

button:hover {
    background-color: #005f8a;
}

/* PPDB Section */
#ppdb {
    background-color: #0077b6;
    color: white;
    padding: 30px;
    border-radius: 10px;
    text-align: center;
}

#ppdb p {
    margin-bottom: 15px;
}

#ppdb button {
    background-color: white;
    color: #0077b6;
    font-weight: bold;
}

#ppdb button:hover {
    background-color: #eef2f3;
}

/* Responsive */
@media (max-width: 768px) {
    .main-header {
        flex-direction: column;
    }

    nav {
        margin-top: 10px;
    }

    nav a {
        display: block;
        margin: 5px 0;
    }
}PK~ y�,  ,  PK    ؎lZ                            js/PK    ؎lZ                        1   css/PK    ؎lZH�]�  �  
             c   index.htmlPK    ؎lZy����  �               $  js/script.jsPK    ؎lZ~ y�,  ,                  css/style.cssPK        �"    