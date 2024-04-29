 # Percobaan Pertama
## Kode Program
```HTML
<!DOCTYPE html>
<html>
    <head>
        <title>Belajar CSS 1</title>
        <style>
            p {
                color: red;
            }
        </style>
    </head>
    <body>
        <p>Welcome CSS</p>
    </body>
</html>
```

## Hasil
![[Screenshot14.png]]

## Penjelasan
1. `<!DOCTYPE html>`: Mendefinisikan jenis dokumen HTML yang digunakan, dalam hal ini HTML5.
2. `<html>`: Elemen utama yang memuat seluruh konten dokumen.
3. `<head>`: Bagian yang berisi informasi tambahan tentang dokumen, seperti judul dan link ke stylesheet eksternal.
4. `<title>`: Menentukan judul halaman web yang akan ditampilkan di tab browser.
5. `<style>`: Bagian di mana Anda dapat menambahkan aturan CSS untuk mengubah tampilan elemen HTML di halaman.
6. `p { color: red; }`: Aturan CSS yang mengubah warna teks pada semua elemen `<p>` menjadi merah.
7. `<body>`: Bagian yang berisi konten aktual halaman web, seperti teks, gambar, atau elemen lainnya.
8. `<p>Welcome CSS</p>`: Elemen paragraf dengan teks "Welcome CSS", yang akan ditampilkan dengan warna merah karena aturan CSS yang telah ditentukan sebelumnya.

# Percobaan  Kedua

## Kode CSS
```CSS
         button {
            font-size: 20px;
            border:none;
            width: 150px;
            height: 50px;
            font-family:'sans-serif';
        }
```
## Font-size
### Before
![[CSS/aset/Screenshot(7).png]]
### After
![[CSS/aset/Screenshot(6).png]]

>[!faq]- Apa itu font-size?
>Font-size adalah property CSS yang berfungsi untuk mengatur ukuran font.

## Border
### Before
![[CSS/aset/Screenshot(7).png]]


### After
![[CSS/aset/Screenshot(6).png]]

>[!faq]- Apa itu Border?
>Border merupakan property CSS yang berguna untuk mengatur garis pinggir dari tombol.


## Font-family
### Before
![[CSS/aset/Screenshot(7).png]]
### After
![[CSS/aset/Screenshot(6).png]]

>[!faq]- Apa itu font-family?
>font-family adalah property CSS yang berfungsi untuk mengubah jenis font.

# Cara pemanggilan CSS
## IN-LINE

Penggunaan Inline CSS: CSS dapat dimasukkan langsung ke dalam atribut style pada elemen HTML. Ini adalah cara paling langsung untuk menerapkan gaya pada suatu elemen.

Contoh:

```html
<p style="font-size: 48px;">welcome css</p>
```

## INTERNAL

Penggunaan Internal CSS: CSS dapat ditulis di dalam tag `<style>` di bagian `<head>` dari dokumen HTML. Ini memungkinkan Anda untuk mendefinisikan gaya untuk seluruh halaman web.

Contoh

```html
<!DOCTYPE html>

<html>

    <head>

        <style>

            p{

                color:red

            }

            button{

                width: 150px;

                height: 50px;

                color: aqua;

                background-color: #7949ff;

                text-align: right;

            }

        </style>

        <title>DIV-SPAN</title>

    </head>
    <title>DIV-SPAN</title>

    </head>

    <body>

        <p>welcome css</p>

  

        <button>klik aku</button>

    </body>
```

## EXTERNAL

*Penggunaan External CSS*: CSS dapat disimpan di file terpisah dengan ekstensi .css dan kemudian dihubungkan ke dalam dokumen HTML menggunakan tag `<link>`. Ini memungkinkan Anda untuk memisahkan struktur dan gaya dalam pengembangan web.

Contoh 

```html
<!DOCTYPE html>

<html lang="en">

<head>

    <title>Document</title>

    <link rel="stylesheet" href="p.css">

</head>

<body>

    <p style="font-size: 48px;">welcome css</p>

  

    <h1>AND THE GANK</h1>

  

    <P class="MERAH"> INI WARNA MERAH</P>

    <P class="BIRU teks-besar"> INI WARNA BIRU</P>

    <P class="kuning poke"> INI WARNA kuning</P>

  

    <p id="HIJAU">ini warna hijau</p>

</body>

</html>
```


```css
h1{

    color: darkseagreen;

    font-size: 100px;

    font-weight: bold;

}

  

.MERAH {

    color: red;

}

.BIRU {

    color: blue;

}

.kuning {

    color: yellow;

}

 #HIJAU{

    color: green;

 }

  

.teks-besar{

    color: gold;

}

.poke {

    font-size: 40px;

}
`````



