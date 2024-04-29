# Anatomi CSS
![[anatomi_css.jpg]]
# Selector
Selector dalam CSS adalah mekanisme yang memungkinkan Anda memilih elemen HTML yang akan diberi gaya atau diatur tampilannya. 
# Property
Dalam CSS, properti (properties) merujuk pada atribute yang digunakan untuk mengatur penampilan dan tata letak elemen HTML. Properti didefinisikan dalam aturan gaya CSS dan memiliki nilai tertentu yang menentukan cara elemen tersebut akan ditampilkan di halaman web.
# Property value
Dalam CSS, nilai properti (property values) adalah nilai atau sekumpulan nilai yang diberikan untuk properti tertentu. Nilai properti menentukan bagaimana elemen HTML akan ditampilkan atau diatur. 
# Percobaan Pertama
### Kode Program
```Css
p {
Color: yellow
}
```
### Hasil
![[IMG_20240304_092923.jpg]]
### Penjelasan
aturan gaya CSS yang mengatur penampilan elemen paragraf (`<p>`). 

# Percobaan ke 2
## Kode CSS
```Css
 button {
      width: 150px;
      height: 50px;
      font-size: 20px;
      border: none;
      font-weight: bold;
    }
```

## Font-size
```Css
font-size: 20px
```
### Before
![[IMG_20240219_132250 1.jpg]]

### After 
![[IMG_20240219_121128.jpg]]

### Before
![[IMG_20240219_121128 1.jpg]]
### After
![[IMG_20240219_121325.jpg]]
## Border
```css
border: none;
```
### Before
![[IMG_20240219_121325 2.jpg]]

### After
![gambar](IMG_20240219_121019.jpg)

## Font
```css
font-weight: bold;
```

# Cara Pemanggilan CSS
## Cara Pemanggilan Secara Eksternal
Pemanggilan CSS secara eksternal mengacu pada praktek menyisipkan aturan gaya CSS dari file terpisah ke dalam dokumen HTML. Ini dilakukan dengan menggunakan elemen `<link>` di bagian `<head>` dokumen HTML
## Contoh Kode Program
### Kode Html
```html
<!DOCTYPE html>
<html>
  <head>
    <title>belajar css</title>
    <link rel="stylesheet" href="Style.css">
  </head>
  
  <body>
   <p>ini menggunakan pemanggilan ekternal</p>
  </body>
  
</html>
```
---
### Kode CSS
```css
p {
color: yellow;
}
```
### Pemanggilan CSS Secara internal
Pemanggilan CSS secara internal merujuk pada penyisipan aturan gaya CSS langsung di dalam tag `<style>` di bagian `<head> `dokumen HTML
### Kode program
```html
<html>
  <head>
    <title>belajar css</title>
    <style>
    p {
    color : yellow;
    }
    </style>
  </head>
  
  <body>
   <p>ini menggunakan pemanggilan internal</p>
  </body>
  
</html>
```
## Pemanggilan CSS Secara inline
Pemanggilan CSS secara inline merujuk pada penyisipan aturan gaya CSS langsung di dalam atribut style pada tag HTML tertentu. 
### Kode Program
```html
<!DOCTYPE html>
<html>
  <head>
    <title>belajar css</title>
  </head>
  
  <body>
   <p style="color: yellow;">ini menggunakan pemanggilan inline</p>
  </body>
  
</html>
```
# Selector
## Selector Elemen
Selector Elemen dalam CSS digunakan untuk menargetkan dan menggaya elemen spesifik pada halaman web. Penulisan selector elemen cukup sederhana, di mana Anda menggunakan nama tag HTML sebagai selector untuk menentukan elemen yang akan  gaya. 
## Selector Class
Selector Class dalam CSS digunakan untuk menargetkan dan menggaya elemen-elemen yang memiliki kelas tertentu. Dengan menggunakan selector class, Anda dapat memberikan gaya kepada satu atau lebih elemen yang memiliki kelas yang sama.
## Selector Id
Selector ID dalam CSS digunakan untuk menargetkan dan menggaya elemen yang memiliki ID tertentu. ID harus unik dalam satu halaman, sehingga selector ID sangat berguna ketika Anda ingin memberikan gaya kepada elemen yang memiliki identifikasi unik

