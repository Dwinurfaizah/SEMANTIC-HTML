# SEMANTIC-HTML
Latihan Praktikum 1 Semantic HTML

## Semantic HTML Project

1. *PERBEDAAN PADA SOURCE CODE HTML*
  A.)  Diawal tidak terdapat struktur dari meta yang nantinya akan terhubung di file css. Setelah dirubah dan diisi source code meta akan tersambung/keakses di file css serta berkesinambungan.

   <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8"/>
    <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
    <title>HTML Semantic</title>
    <link rel="stylessheet" href="./assets/styles/styles.css">

 Keterangan :

1. *<html lang="en">:*
Fungsi: Elemen <html> adalah root dari semua elemen di halaman web. Atribut lang="en" menunjukkan bahwa bahasa utama yang digunakan di dalam dokumen ini adalah bahasa Inggris (ISO code "en"). Ini membantu mesin pencari dan alat bantu seperti screen reader untuk mengerti bahasa dokumen.

2. *<head>:*
Fungsi: Bagian <head> berisi metadata atau informasi tentang dokumen HTML, seperti pengaturan karakter, judul halaman, dan referensi ke stylesheet, script, atau informasi lain yang tidak ditampilkan langsung di halaman.
   
3. *<meta charset="UTF-8"/>:*
Fungsi: Menetapkan karakter encoding untuk dokumen HTML. UTF-8 adalah format yang umum digunakan karena mendukung hampir semua karakter dari berbagai bahasa di dunia.

4. &<meta name="viewport" content="width=device-width, initial-scale=1.0"/>:*
Fungsi: Mengatur tampilan halaman agar responsif, terutama di perangkat mobile. width=device-width memastikan lebar halaman disesuaikan dengan lebar layar perangkat, dan initial-scale=1.0 memastikan skala halaman diatur ke 100% saat pertama kali dimuat.

5. *<title>HTML Semantic</title>:*
Fungsi: Menentukan judul dari halaman web, yang ditampilkan di tab browser atau hasil pencarian. Judul ini juga membantu mesin pencari memahami topik halaman.

6. *<link rel="stylesheet" href="./assets/styles/styles.css">:*
Fungsi: Menghubungkan file CSS eksternal yang mengatur gaya dan tampilan halaman HTML. Atribut href berisi jalur menuju file CSS, dalam hal ini berada di folder ./assets/styles/.
            
   
  B.) Dimodul Praktikum tidak ada pembuka dan penutup code html serta body. Setelah diperbaruhi dan diisi codenya akan berubah seperti yang dibawah :
  
<body>
<header> 
    <h1>HTML5 Semantic</h1> 
</header> 
<nav> 
  <ul> 
    <li><a href="#home">Home</a></li> 
    <li><a href="#pengertian">Pengertian</a></li>    
    <li><a href="#kesimpulan">Kesimpulan</a></li> 
  </ul> 
</nav> 
<section> 
  Konten 
</section> 
<footer> 
  Copyright 
</footer> 
</body>
</html>

Keterangan:
      1. <HTML>... </HTML> : Sebagai tanda awal dokumen HTML. 
      2.  <BODY> </BODY> Di dalam tag ini bisa diletakkan berbagai page attribute seperti warna latar 
         belakang, warna teks, warna link, warna visited link, warna active link, form, field, dan lain-      lain. 

2. *PERBEDAAN PADA SOURCE CODE CSS*

   Penempatan source code yang terbalik dan acak. Ketika sudah tertata akan seperti yang tertulis di unggahan file css.
   keterangan :
   
1. *display: grid;:*
   Fungsi: Mengubah kontainer <body> menjadi grid layout. Ini memungkinkan elemen-elemen anak (seperti          <header>, <nav>, <section>, dan <footer>) ditempatkan di dalam grid dengan cara yang lebih terstruktur.

2. *grid-template-areas:*
   Fungsi: Mendefinisikan area-area di dalam grid. Kode ini membagi halaman menjadi tiga baris:
  - Baris pertama: Semua sel diisi oleh "header".
  -Baris kedua: Sel pertama untuk "nav", dua sel berikutnya untuk "section".
  -Baris ketiga: Semua sel diisi oleh "footer".

3. *grid-template-rows: 80px 1fr 50px;:*
   Fungsi: Mengatur tinggi baris grid. Baris pertama (header) memiliki tinggi 80px, baris kedua (konten          utama, seperti nav dan section) memiliki fleksibilitas untuk memanjang sesuai ukuran konten (1fr = 1        fraction unit), dan baris ketiga (footer) memiliki tinggi 50px.
   
4. *grid-template-columns: 20% 1fr 18%;:*
   Fungsi: Mengatur lebar kolom grid. Kolom pertama (nav) memiliki lebar 20%, kolom kedua (section)             fleksibel (1fr), dan kolom ketiga (yang mungkin berisi konten tambahan) memiliki lebar 18%.
   
5. *grid-gap: 5px;:*
   Fungsi: Menambahkan jarak 5px antara setiap item grid, sehingga memberikan ruang antara elemen-elemen di dalam grid.

6. *height: 100vh;:*
   Fungsi: Mengatur tinggi halaman agar selalu memenuhi tinggi viewport (layar), 100% dari tinggi layar.

7. *margin: 10px;:*
   Fungsi: Memberikan jarak luar (margin) sebesar 10px di sekitar kontainer <body>.

8. *Elemen: header, nav, section, footer*
   padding: 5px;:
   Fungsi: Menambahkan jarak dalam (padding) sebesar 5px di dalam elemen-elemen <header>, <nav>,             <section>, dan <footer>, sehingga konten di dalam elemen tidak terlalu rapat dengan tepi elemen.

10. *<nav>*
   #1e1bc7;:
   Fungsi: Memberikan warna latar belakang biru tua pada elemen navigasi.
   - grid-area: nav;:
   Fungsi: Menempatkan elemen <nav> di area "nav" yang didefinisikan di grid-template-areas.

11. *< header >*
   background: #7e198e;:
   Fungsi: Memberikan warna latar belakang ungu pada elemen header.
   - grid-area: header;:
   Fungsi: Menempatkan elemen <header> di area "header" yang didefinisikan di grid-template-areas.
   - text-align: center;:
   Fungsi: Menyelaraskan teks yang ada di dalam elemen header ke tengah secara horizontal.

11. *< section >*
    background: #921717;:
   Fungsi: Memberikan warna latar belakang merah tua pada elemen section.
   - grid-area: section;:
   Fungsi: Menempatkan elemen <section> di area "section" yang didefinisikan di grid-template-areas.

12. *< footer >*
    background: #34023c;:
   Fungsi: Memberikan warna latar belakang ungu gelap pada elemen footer.
   - grid-area: footer;:
   Fungsi: Menempatkan elemen <footer> di area "footer" yang didefinisikan di grid-template-areas.
   - font-size: small;:
   Fungsi: Mengatur ukuran font menjadi kecil.
   - text-align: center;:
   Fungsi: Menyelaraskan teks di dalam elemen footer ke tengah.