# TEXT
## Text decoration
### Penjelasan
-  `text-decoration: overline;` digunakan untuk menambahkan garis atas pada teks.
-  `text-decoration: underline;` digunakan untuk menambahkan garis bawah pada teks.
-  `text-decoration: line-through;` digunakan untuk menambahkan garis melalui pada teks. 
-  `text-decoration: none;` digunakan untuk menghapus dekorasi pada teks.
### Kode Program
```css
    .under {
     text-decoration: underline;
     }
```
### Hasil
![[CSS/aset/Screenshot(8).png]]
### Kesimpulan
Text-decoration adalah fitur CSS yang digunakan untuk menambahkan dekorasi pada teks, seperti garis bawah, garis atas, dan garis melalui.
## Text transform
### Penjelasan
- `none` (default): Menjaga kapitalisasi teks seperti pada penulisan aslinya.
- `uppercase`: Mengubah semua huruf menjadi huruf besar (uppercase).
- `lowercase`: Mengubah semua huruf menjadi huruf kecil (lowercase).
- `capitalize`: Mengubah huruf pertama setiap kata menjadi huruf besar (capitalize), mirip gaya penulisan judul.
### Kode Program
```css
 p {
    text-transform: uppercase;
  }
```
### Hasil
![[CSS/aset/Screenshot(9).png]]
### Kesimpulan 
Text-transform adalah fitur CSS yang digunakan untuk mengubah tampilan teks, seperti huruf besar, huruf kecil, dan huruf kapital.

# Background 
## Background-color
### Penjelasan
background-color merupakan properti css yang mengatur warna latar belakang halaman.
### Kode program

```css
<!DOCTYPE html>

<html lang="en">

<head>

    <style>

        body {

            background-color: #001A54;

        }

    </style>

</head>

</html>
```



### Hasil
![[CSS/aset/Screenshot(2).png]]
### Kesimpulan
Merupakan properti CSSyang memberikan warna pada latar belakang web
## Background-image
### Penjelasan
Background-image dalam CSS adalah properti yang digunakan untuk menentukan gambar yang akan digunakan sebagai latar belakang dari suatu elemen.
### Kode program
```css
<head>
<style>
body {
    background-image: url("95754.jpg");
}
</style>
</head>
<body>
<p>Hello World!</p>
</body>
```
### Hasil
![[CSS/aset/Screenshot(10).png]]
### Kesimpulan
merupakan property CSS yang dapat mengatur gambar pada latar belakang web.
## Background-repeat
### Penjelasan
Background-repeat adalah properti yang digunakan untuk mengatur gambar latar belakang yang digunakan apakah ingin di ulang atau tidak.
### Kode program
```css
<head>
<style>
body {
    background-image: url("mawar.png");
    background-repeat: no-repeat;
}
</style>
</head>
<body>
<p>Hello World!</p>
</body>
```
### Hasil
![[CSS/aset/Screenshot(11).png]]
### Kesimpulan
Background-repeat adalah properti yang digunakan untuk mengulang gambar latar belakang atau tidak.
## Background-attachament
### Penjelasan
Properti `background-attachment` digunakan untuk mengontrol apakah gambar latar belakang akan tetap diam (`fixed`) atau akan bergulir bersamaan dengan konten (`scroll`) saat pengguna menggulir halaman. Dalam contoh ini, gambar latar belakang tetap diam bahkan saat halaman digulir.
### Kode program
```css
<!DOCTYPE html>

<html>

<head>

<style>

body  {

  background-image: url("avatarlogin.png");

  background-repeat: no-repeat;

  background-attachment: fixed;

}

</style>

</head>

<body>

    <p>Nayah Comel</p>

</body>

</html>
```
### Hasil
![[Screenshot15.png]]
### Kesimpulan
background tersebut digunakan untuk  menambahkan gambar tetapi halaman tersebut tdk dapat digulir ke halaman berikutnya
# FONT
## Font-Size
### Penjelasan
`font-size` merupakan properti css yang digunakan untuk mengatur ukuran font.
### Kode program
```css
<head>
    <title>font</title>
    <style>
        .size {
    font-size: 100px;
    }  
    </style>
</head>
<body>    
    <p class="size">nayah</p>
</body>
```
### Hasil
![[CSS/aset/Screenshot(3).png]]
### Kesimpulan
font-size merupakan properti yang digunakan untuk mengatur seberapa besar atau kecil ukuran font yang di inginkan.
## font-weight
Penjelasan
`font-weight` adalah properti CSS yang dapat mengubah ketebalan sebuah teks.
### Kode program
```css
<head>
    <title>font</title>
    <style>
        .weight {
    font-weight:bolder;
    }
    </style>
</head>
<body>    
    <p class="weight">nayah</p>
</body>
```
### Hasil
![[CSS/aset/Screenshot(13).png]]
### Kesimpulan
font-weight adalah properti yang digunakan untuk mengatur ketebalan teks sesuai keinginan.