# MATERI Text
## Text Align
`text-align` dalam CSS adalah sebuah properti yang digunakan untuk mengatur penataan horisontal teks di dalam sebuah elemen. Properti ini dapat digunakan untuk mengatur posisi teks dalam konten elemen.
Contoh:
`left`: Alirkan teks ke kiri.
`right`: Alirkan teks ke kanan.
`center`: Alirkan teks ke tengah.
`justify`: Meratakan teks ke kiri dan kanan, dengan menyesuaikan spasi antarkata untuk mengisi lebar elemen.
`justify-all`: Sama seperti justify, namun juga meratakan spasi antarkata pada baris terakhir.
### Kode Program
```html
<p style="text-align:center;">menggunakan text align center</p>
```
### Hasil
![[IMG_20240304_102954.jpg]]
### Kesimpulan
Program tersebut menggambarkan penggunaan properti CSS text-align untuk mengatur penataan teks pada elemen paragraf (`<p>`). Pada contoh ini, text-align: center; diterapkan, sehingga teks di dalam paragraf akan berada di tengah 
## Text decoration
`text-decoration` dalam CSS adalah properti yang digunakan untuk mengatur dekorasi teks, seperti garis bawah, garis tengah, dan garis atas. Properti ini memungkinkan pengaturan visual tambahan pada teks.
Contoh :
`Text-decoration: Underline;`
Menambahkan garis bawah pada teks.
`text-decoration: overline;`
Menambahkan garis atas pada teks.
`text-decoration: line-through;`
Menambahkan garis tengah pada teks.
`text-decoration: none;`
Menghapus semua dekorasi teks.
### Kode program
```Html
<p style="text-decoration: overline;">menggunakan text decoration underline</p>
```
### Hasil
![[IMG_20240304_103819.jpg]]
### Kesimpulan
Program tersebut menggunakan properti CSS `text-decoration` pada elemen paragraf (`<p>`) dengan nilai `overline` untuk memberikan efek garis di atas teks.
## Text transform
**text-transform** dalam CSS adalah properti yang digunakan untuk mengontrol transformasi teks, seperti pengubahan huruf menjadi huruf kapital atau huruf kecil. Properti ini memberikan kemampuan untuk mengubah tampilan teks tanpa mengubah struktur HTML atau kontennya
Contoh :
`text-transform: uppercase:`
Mengubah seluruh huruf dalam teks menjadi huruf kapital (UPPERCASE).
`text-transform: lowercase;`
Mengubah seluruh huruf dalam teks menjadi huruf kecil (lowercase).
`text-transform: capitalize;`
Mengubah huruf pertama setiap kata dalam teks menjadi huruf kapital.
`text-transform: none;`
Tidak ada transformasi teks yang diterapkan.
### Kode Program
```html
     <p style="text-transform: uppercase;">menggunakan text transform uppercase</p>
```
### Hasil
![[IMG_20240304_105847.jpg]]
### Kesimpulan
Program tersebut menggunakan properti CSS `text-transform` pada elemen paragraf (`<p>`) dengan nilai `uppercase` untuk mengubah seluruh teks di dalamnya menjadi huruf kapital atau huruf besar.
## Text indent
**text-indent** dalam CSS adalah properti yang digunakan untuk mengatur jumlah indentasi pada awal paragraf atau baris teks. Properti ini memungkinkan penyesuaian posisi awal teks dalam suatu elemen
**text-indent**: 50px; akan membuat teks pada elemen tersebut dimulai 50 piksel dari batas kiri, menciptakan efek indentasi
### Kode program
```html
    <p style="text-indent: 50px;">menggunakan text indent 50 pixel</p>
```
### Hasil
![[IMG_20240304_104505.jpg]]
### Kesimpulan
Program tersebut menggunakan properti CSS `text-indent` pada elemen paragraf (`<p>`) dengan nilai `50px`. Properti ini digunakan untuk menetapkan indentasi teks pada awal paragraf sebesar 50 piksel dari batas kiri elemen.
Dengan demikian, ketika program dijalankan, teks di dalam paragraf akan dimulai dari posisi yang lebih ke kanan sejauh 50 piksel
## Letter-Spacing
`letter-spacing` dalam CSS adalah properti yang digunakan untuk mengatur jarak antara karakter dalam teks. Properti ini memungkinkan penyesuaian spasi antara huruf-huruf dalam suatu teks.
`Nilai positif`: Meningkatkan jarak antara karakter.
`Nilai negatif`: Mengurangi jarak antara karakter.
### Kode Program
```html
<p style="letter-spacing: 20px;">menggunakan letter spacing 20 pixel</p>
```
### Hasil
![[IMG_20240304_105145.jpg]]
### Kesimpulan
Program tersebut menggunakan properti CSS `letter-spacing` pada elemen paragraf (`<p>`) dengan nilai `20px`. Properti ini mengatur jarak antar huruf dalam teks pada paragraf tersebut.
## Line-height
`line-height` adalah properti CSS yang menentukan tinggi baris di dalam sebuah elemen. Properti ini mempengaruhi jarak vertikal antara baris teks dalam elemen tersebut. Nilai `line-height` dapat didefinisikan menggunakan nilai numerik, persentase, atau nilai non-numerik seperti normal.
### Kode Program 
```html
<p style="line-height: 100px;">menggunakan line height  100 pixel</p>
```
![[IMG_20240304_114444.jpg]]
### Kesimpulan
Program tersebut menggunakan properti CSS `line-height` pada elemen paragraf (`<p>`) dengan nilai `100px`. Properti ini mengatur tinggi baris atau jarak vertikal antara baris teks dalam paragraf tersebut.
## Word spacing
Properti `word-spacing` dalam CSS digunakan untuk mengatur jarak antara kata-kata dalam teks.
### Kode Program 
```html
<p style="word-spacing: 15px;">menggunakan word spacing 15 pixel</p>
```
### Hasil
![[IMG_20240304_114705.jpg]]
### Kesimpulan
Program tersebut menggunakan properti CSS `word-spacing` pada elemen paragraf (`<p>`) dengan nilai `15px`. Properti ini mengatur jarak antar kata dalam teks pada paragraf tersebut.
Dengan nilai `word-spacing: 15px;`, program menciptakan efek peningkatan jarak antar kata sebanyak 15 piksel. Sehingga, kata-kata dalam teks pada paragraf akan memiliki ruang lebih besar antar satu sama lain.
# Background
## Background-image
`background-image` adalah properti CSS yang digunakan untuk menentukan gambar latar belakang dari suatu elemen HTML.
### Kode Program
```html
<!DOCTYPE html>
<html>
  <head>
    <title>belajar materi background css</title>
    <style>
    p {
      background-image: url('Video,Foto,Audio/ml2.jpg');
      height: 100vh;
    }
    </style>
  </head>
  <body>
    <p>ini background image</p>
  </body>
</html>
```
### Hasil
![[IMG_20240304_115808.jpg]]
### Kesimpulan
Program tersebut mencoba mengatur background image pada elemen paragraf (`<p>`) dengan menggunakan CSS.
## Background-Size
`background-size` adalah properti CSS yang digunakan untuk menentukan ukuran dari gambar latar belakang yang diterapkan pada suatu elemen.
### Kode Program
```html
<!DOCTYPE html>
<html>
  <head>
    <title>belajar materi background css</title>
    <style>
    p {
      background-image: url('Video,Foto,Audio/ml2.jpg');
      height: 100vh;
      background-size: 50px 50px;
    }
    </style>
  </head>
  <body>
    <p>ini background image</p>
  </body>
</html>
```
### Hasil
![[IMG_20240304_120339.jpg]]
## Background-Repeat
`background-repeat` adalah properti CSS yang digunakan untuk menentukan apakah dan bagaimana gambar latar belakang diulang pada suatu elemen jika ukurannya lebih kecil daripada elemen tersebut
`repeat`: Gambar latar belakang akan diulang secara vertikal dan horizontal untuk mengisi seluruh area elemen.
`no-repeat`: Gambar latar belakang tidak akan diulang, sehingga hanya ditampilkan sekali di area elemen.
### Kode Program
### Hasil ![[IMG_20240304_122501.jpg]]
## Background-attechment
`background-attachment` adalah properti CSS yang digunakan untuk menentukan apakah gambar latar belakang akan terus bergerak atau tetap pada posisinya ketika elemen bergulir.
`scroll`: Gambar latar belakang akan bergulir bersama dengan isi halaman saat pengguna menggulir halaman.
`fixed`: Gambar latar belakang akan tetap diam relatif terhadap jendela browser, sehingga akan tetap terlihat di tempatnya saat pengguna menggulir halaman.
### Kode Program
```html
<!DOCTYPE html>
<html>
  <head>
    <title>belajar materi background css</title>
    <style>
    p {
      background-image: url('Video,Foto,Audio/ml2.jpg');
      height: 100vh;
      background-size: 50px 50px;
      background-repeat: no-repeat;
      background-attachment: fixed;
    }
    </style>
  </head>
  <body>
    <p>ini background image</p>
  </body>
</html>
```
### Hasil
![[IMG_20240304_122957.jpg]]
## Background-Position
`background-position` adalah properti CSS yang digunakan untuk menentukan posisi horizontal dan vertikal dari gambar latar belakang di dalam suatu elemen.
`top`: Menempatkan gambar latar belakang di bagian atas elemen.
`bottom`: Menempatkan gambar latar belakang di bagian bawah elemen.
`left`: Menempatkan gambar latar belakang di bagian kiri elemen.
`right`: Menempatkan gambar latar belakang di bagian kanan elemen.
`center`: Menempatkan gambar latar belakang di tengah elemen, baik secara horizontal maupun vertikal.
### Kode Program
```html
<!DOCTYPE html>
<html>
  <head>
    <title>belajar materi background css</title>
    <style>
    p {
      background-image: url('Video,Foto,Audio/ml2.jpg');
      height: 100vh;
      background-size: 50px 50px;
      background-repeat: no-repeat;
      background-attachment: fixed;
      background-position: center;
    }
    </style>
  </head>
  <body>
    <p>ini background image</p>
  </body>
</html>
```
### Hasil
![[IMG_20240304_123635.jpg]]
# MATERI FONT
## Font-size
`font-size`: Properti ini menentukan ukuran teks. Anda dapat menetapkan nilai dalam berbagai format, seperti piksel `(px)`, poin `(pt)`, persentase `(%)`, atau nilai em `(em)`.
### Kode Program

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Saya</title>
    <style>
    p {
      font-size: 70px;
    }
    </style>
  </head>
  <body>
    <p>hallo world</p>
  </body>
