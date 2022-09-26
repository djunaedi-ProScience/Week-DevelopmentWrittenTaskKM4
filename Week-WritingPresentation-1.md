# Week Presentation 1
---

## Unix Command Line
- CLI (Command Line Interface)
  Merupakan sebuah program yang memungkinkan user mengetik perintah atau command yang akan mmemerintahkan perangkat komputer untuk melakukan suatu tugas tertentu.
- Shell
  Agar bisa terhubung dengan komputer maka user akan memerlukan penerjemah. Maka dari itu user memerlukan yang namanya shell. Definisi shell secara harfiah sendiri adalah program yang digunakan untuk berkomunikasi atau memerintah sistem.
- Terminal
  User dan komputer dihubungkan dengan namanya terminal, yaitu tempat/aplikasi dimana user dapat mengetikan atau memberikan suatu perintah. Disinilah tempat dimana shell akan berperan.
- Structure File
Dalam Unix Seperti Akar Pohon dan dalam windows dari akar pohon dan banyak cabang
- **Command**    
  - pwd (print working directory), untuk melihat current working directory
  - dir (directory), untuk melihat directory
  - cd (change directory), untuk pindah directory
  - ls (list), untuk melihat isi file di dalam directory
  - touch, untuk membuat file directory
  - cp (copy), untuk menyalin file directory
  - mv (move), untuk memindahkan file directory
  - rm (remove), untuk menghapus file directory

## Git & Github
  - __Penjelasan Git & Github__
  
     - Git    
     Merupakan aplikasi yang dapat melacaks suatu perubahan yang terjadi di suatu folder ataupun file, yang biasanya digunakan oleh programmer sebagai tempat untuk menyimpan file programan mereka karena lebih efektif.
     - Github  
     Merupakan vendor penyedia layanan git yang dimiliki oleh microsoft atau secara definisi merupakan layanan hosting berbasis web sebagai repositori git.
  - __Perbedaan Git & Github__    
  Mengapa wajib menggunakan Git & Github?
Alasan utamanya adalah sepandai apapun programmer, tidak akan mampu untuk mengerjakan semuanya sendiri selamanya. Maka dari itu dengan menggunakan Git & Github akan memudahkan programmer untuk bisa bekerja sama dalam sebuah tim. Tujuan besarnya adalah programmer bisa berkolaborasi dengan programmer lainnya dengan mengerjakan proyek yang sama tanpa harus repot copy paste folder aplikasi yang terupdate.

### command dalam Git 
  - SETUP  
```sh
tetapkan nama yang dapat diidentifikasi untuk kredit saat meninjau riwayat versi

git config --global user.name “[firstname lastname]”
atur alamat email yang akan dikaitkan dengan setiap penanda riwayat

git config --global user.email “[valid-email]”
```

- SETUP & INIT    


```sh
inisialisasi direktori yang ada sebagai repositori Git

**git init**
ambil seluruh repositori dari lokasi yang dihosting melalui URL

**git clone [url]**

```

### STAGE & SNAPSHOT    
Bekerja dengan snapshot dan area pementasan Git

tampilkan file yang dimodifikasi di direktori kerja, dipentaskan untuk komit Anda berikutnya
```sh

git status

```
tambahkan file seperti yang terlihat sekarang ke komit Anda (tahap) berikutnya

```sh

git add [file]

```
unstage file sambil mempertahankan perubahan di direktori kerja

```sh

git reset [file]

```
komit konten Anda yang dipentaskan sebagai snapshot komit baru
```sh

git commit -m “[descriptive message]”

```

Mengirimkan komit cabang lokal ke cabang repositori jarak jauh
```sh

git push [alias] [branch]

```

## HTML 

### Apa itu Html
>Merupakan bahasa komputer yang digunakan untuk membuat kerangka atau struktur untuk Web pages (halaman website) di internet. Bagaimana peran HTML pada web development? Web browser seperti Chrome, Firefox, Edge, Safari, atau Opera akan membaca dokumen HTML. Dokumen HTML yang berisi tag-tag HTML akan memberitahu browser bagaimana cara menampilkan sebuah konten