## font-style
### Penjelasan
`font-style` merupakan properti CSS yang mengatur gaya dari teks, seperti kemiringan.
### Kode program
```css
<head>
    <title>font</title>
    <style>
        .style {
    font-style:italic;
    }
    </style>
</head>
<body>    
    <p class="style">nayah</p>
</body>
```
### Hasil
![[Screenshot(4).png]]
### Kesimpulan
font-style digunakan untuk mengatur gaya dari sebuah  teks

## font-family
### Penjelasan
`font-family` adalah property CSS yang dapat mengubah jenis font suatu text.

### Kode Program
```css
.family {
font-family: 'Courier New' , Courier, monospace
}
```

### Hasil
![[CSS/aset/Screenshot(12).png]]

### Kesimpulan
Font-family adalah property CSSS yg digunakan untuk mengatur jenis text.Font-family juga dapat menampung beberapa nama font  sesuai selera,jika font pertama tidak terbaca maka font selanjutnya  akan dijalankan,Nama font harus dipisah dengan tanda koma

# Box Model

# Pseudo-classes
## Haver
### Penjelasan
Digunakan untuk mengganti tampilan elemen saat kursor mouse berada di atasnya. Ini sering digunakan untuk efek hover seperti perubahan warna latar belakang atau tampilan teks yang berubah.
## Kode Program
```css
<!DOCTYPE html>

<html>

<head>

<style>

a:hover {

  background-color: yellow;

}

</style>

</head>

<body>

  

<h1>Contoh hover</h1>

  

<p>Nayah comel</p>

<a href="https://www.wikipedia.org">wikipedia.org</a>

  

</body>

</html>
```
### Hasil
![[Screenshot16.png]]
## Active
### Penjelasan 
Digunakan untuk mengganti tampilan elemen saat elemen tersebut sedang aktif atau ditekan, seperti tombol yang sedang ditekan.
### Kode Program
```CSS
<!DOCTYPE html>

<html>

<head>

<style>

a:active {

  background-color: yellow;

}

</style>

</head>

<body>

  

<h1>Contoh Active</h1>

  

<a href="https://www.smk7mks.com">SMK 7</a><br>

  
  

</body>

</html>
```
### Hasil
![[Screenshot17.png]]

## Visited
### Penjelasan
digunakan untuk memilih tautan yang dikunjungi
###  Kode Program
```css
<!DOCTYPE html>

<html>

<head>

<style>

a:visited {

  color: pink;

}

</style>

</head>

<body>

  

<h1>Contoh Visited</h1>

  

<a href="https://www.smk7mks.com">smk7</a><br>

  

</body>

</html>
```
### Hasil
![[Screenshot18.png]]
# Transition
## Transition-property
### Penjelasan
adalah atribut yang digunakan untuk transisi yang apabila kursor didekatkan maka transisi akan berfungsi.
### Kode Program
```css
<html>

<head>

<style>

div {

  width: 100px;

  height: 100px;

  background: red;

  transition-property: width;

  transition-duration: 2s;

}

  

div:hover {

  width: 300px;

}

</style>

</head>

<body>

<div></div>

</body>

</html>
```
### Hasil
![[Screenshot19.png]]
## Transition-duration
### Penjelasan
Properti ini `transition-duration`menentukan berapa detik (s) atau milidetik (ms) yang diperlukan untuk menyelesaikan efek transisi.
### Kode Program
```css
<html>

<head>

<style>

div {

  width: 100px;

  height: 100px;

  background: red;

  transition-property: width;

  transition-duration: 5s;

}

  

div:hover {

  width: 300px;

}

</style>

</head>

<body>

<div></div>

</body>

</html>
```

### Hasil
![[Screenshot20.png]]

## Transition-timing function
### Penjelasan
Properti `transition-timing-function`menentukan kurva kecepatan efek transisi.
Properti ini memungkinkan efek transisi untuk mengubah kecepatan sepanjang durasinya
### Kode program
```css
<!DOCTYPE html>

<html>

<head>

<style>

div {

  width: 100px;

  height: 100px;

  background: blueviolet;

  transition: width 2s;

  transition-timing-function: linear;

}

  

div:hover {

  width: 300px;

}

</style>

</head>

<body>

<div></div>

</body>

</html>
```