</html>
```
### Hasil
![[IMG_20240304_132029.jpg]]
## Font-Style
`font-style`: Properti ini menentukan gaya teks, seperti `normal` (biasa), `italic` (miring), atau `oblique` (miring dengan sudut tertentu).
### Kode Program

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Saya</title>
    <style>
    p {
      font-size: 70px;
      font-style: italic;
    }
    </style>
  </head>
  <body>
    <p>hallo world</p>
  </body>
</html>
```

### Hasil
![[IMG_20240304_132401.jpg]]
## Font-weight
`font-weight`: Properti ini menentukan ketebalan teks. Nilai umum termasuk `normal`,` bold`, atau menggunakan nilai numerik seperti `400` untuk normal dan `700` untuk bold.
### Kode Program
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Saya</title>
    <style>
    p {
      font-size: 70px;
      font-style: italic;
      font-weight: bold;
    }
    </style>
  </head>
  <body>
    <p>hallo world</p>
  </body>
</html>
```
### Hasil
![[IMG_20240304_132516.jpg]]
## Font-family
`font-family`: Properti ini menentukan jenis font atau keluarga font yang akan digunakan. Anda dapat menyediakan beberapa jenis font sebagai alternatif jika jenis font utama tidak tersedia.
### Kode Program
```css
    p {
      font-family: Times New Roman;
    }
