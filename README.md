PENJELASAN DARI TAHAP-TAHAP PRAKTIKUM

Pertama mrmbuat folder untuk menyimpan file/project

1. Membuat dokumen HTML 
Buatlah dokumen HTML seperti berikut:
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Dasar</title>
</head>

<body>
    <header>
        <h1>CSS Internal dan <i>Inline CSS</i></h1>
    </header>
    <nav>
        <a href="lab2_css_dasar.html">CSS Dasar</a>
        <a href="lab2_css_eksternal.html">CSS Eksternal</a>
        <a  href="lab2_tag_dasar.html">HTML Dasar</a>
    </nav>
   
  
    <!--CSS ID Selector-->
    <div id="intro"> 
        <h1>Hello World</h1>
        <p></pstyle>>kami sedang belajar HTML dan CSS dasar, pada matakualiah <b>Pemograman Web</b> di 
        <i>Universitas Pelita Bangsa</i>. pelajaran pertama kami dapat adalah membuat tampilan web sederhana
        dalam rangka mengenal tag-tag dasar HTML dan CSS.</p>
        <!--css Class Selector-->
        <a class="button btn-primary" href="#intro">Informasi selengkapnya</a>
    </div>
</body>
</html>

Selanjutnya buka pada brwoser untuk melihat hasilnya dari kodingan yang telah di masukan

2. Mendeklarasikan CSS Internal 
Kemudian tambahkan deklarasi CSS internal seperti berikut pada bagian head dokumen.
<head>
    <title>CSS Dasar</title>
    <style>
        body {
            font-family: Open sans', sans-serif;
        }
        header {
            min-height: 80px;
            border-bottom: 1px solid #77CCEF;
        }
        h1 {
            font-size: 24px;
            color: #0F189F;
            text-align: center;
            padding: 20px 10px;
        }
        h1 i {
            color: #6d6a6b;
        }
    </style>
</head>
selanjutnya simpan dan refresh browser dan lihat hasilnya

3. Menambahkan Inline CSS 
Kemudian tambahkan deklarasi inline CSS pada tag <p> seperti berikut.
  
<p style="text-align: center; color: #ccd8e4;">
  
 Simpan kembali dan refresh kembali browser untuk melihat perubahannya.
 
 4. Membuat CSS Eksternal 
Buatlah file baru dengan nama style_eksternal.css kemudian buatlah deklarasi CSS seperti berikut:

nav {
    background: #20A759;
    color: #fff;
    padding: 10px;
}
nav a {
    color: #fff;
    text-decoration: none;
    padding: 10px 20px;
}
nav a.active,
nav a:hover {
    background: #0B6B3A;
}

Kemudian tambahkan tag <link> untuk merujuk file css yang sudah dibuat pada bagian <head>
  
 <head>
    <!--menyisipkan css eksternal-->
    <link rel="stylesheet" href="style_eksternal.css" type="text/css">
</head>

Selanjutnya refresh kembali browser untuk melihat perubahannya.

5. Menambahkan CSS Selector 
Selanjutnya menambahkan CSS Selector menggunakan ID dan Class Selector. Pada file style_eksternal.css, 

/* ID Selector */
#intro {
    background: #418fb1;
    border: 1p solid #099249;
    min-height: 100px;
    padding: 10px;
}
#intro h1 {
    text-align: left;
    border: 0;
    color: #fff;
}

/* class Selector */
.button {
    padding: 15px 20px;
    background: #bebcbd;
    color: #fff;
    display: inline-block;
    margin: 10px;
    text-decoration: none;
}
.btn-primary {
    background: #E42A42;
}

Kemudian simpan kembali dan refresh browser untuk melihat perubahannya pada browser.

 