### Hasil
![[Screenshot21.png]]
# Transform 
### Penjelasan
`Transform` adalah untuk mengubah tampilan elemen HTML, seperti menggeser, memutar, atau mengubah ukurannya ketika di klik. Ini adalah cara untuk membuat animasi sederhana atau mengatur posisi elemen dengan lebih fleksibel, atau lebih singkatnya mengubah gaya pada suatu elemen HTML ketika diklik.

### Kode Program
```css
<html>

    <head>

        <title>Home</title>

        <link rel="stylesheet" href="percobaan1.css">

    </head>

    </head>

    <body>

          <p>Klik untuk membuat dirinya menyukaimu</p>

          <button class="tombol">AYO KLIKKK!!!</button>

       </div>

    </body>

</html>


```

```css
.tombol {

    background-color: blue;

    color: white;

    border: none;

    width: 180px;

    height: 40px;

    font-size: 15px;

    border: 30px;

}

.tombol:hover {

    background-color: yellow;

    color: black;

    border: none;

    width: 160px;

    height: 40px;

    font-size: 20px;

    font-family: 'Segoe UI';

    font-weight: bold;

    border-radius: 30px;

    transition: all 0.3s ease-in;

  

}

.tombol:active {

    transform: scale(0.15);

}

```
### Hasil
![[Screenshot22 1.png]]

# Flexbox
## Justify-content
- **justify-content: space-around**
    Properti ini digunakan dalam Flexbox untuk **mengatur elemen-elemen anak di dalam wadah Flex akan didistribusikan sepanjang axis utama.** Ketika Anda mengatur `justify-content` ke `space-around`, elemen-elemen tersebut akan **didistribusikan secara merata di dalam wadah,** dengan ruang yang sama di antara mereka dan di sekitar elemen-elemen yang ada di tepi wadah.

### Kode program
```css
<!DOCTYPE html>

<html lang="en">

<head>

    <title>Justify Content</title>

    <style>

        .box{

            display: flex;

            justify-content: space-around;

        }

        .box-1 {

             background-color: blueviolet;

             width: 100px;

             height: 50px;

        }

        .box-2 {

            background-color: grey;

            width: 100px;

            height: 50px;

        }

        .box-3 {

            background-color: yellow;

            width: 100px;

            height: 50px;

        }

    </style>

</head>

<body>

    <div class="box">

        <div class="box-1">

            content-1

        </div>

    <div class="box-2">

        content-2

    </div>

    <div class="box-3">

        content-3

    </div>

    </div>

</body>

</html>
```

### Hasil
![[Screenshot23.png]]



- **justify-content: space-between**
       Dengan nilai **"space-between"** pada properti **"justify-content,"** elemen-elemen anak akan **didistribusikan secara merata di dalam wadah,** tetapi t***idak akan ada ruang di sekitar elemen-elemen yang berada di tepi wadah.*** 

### Kode Program
```css
<!DOCTYPE html>

<html lang="en">

<head>

    <title>Justify Content</title>

    <style>

        .box{

            display: flex;

            justify-content: space-between;

        }

        .box-1 {

             background-color: blueviolet;

             width: 100px;

             height: 50px;

        }

        .box-2 {

            background-color: grey;

            width: 100px;

            height: 50px;

        }

        .box-3 {

            background-color: yellow;

            width: 100px;

            height: 50px;

        }

    </style>

</head>

<body>

    <div class="box">

        <div class="box-1">

            content-1

        </div>

    <div class="box-2">

        content-2

    </div>

    <div class="box-3">

        content-3

    </div>

    </div>

</body>

</html>
```
### Hasil
![[Screenshot24.png]]

## Container
container adalah sebuah box yang didalamnya bisa jadi terdapat container lagi
- flex direction : - row ke samping
				- column ke bawah

- align item : - center rata kiri kanan 
## Item

# Tantangan Flexbox

# Position
## Relative
berpindah dari tempat asalnya
## Absolute
berpindah berdasarkan parentnya
# Tantangan Position
# Responsife
## Penjelasan
Responsive web design atau desain web responsif adalah sebuah teknik atau metode bagi
web designer untuk membuat suatu layout website yang dapat menyesuaikan diri sesuai
dengan ukuran layar pengguna. Baik dari ukuran huruf, user interface, gambar dan tata
letak akan menyesuaikan dengan lebar layar dan resolusi device yang digunakan.
Selain dapat memengaruhi apa yang ditampilkan pada perangkat tertentu, ini juga untuk
meningkatkan kenyamanan pengguna dalam mengunjungi suatu website

## Kode Program

```mysql

```
## Hasil