```
### Hasil
![[IMG_20240304_132840.jpg]]
# Box Model
## Materi height & width

### Penjelasan
Model kotak (Box Model) dalam CSS adalah konsep fundamental yang menggambarkan bagaimana setiap elemen HTML dianggap sebagai sebuah kotak yang terdiri dari beberapa komponen. Model ini memandu cara elemen tersebut diposisikan, diatur ukurannya, dan berinteraksi dengan elemen lain dalam tata letak halaman web.

**•Height**: Properti ini menentukan tinggi (height) dari elemen. Anda dapat menetapkan nilai dalam satuan seperti piksel (px), persentase (%), poin (pt), atau em (em), tergantung pada preferensi Anda.
•**Width:**
Properti ini menentukan lebar (width) dari elemen. Seperti height, Anda dapat menetapkan nilai dalam berbagai satuan.
### Kode Program
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Saya</title>
    <style>
    button {
      width: 75px;
      height: 25px;
    }
    </style>
  </head>
  <body>
    <button>Klik Aku!</button>
  </body>
</html>
```
### Hasil
![[IMG_20240304_134242.jpg]]
## Materi Border 
### Border-width
#### Penjelasan
border-width adalah properti CSS yang digunakan untuk menentukan lebar dari border pada elemen HTML. Nilai yang dapat digunakan termasuk px (pixel), em, rem, atau persentase. Misalnya, border-width: 2px; akan mengatur lebar border menjadi 2 pixel. 
#### Kode Program
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Box Model CSS</title>
    <style>
    button {
      border-width: 2px;
    }
    </style>
  </head>
  <body>
    <button>Klik Aku!</button>
  </body>
