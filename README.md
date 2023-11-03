# Lab6web

# Membuat Layout sederhana
## Kerangka Layout

![image](https://github.com/adityaputrawijaya/Lab6web/assets/115687055/7e66f15f-0c17-4cfa-a3a1-24950198e70e)

```
<!DOCTYPE html>
<html>
<head>
<title>Page Title</title>
</head>
<body>

</body>
</html>
```


## Membuat Navigasi
Membuat navigasi menggunakan html
```
<header><h1>Berita News</h1></header>
    <nav>
      <ul>
        <a href="web.html" class="active">Home</a>
        <a href="#main">Artikel</a>
        <a href="about.html">About</a>
        <a href="kontak.html">Contact</a>
      </ul>
    </nav>
```
Kemudian tambahkan css kedalam html
```
*{
    padding: 0;
    margin: 0;
}
/* layout CSS */
#main {
    float: left;
    width: 640px;
    padding: 19px;
}

/* BODY */
body {
    line-height:1;
    font-size:100%;
    font-family:'Open Sans', sans-serif;
    color:#6b6969;
}

/* container */
#container {
    width: 980px;
    height: 2000px;
    margin: 0 auto;
    box-shadow: 0 0 1em #cccccc;
}

/* Header */
header{
    padding: 10px;
    background-color: #ddd8d8;
}
header h1 {
    margin: 20px 10px;
    color: #181616;
}

/* WRAPPER */
#wrapper{
    margin: 0px;
}

/* Navigasi */
nav{
    display: block;
    background-color: rgb(207, 5, 5);
    padding: 5px;
}
ul a{
    color: white;
    display: inline-block;
    padding: 5px;
    margin: 5px;
    text-decoration: none;
}
```

### Hasil
![image](https://github.com/adityaputrawijaya/Lab6web/assets/115687055/1407a6a8-abd7-4e65-b917-f36208a6c7bc)


## Membuat Slide show 
Membuat slideshow dengan html
```
<section id="wrapper">
      <h1 style="margin: 10px 20px;">Indonesia Emas 2045</h1>
      <!-- Slider -->
      <div class="slide">
        <img src="indo452.jpg.crdownload" alt="sam1" id="sam1">
        <img src="indo451.JPG" alt="sam2" id="sam2">
        <img src="indo45.png" alt="sam3" id="sam3">
      </div>
      <div class="slider-nav">
            <a href="#sam1"></a>
            <a href="#sam2"></a>
            <a href="#sam3"></a>
      </div>
</section>
```
Kemudian tambahkan css kedalam html
```
.slide{
    display: flex;
    aspect-ratio: 16/9;
    overflow-x: auto;
    overflow: hidden;
    scroll-snap-type: x mandatory;
    scroll-behavior: smooth;
}
.slide img{
    max-width: auto;
    padding: 30px;
    flex: 1 0 92%;
    scroll-snap-align: start;
    object-fit: cover;
}
.slider-nav{
    display: flex;
    position: relative;
    column-gap: 5px;
    bottom: 55px;
    left: 150px;
    z-index: 1;
    margin-left:300px;
}
.slider-nav a{
    background-color:grey;
    width:20px;
    height: 20px;
    border-radius: 10px;
    opacity: 0.75;
}
.slider-nav a:hover{
    opacity: 1;
    transition: 1s;
}
```
### Hasil
![image](https://github.com/adityaputrawijaya/Lab6web/assets/115687055/67eb9422-8206-449c-beb0-2d67ed14c850)

![image](https://github.com/adityaputrawijaya/Lab6web/assets/115687055/44741a67-630c-4a13-a9fe-ee0fde477d54)

![image](https://github.com/adityaputrawijaya/Lab6web/assets/115687055/c6e7c9bc-7dbf-4193-9763-2b1ff0936645)

## Membuat Sidebar
Membuat sidebar dengan html
```
<section id="wrapper">
      <aside id="sidebar">
          <div class="side-bar">
            <h3 class="title">Other News</h3>
            <ul>
              <li><a href="#">Sport News</a></li>
              <li><a href="#">Political News</a></li>
              <li><a href="#">Economic News</a></li>
              <li><a href="#">Environmental News</a></li>
              <li><a href="#">Domestic News</a></li>
            </ul>
          </div>
          <div class="side-bar">
            <h3 class="title">Widget Text</h3>
            <p>Vestibulum lorem elit, iaculis in nisl volutpat, malesuada tincidunt 
              arcu. Proin in leo fringilla, vestibulum mi porta, faucibus felis. Integer 
              pharetra est nunc, nec pretium nunc pretium ac.</p>
          </div>
      </aside>
</section>
```
Kemudian tambahkan css kedalam html
```
#sidebar{
    float: left;
    width: 260px;
    padding: 20px;
}
.side-bar .title {
    padding:10px 16px;
    background-color:#428bca;
    color:#fff;
}    
.side-bar {
    border:1px solid #eee;
    margin-bottom:20px;
}
.side-bar ul{
    list-style: none; 
}
.side-bar ul li{
   border-bottom:1px solid #eee;
}
.side-bar a{
    padding:10px 16px;
    color:#333;
    display:block;
    text-decoration:none;
}
.side-bar li:hover a {
    background-color:#eee;
}
.side-bar p {
    padding:15px;
    line-height:25px;
}
```
### Hasil
![image](https://github.com/adityaputrawijaya/Lab6web/assets/115687055/af003a3a-9498-4642-89d0-b91fffd6168e)
 

## Membuat Main content
Membuat main content dengan html
```
<section id="wrapper">
    <section id="main">
        <article class="artikel">
          <p>
            KEMENKO PMK --  Indonesia akan mengalami usia emas pada tahun 2045. Pada saat itu, Indonesia genap berusia 100 tahun alias satu abad. Di masa itu, ditargetkan Indonesia sudah menjadi negara maju dan telah sejajar dengan negara adidaya. 
          </p><br>
          <p>
            Momentum bersejarah tersebut memang masih sekitar saperempat abad lagi. Namun untuk mewujudkannya butuh persiapan yang matang sejak jauh-jauh hari. Sumber daya manusia Indonesia harus unggul, berkualitas, dan memiliki karakter. 
          </p><br>
          <p>
            Menteri Koordinator Bidang Pembangunan Manusia dan Kebudayaan (Menko PMK) Muhadjir Effendy mengatakan, generasi yang akan mewujudkan Indonesia Emas adalah generasi muda, khususnya yang saat ini tengah menempuh pendidikan di perguruan tinggi.
          </p><br>
          <p>
            Dia menerangkan, para mahasiswa/mahasiswi dan lulusan universitas jenjang sarjana saat ini berada di kisaran usia 20 tahun. Menurutnya, pada masa Indonesia berusia 100 tahun yaitu 2045, usia mereka masih sekitar 40 tahun ke atas, yang merupakan usia puncak karir bagi profesional.
          </p><br>
          <p>
            "Artinya, Indonesia Emas itu adalah milik saudara semua, bukan milik saya. Bukan milik mereka yang saat ini usianya sudah di atas 50 tahun," ujar Muhadjir saat menyampaikan sambutan pada Wisuda Ke-105 Periode III Universitas Muhammadiyah Malang (UMM), di UMM Dome Malang, pada Kamis (6/10/2022).
          </p>
        </article>
    </section>
</section>
```
Kemudian tambahkan css kedalam html
```
.artikel{
   margin-left: 10px;
   padding: 30px;
}
.artikel p{
    font-size: 100%;
    justify-content: space-between;
}
```
### Hasi
![image](https://github.com/adityaputrawijaya/Lab6web/assets/115687055/1e1c724f-ea61-44f1-bc6a-8b13bd9ef6fe)


## Membuat Artikel Lainnya
Membuat more artikel dengan html
```
<section id="wrapper">
	<section id="main">
          <hr class="divider" />

            <article class="entry">
                <h2>Pemilihan Umum 2024</h2>
                <img src="gambar/pemilu.jpeg" alt="Pemilu">
                <p>Indonesia mendekati waktu pemilihan umum (pemilu) serentak tahun 2024. Pemilu serentak ini memilih Presiden dan Wakil Presiden, Anggota DPR, DPD, DPRD Provinsi dan DPRD Kabupaten/Kota.
                  <a href="#">Lantas siapa peserta pemilu 2024?.</a>
                </p>
            </article>
        
          <hr class="divider" />
    
            <article class="entry">
                <h2>Ice Cold Documentary Film</h2>
                <img src="gambar/Icecold.jpeg" alt="IceCold" class="right-img">
                <p>Dokumenter ini mengulas berbagai pertanyaan tak terjawab seputar persidangan Jessica Wongso—bertahun-tahun setelah kematian sahabatnya, Mirna Salihin.
                  Dengan menyaksikan dokumenter ini, mari bersama-sama memahami kasus ini <a href="#">lebih kompleks lagi.</a>
                </p>
            </article>
	</section>
</section>
```
Kemudian tambahkan css kedalam html 
```
.divider {
    border:0;
    border-top:1px solid #eeeeee;
    margin:40px 0;
}
.entry {
    margin: 15px 0;
    margin-left: 30px;
}
.entry h2 {
    margin-bottom: 20px;
}
.entry p {
    line-height: 25px;
}
.entry img {
    float: left;
    border-radius: 5px;
    margin-right: 15px;
}
.entry .right-img {
    float: right;
}
```
### Hasil
<img 

## Membuat Footer
Membuat footer dengan html
```
    <footer>
      <div class="kontak">
        <h2><a href="kontak.html" style="text-decoration: none;">Contact</a></h2>
        <p>&#128383; 0812-9318-9221</p>
        <p><a href="kontak.html" style="text-decoration: none;">&#128386; dimasf.30@mhs.pelitabangsa.ac.id</a></p>
      </div>
      <div class="lisensi">
        <p>&copy; 2023 - Dimas Firmansyah</p>
      </div>
    </footer>
```
Kemudian tambahkan css kedalam html
```
footer{
    background-color: aqua;
    padding: 20px;
    margin: 10px;
    margin-bottom: 10px;
    border-radius: 10px;
}
.lisensi{
    float: right;
}
```
### Hasil
<img 

### Hasil Akhir

![hasil13]

### Tambahkan Layout untuk menu About
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>About</title>
</head>
<style>
*{
    padding: 0px;
    margin: 0px;
}
body{
    line-height:1;
    font-size:100%;
    font-family:'Open Sans', sans-serif;
    color:#6b6969;
}
#container {
    width: 600px;
    height: 600px;
    margin: 0 auto;
    box-shadow: 0 0 1em #cccccc;
}
#wrapper{
  margin: 0px;
}
.gambar img{
  width: 100px;
  height: 100px;
  border-radius: 50%;
  padding: 10px;
  margin: 0px auto;
  display: block;
}
.desc{
  box-shadow: 0 0 1em #cccccc;
  border-radius: 10px;
  width: 500px;
  margin: 0px auto;
  display: block;
}
.desc p{
  padding: 5px;
}
.button{
  padding: 10px;
}
.button button{
  margin: 0px auto;
  display: block;
}
button a{
  text-decoration: none;
  margin: 0px auto;
  display: block;
  padding: 10px;
}
</style>
<body>
  <div id="container">
    <section class="about">
      <h1 align="center">About Me</h1>
      <hr>
    </section>

    <section id="wrapper">
      <div class="gambar">
        <img src="gambar/saya.png" alt="me">
      </div>
      <h1 align="center">Dimas Firmansyah</h1><br>
      <div class="desc">
        <p>
          Saya, Dimas Firmansyah, merupakan salah satu mahasiswa Universitas Pelita Bangsa.
        </p>
        <p>
          Saat ini, saya sedang menempuh jenjang sarjana di bidang teknik informatika, dan kami sedang mempelajari cara membuat tata letak website.
        </p>
        <p>
          Tata letak website adalah komponen yang sangat penting dalam proses pembuatan website, terutama untuk pengembangan desain dan pengalaman pengguna.
        </p>
        <p>
          Selain itu, tata letak website juga berfungsi untuk mempermudah para pengembang web dalam proses pembuatan website secara keseluruhan
        </p>

      </div>
    </section>

    <div class="button">
      <button><a href="home.html">Back to Content</a></button>
    </div>

  </div>
</body>
</html>
```
### Hasil
<img 

### Tambahkan layout untuk menu Contact
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Form</title>
</head>
<style>
body{
    font-size:100%;
    font-family:'Open Sans', sans-serif;
}
.form{
    border: 2px solid #000;
    padding: 20px; 
    display: flex;
    flex-direction: column;
    max-width: 300px;
    margin: 0 auto;
    border-radius: 10px;
    background-color: aquamarine;
}
.title{
    border: 2px solid black;
    text-align: center;
    border-radius: 10px;
    display: flex;
    flex-direction: column;
    padding: 10px;
    box-shadow: 5px 10px black;
}
.title h1{
    font-size: 100%;
}
.button{
    column-gap: 10px;
    display: flex;
    margin: 0 auto;
}
</style>
<body>
   <div class="main">
        <form action="proses.php" method="post" class="form">
            <div class="title">
                <h1><b>Contact Me</b></h1>
            </div>
            <p>
                <label for="name">Nama:</label><br>
                <input type="text" id="name" name="name" placeholder="Masukkan Nama Anda">
            </p>
            <p>
                <label for="email">Email:</label><br>
                <input type="text" name="email" id="email" placeholder="Masukkan Email Anda">
            </p>
            <p>
                <label for="order">Pesan:</label><br>
                <textarea name="pesan" id="pesan" cols="30" rows="10" placeholder="Masukan Pesan Anda Disini"></textarea>
            </p>
            <div class="button">
                <p align = "center">
                    <button>
                        <a href="home.html" style="text-decoration: none;">Batal</a>
                    </button>
                <p align = "center">
                    <input type="submit" value="Kirim">
                </p>
            </div>
        </form>
   </div>
</body>
</html>
```
### hasil
<img