### Membuat HTML
```sh
<html>
<head>
<title>
    Judul Website
  </title>
<body>
    saya sedang belajar pemrograman HTML dasar.
  </body>
</html>
```

### Menyiapkan Tools Pendukung
![ini gambar](https://github.com/djunaedi-ProScience/Week-DevelopmentWrittenTaskKM4/blob/main/imgWeekPresentation/LiveServer.png?raw=true)

### Membuat tag html sederhana

```sh
<ul>
  Dafunda
  <li>Dafunda Tekno</li>
  <li>Dafunda Otaku</li>
  <li>Dafunda Games</li>
</ul>
```

__Tampilkan Ke Live Server__
![liveServer](https://github.com/djunaedi-ProScience/Week-DevelopmentWrittenTaskKM4/blob/main/imgWeekPresentation/golive.png?raw=true)

### Deploy HTML

Deploy adalah sebuah proses untuk menyebarkan aplikasi yang sudah kita kerjakan supaya bisa digunakan oleh orang-orang. Jika aplikasi kita HTML atau Web App kita perlu mendeploy ke server. Untuk melakukan hal tersebut kita bisa menggunakan layanan yang bernama Netlify

## CSS
-__Definisi CSS__

>CSS adalah bahasa komputer yang digunakan untuk menambahkan design ke suatu halaman website di internet agar terlihat lebih cantik/menarik. CSS adalah singkatan dari Cascading Style Sheets. Kita ibaratkan HTML adalah kerangka yang memberi sturuktur pada website, maka CSS adalah baju yang memberi warna dan layout pada website.

### Inline CSS
Ada 3 cara untuk menyisipkan CSS ke dalam HTML, yaitu:

 1 Inline CSS, yaitu menggunakan attribute style untuk menyisipkan kode CSS langsung di dalam HTML element.

2 Internal CSS, yaitu menggunakan element <style> untuk menyisipkan kode CSS. Element </style>          tersebut diletakkan di dalam element .   

3 External CSS, yaitu sebuah file CSS terpisah yang disambungkan dengan file HTML dengan menggunakan   element <link>.

__cara menyisipkan CSS ke dalam HTML__
`inline`
```sh
<!DOCTYPE html>
<html>
  <head>
    <title>
      Website Pertamaku
    </title>
  </head>
  <body>
    <h1 style="color:blue;">Selamat Datang</h1>
  </body>
</html>
```

__internal__
```sh
<!DOCTYPE html>
<html>
  <head>
    <title>Website Pertamaku</title>
    <style>
      body {
        background-color: yellow;
      }
      h1 {
        color: blue;
      }
      p {
        color: red;
      }
    </style>
  </head>
  <body>
    <h1>Website Pertamaku</h1>
    <p>Selamat Datang</p>
  </body>
</html>
```

eksternal

```sh
<!-- File index.html -->
<!DOCTYPE html>
<html>
  <head>
    <title>Website Pertamaku</title>
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <h1>Website Pertamaku</h1>
    <p>Selamat Datang</p>
  </body>
</html>
/* File styles.css */
body {
  background-color: pink;
}
h1 {
  color: blue;
}
p {
  color: black;
}
```

__menyisipkan eksternal__
> <head>
    <title>Website Pertamaku</title>
    <link rel="stylesheet" href="style1.css" />
    <link rel="stylesheet" href="style2.css" />
  </head>
  
### CSS Syntax

CSS Syntax adalah syntax yang digunakan untuk menunjuk atau memilih HTML element mana yang ingin diberi style (dihias). CSS syntax terdiri dari selector, property, dan value.

Syntaxnya seperti ini:

>selector {
  property: value;
}

Pseudo Class
Syntax saat menggunakan pseudo-class adalah sebagai berikut:

>selector:pseudo-class {
  property: nilai;
}

### Flexbox
adalah cara untuk **mengatur layout**

Flexbox memiliki 1 parent/container dan bisa beberapa child/item
>.container {
  display: flex; /* or inline-flex */
}

>.container {
  flex-direction: row | row-reverse | column | column-reverse;
}

>.container {
  flex-wrap: nowrap | wrap | wrap-reverse;
}

>.container {
  justify-content: flex-start | flex-end | center | space-between | space-around | space-evenly | start | end | left | right ... + safe | unsafe;
}

Properties for the Children
>.item {
  order: 5; /* default is 0 */
}

>.item {
  flex-shrink: 3; /* default 1 */
}

>.item {
  flex-grow: 4; /* default 0 */
}

>.item {
  align-self: auto | flex-start | flex-end | center | baseline | stretch;
}

## __Algoritma__

Algortima Adalah deskripsi berupa step-step yang dibutuhkan untuk menyelesaikan suatu masalah. Untuk menyelesaikan suatu masalah, tentunya kita harus mempunyai data struktur, nah data inilah yang akan kita gunakan untuk menyelesaikan suatu masalah dengan menggunakan algoritma.
 

__Mengapa kita memerlukan algoritma?__

- Manfaat algoritma antara lain:

    Membantu menyederhanakan suatu program yang rumit dan juga besar.
Mempermudah pembuatan program yang dapat menyelesaikan masalah tertentu.
Membantu menyelesaikan suatu masalah dengan logika dan juga sistematis.
 

### Kualitas Algortima

- __Kualitas wajib dari algoritma__

    Input dan output harus didefinisikan terlebih dahulu dengan tepat
Setiap step harus benar-benar clear dan tidak ambigu
Algoritma seharusnya tidak mengandung suatu code pada bahasa pemograman tertentu.
Algoritma harus dibuat agar dapat digunakan dalam bahasa pemograman apapun.
 

### Penggunaan Algortima

#### __Soal__

Buatlah Algoritma untuk menyelesaikan problem ini
David memiliki program yang membutuhkan untuk convert data dari jumlah jam ke detik

Contohnya jika program memiliki input 2 jam maka output yang diharapkan adalah 7200 detik

Jawaban
```sh
Mulai
Deklarasi variabel n, hasil_convert
Menambahkan nilai n
Melakukan proses (n jam = n \* 3600" lalu disimpan ke dalam hasil_convert
Menampilkan hasil convert (n jam) = + "detik"
Stop
```

### __Pseudocode__

Pseudocode adalah menuliskan algoritma sebelum kita implementasikan ke bahasa pemograman tertentu.
 

Bagaimana menulis pseudocode
```sh
Menggunakan HURUF BESAR pada kata kunci (key commands).
CONTOH: IF number is > 10 THEN …

1 statement = 1 baris

Gunakan indentasi

Simpel

Contoh :

STORE "width" with any number
STORE "height" with any nummber
STORE "area" without any value

CALCULATE "width" times "height"
SET "area" value with calculation result
DISPLAY "area"
``` 

Pseudocode berdasarkan kondisi masalah

### **Procedural**

Procedural adalah cara berpikir secara runtun. Artinya serangkaian perintah yang berurutan.

Contoh :
```sh
STORE "width" with any number
STORE "height" with any nummber
STORE "area" without any value

CALCULATE "width" times "height"
SET "area" value with calculation result
DISPLAY "area"
``` 

### Conditional

Conditional digunakan saat dibutuhkan percabangan kasus. Komputer akan melakukan suatu tindakan jika suatu kondisi terpenuhi.

Jika hari ini tidak hujan, maka Bob pergi ke pasar,

jika tidak maka Bob dirumah aja.
```sh
IF "bright"
DO "go to the market"
ELSE
DO "stay at home"
``` 

### Looping

Komputer dapat melakukan sebuah proses yang sama berulang-ulang.

Jika membutuhkan perulangan dalam kasus tertentu, kita bisa menggunakan Looping.

Contoh :
```sh
STORE "count" t0 1

WHILE "count" < 11
DISPLAY "count"
CALCULATE "count" mod 2
STORE "reminder" value with calculation result
IF "reminder" equals to 0
DISPLAY "EVEN!"
ELSE
DISPLAY "ODD!"
``` 

### Recursive

Recursive adalah pola pikir dalam algoritma yang memanggil method/function didalam sebuah function

## Javascript Dasar


### JavaScript Introduction     

__Javascript__ merupakan bahasa pemrograman yang digunakan untuk membuat suatu website menjadi interaktif
Cara menjalankan javascript adalah melalui berbagai browser. Namun mozilla dan google chrome merupakan browser yang paling umum digunakan.


---
Pada Javascript dikenal dengan istilah Syntax dan Statement
Syntax adalah sesuatu yang dapat diibaratkan sebagai kamus dan berperan dalam mengatur tata cara dalam bahasa pemrograman. Syntax digunakan untuk membuat statement program, instruksi untuk dijalankan atau dieksekusi oleh web browser dan compiler.
```sh
### Contoh Syntax Java Script
Alert
Prompt
confirm
Console Log adalah tempat untuk melakukan pengecekan logic pemrograman serta pemeriksaaan apakah terdapat error atau tidak pada pemrograman.
```
```sh
Comments
Single Comments: //
Multiline Comments: /* */
```
### Tipe Data

__Ada 6 macam tipe data fundamaental pada javascript yaitu :__
1 Number : tipe data yang mengandung semua jenis angka.
2 Tipe data number ada 2 macam yaitu integer (terdiri dari bilangan bulat positif atau negatif) dan 3 3 float (terdiri dari bilangan desimal)
4 String : tipe data yang terdiri dari huruf, angka, spasi maupun simbol

__Tipe data string ada 2 macam yaitu char dan__
1 Boolean : tipe data yang memiliki nilai true or false
2 Null : tipe data pada sebuah data/variabel yang tidak memiliki nilai
3 Undefined : tipe data yang merepresentasikan varibel/data yang tidak memiliki nilai
4 Object : tipe data yg dapat berisi berbagai nilai dan berhubungan dengan dunia nyata

**Variabel merupakan wadah atau tempat untuk menyimpan sebuah nilai 3 hal yang dapat dilakukan pada variabel:**
1 variabel harus dibuat dengan nama yang jelas dan menggabarkan tentang data tersebut
2 variabel dapat menimpan dan mengupdate informasi data yang disimpan
3 variabel digunakan untuk menampilkan atau mendapatkan data yang tersimpan
__Ada 3 cara untuk mendefinisikan variabel yaitu :__
1 var
2 let
3 const

__Aturan Penamaan variabel yaitu :__
Harus mendeskripsikan dengan jelas tentang data yang disimpan
Tidak bisa menggunakan angka diawal variabel
Menggunakan camelcase untuk nama variabel yg lebih dari 1 kata
__Operator__
>Assignment Operator (=) digunakan untuk menyimpan sebuah nilai pada variabel contohnya : let myName = 'Chaca'

__Mathematical Assignment Operator__
```sh
>contohnya :
>  let x = 10 ; 
>  x *= 2 ; 
>  console.log(x) // Output: 20
>Increment dan Decrement digunakan untuk menambah atau mengurangi sebesar 1 nilai
>contohnya :
>let a = 10;
>a++
>  console.log(a) // output: 11
>Arithmetic Operator digunakan apabila melibatkan operasi matematika
>Pertambahan (+)
>Pengurangan (-)
>Perkalian (*)
>Pembagian (/)
>Modulus (%)
```
__Comparism Operator digunakan untuk membandingkan suatu nilai__
```sh
>Lebih Besar (>)
>Lebih Kecil (<)
>Lebih kecil atau samadengan (<=)
>Lebih besar atau samadengan (>=)
>Samadengan (===)
>Tidak Sama dengan (!==)
>Logical Operator digunakan untuk sebuah kondisi
>AND operator (&&)
>OR operator (||)
>NOT operator (!)
```

### Javascript Conditions
#### __syntax__
```sh
if (condition){
    logic
}

condition 2

if (condition){
    
} else{
    
}

condition 3

if (condition){
    
} else if (){
    
}else{
    
}
```
# ___TerimaKasih___




 