</html>
```
#### Hasil
![[IMG_20240304_135438.jpg]]
## Border-style
#### Penjelasan
**border-style** adalah properti CSS yang digunakan untuk menentukan jenis atau gaya dari border pada elemen HTML. Properti ini memungkinkan Anda mengatur bagaimana border akan ditampilkan di sekeliling elemen. Beberapa nilai umum untuk border-style melibatkan jenis garis seperti:

**•solid**: Border berupa garis lurus dan penuh.
**•dashed**: Border berupa garis putus-putus.
**•dotted**: Border berupa titik-titik.
**•double**: Border berupa dua garis paralel.
#### Kode Program
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Box Model CSS</title>
    <style>
    button {
      border-style: double;
    }
    </style>
  </head>
  <body>
    <button>Klik Aku!</button>
  </body>
</html>
```
#### Hasil
![[IMG_20240304_140646.jpg]]
## Border-color
### Penjelasan
border-color adalah properti CSS yang digunakan untuk menentukan warna dari border pada elemen HTML.
### Kode Program

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Box Model CSS</title>
    <style>
    button {
      Border-color: green;
    }
    </style>
  </head>
  <body>
    <button>Klik Aku!</button>
  </body>
</html>
```

## Border-radius
### Penjelasan
`border-radius` adalah properti CSS yang digunakan untuk menentukan sudut lengkungan dari sudut-sudut border pada elemen HTML, sehingga menciptakan efek lengkungan atau melengkung pada elemen tersebut. Properti ini memungkinkan Anda untuk memberikan elemen tampilan yang lebih lembut dan modern
Contoh penggunaan:

**border-radius**: 10px; akan memberikan sudut lengkungan sebanyak 10 piksel pada keempat sudut elemen.
**border-radius**: 5px 15px; akan memberikan sudut lengkungan 5 piksel pada sudut atas kiri dan sudut bawah kanan, serta 15 piksel pada sudut atas kanan dan sudut bawah kiri.
**border-radius**: 50%; akan memberikan elemen bentuk bulat sepenuhnya, karena sudut lengkungan akan sejajar dengan setengah dari lebar atau tinggi elemen.
### Kode program
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Box Model CSS</title>
    <style>
    button {
      Border-radius: 15px 5px;
    }
    </style>
  </head>
  <body>
    <button>Klik Aku!</button>
  </body>
</html>
```
### Hasil
![[IMG_20240304_142826.jpg]]
# Materi Padding
## Padding-right
### Penjelasan
`padding-right `adalah properti CSS yang digunakan untuk menentukan ruang atau jarak antara batas dalam elemen dan kontennya pada sisi kanan elemen tersebut. Properti ini mengatur seberapa besar "padding" atau ruang tambahan pada sisi kanan elemen.

**Contoh penggunaan:**

`padding-right`: 10px; akan memberikan padding sebesar 10 piksel hanya pada sisi kanan elemen.
`padding-right`: 5%; akan memberikan padding sebesar 5% dari lebar elemen pada sisi kanan.
### Kode Program
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Saya</title>
    <style>
    button {
      padding-right: 100px;
    }
    </style>
  </head>
  <body>
    <button>Klik Aku!</button>
  </body>
</html>
```
### Hasil
![[IMG_20240304_222959 1.jpg]]
### Kesimpulan
## Padding-left
### Penjelasan
`padding-left` adalah properti CSS yang digunakan untuk menentukan ruang atau jarak antara batas dalam elemen dan kontennya pada sisi kiri elemen tersebut. Properti ini mengatur seberapa besar "padding" atau ruang tambahan pada sisi kiri elemen.

**Contoh penggunaan**:

`padding-left`: 10px; akan memberikan padding sebesar 10 piksel hanya pada sisi kiri elemen.
`padding-left`: 5%; akan memberikan padding sebesar 5% dari lebar elemen pada sisi kiri.
### Kode Program
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Saya</title>
    <style>
    button {
      padding-left: 75px;
    }
    </style>
  </head>
  <body>
    <button>Klik Aku!</button>
  </body>
</html>
```
### Hasil
![[IMG_20240304_223026.jpg]]
### Kesimpulan
## Padding-bottom
### Penjelasan
margin adalah properti CSS yang digunakan untuk menentukan ruang atau jarak antara batas luar elemen dengan elemen-elemen di sekitarnya. Properti ini mengontrol seberapa besar "margin" atau celah yang ada di sekitar elemen tersebut.

**Contoh penggunaan:**

`margin: 10px`; akan memberikan margin sebesar 10 piksel pada keempat sisi elemen.
`margin: 5px