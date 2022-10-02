## Javascript Dasar

#Rekaman Week2 : https://drive.google.com/drive/folders/1mCQGHpYbrbhGgf-mfNAp5AJqHB7AcNPz?usp=sharing

### Loop        
Loop dalam Bahasa Indonesia artinya putaran. Dalam JavaScript,

__Ada 5 jenis loop di JavaScript, yaitu:__

>for        
>for...in       
>for...of       
>while      
>do...while     

### __Syntax yang digunakan ketika menggunakan for loop adalah sebagai berikut:__
```sh
for (pernyataan1; pernyataan2; pernyataan3) {
  // kode yang akan dijalankan ketika pernyataan2 benar (true)
}
```

Penjelasan kode di atas:

- pernyataan1 digunakan untuk menentukan nilai awal berjalannya loop.
- pernyataan2 digunakan untuk mendefinisikan kondisi berjalannya sebuah loop. Apabila nilai kondisinya false, maka loop akan berakhir.
- pernyataan3 digunakan untuk menambah atau mengurangi nilai awal pada pernyataan1 setiap kali loop dijalankan.


### For/In Loop
Berbeda dengan for loop dari topik sebelumnya, for...in digunakan untuk mengulang setiap properti dari sebuah objek.

```sh
for (propertiObjek in namaObjek) {
  // kode yang akan dijalankan
}
```

### For/Of Loop
Berbeda dengan for loop dari topik sebelumnya, for...of digunakan untuk mengulang setiap element dari objek yang bisa diulang (contoh array atau string).

Syntax yang digunakan ketika menggunakan for...of loop adalah sebagai berikut:
```sh
for (let element of namaVariabel) {
  // kode yang akan dijalankan
}

```


#### Penjelasan kode di atas:

- `for (let element of namaVariabel)` berarti untuk setiap element di namaVariabel, maka jalankan kode di dalam {}. Variabel element bisa diganti dengan nama variabel apapun.
- 


## While
Syntax dalam menggunakan while loop adalah sebagai berikut:


```sh
while (kondisi) {
  // kode yang akan dijalankan ketika kondisi benar (true)
}
```
Penjelasan kode di atas:

- while (kondisi) berarti ketika kondisi yang ditentukan benar (true), maka jalankan semua kode yang ada di dalam {}.
- 

### Do While Loop


Fungsi melakukan perulangan lalu cek kondisi
Syntax dalam penggunaan do...while loop adalah:


```sh
do {
  // kode yang akan dijalankan ketika kondisi benar (true)
} while (kondisi);
```

### Function
 cara buat function ada 3
 ```sh
// 1 - function clasic =============
// function myFunction(kondisi) { }

// 2 - fanction variable =============
// let myFunction = function (kondisi) { }

// 3 - arrow function =============
// let myFunction = (kondisi) => { }
```


Fungsi dapat dipanggil cukup dengan menambahkan tanda kurung () setelah nama fungsi tersebut. Dalam dua contoh di atas, pemanggilan fungsinya adalah sebagai berikut:


```sh
namaFungsi();

namaVariabelFungsi();
```

`Parameter` adalah syarat input yang harus dimasukkan ke dalam suatu fungsi dan dideklarasikan bersama dengan deklarasi fungsi. Sementara argument adalah nilai yang dimasukan ke dalam suatu fungsi, sesuai dengan persyaratan parameter, di mana argument dituliskan bersamaan dengan pemanggilan fungsi.

Bisa digambarkan seperti ini:


```sh
function operasiPerkalian(angka1, angka2){
  return angka1 * angka2;
}

console.log(operasiPerkalian(2, 6)) // Output: 12
```

### Scope
**Scope** adalah konsep dalam flow data variabel
Analoginya seperti
Kita semua bisa melihat bintang-bintang dilangit karena bumi bersifat global.

Namun jika kamu tinggal di Bandung, kamu tidak akan bisa melihat monas yang berada di jakarta. Monas bersifat local yaitu hanya berada di Jakarta.

**Global scope** berarti variabel yang kita buat dapat diakses dimanapun dalam suatu file.
**Local scope** berarti kita mendeklarasikan variabel didalam blocks seperti function, conditional, dan looping.

### **Blocks**
Blocks adalah code yang berada didalam curly braces {}
contoh
Conditional, function, dan  looping menggunakan blocks.

## JavaScript data types and data structures
JavaScript types
Himpunan tipe dalam bahasa JavaScript terdiri dari nilai dan objek primitif.

#### Nilai primitif
Semua jenis kecuali objek mendefinisikan nilai yang tidak dapat diubah (yaitu, nilai yang tidak dapat diubah). Misalnya, String tidak dapat diubah. Kami menyebut nilai jenis ini sebagai "nilai primitif".

#### Boolean type
Boolean mewakili entitas logis dan dapat memiliki dua nilai: benar dan salah.

#### Null type

Tipe Null memiliki tepat satu nilai: null.

#### Undefined type
variabel yang belum diberi nilai memiliki nilai yang tidak terdefinisi

#### String type
Objek String digunakan untuk mewakili dan memanipulasi urutan karakter.


## Membuat Properti dan Method dari String tipe 


```sh
// ====================== String ===============================
let hewan = "kAnCIl"

mengecek tipe data string
console.log(typeof hewan)

// properties
console.log(hewan.length);

// built-in method
Membuat huruf lebih besar
console.log(hewan.toUpperCase())
Membuat huruf lebih kecil
console.log(hewan.toLowerCase())

mengambil 1 character
console.log(hewan.charAt(1))
console.log(hewan[1])

// kAnCIl
console.log(hewan.includes("s"))

let kalimat = "dengan menggunakan split(), kita dapat memisahkan sebuah string menjadi data array"
console.log("BEFORE", kalimat)
console.log("AFTER", kalimat.split(" "));


```

## membuat properti dan method dari tipe Number

```javascript
// ==================== Number ===========================

console.log(Number("123")); // 123 in Number

console.log(isNaN(2131)) // false
console.log(isNaN("dawdf")) // true

let angka = 3.12345
console.log(angka.toFixed(1)) // 3.1
console.log(angka.toFixed(2)) // 3.12
```


### Mencoba properti dan method bawaan libary math

```javascript
// ========================= Math  ==============================

// properties
console.log(Math.PI)

// method
console.log(Math.abs(-5)) // 5
console.log(Math.ceil(5.2)) // 6
console.log(Math.floor(5.6)) // 5
console.log(Math.round(5.6)) // 6
console.log(Math.round(5.2)) // 5
console.log(Math.random()) // 0.123342

```


### properti dan method bawaan Date
```javascript
// ====================== Date  ============================

console.log(Date()) // 'Tue Sep 27 2022 20:31:20 GMT+0700 (Indochina Time)'
console.log(Date.now()) // 1664285495449

let date = new Date()
console.log(date.getDay()); 
console.log(date.getFullYear()); // 2022


```

## membuat fungsi baru menggunakan protoype

```javascript
// ==================== prototype ========================

// kasus
// hallo -> ollah

// membuat method baru utk tipe data string
String.prototype.reverse = function(){
  let s = ""
  for (let i = String(this).length-1; i >= 0 ; i--) {
    s = s + String(this)[i]
  }

  return s
}

// method yg dimiliki oleh string
console.log("hallo".reverse())
console.log("selamat datang".reverse())

// function dgn argumen string
// console.log(reverse("hallo"));
```


## DOM
DOM bukan bagian dari JavaScript, 
melainkan browser (Web API)

Gunakan Defer untuk mencegah pasing html berhenti atau taruh di akhir `<script>` buat mengghindari html gagal di download

***Perbandingan innerHTML dan textContent***
Inner html
>Harus dibandingkan dengan .textContent sebelumnya, misal kalau pakai textContent kita tambahin ><h1>asdasd</h1>
itu nanti di webpagenya beneran tertulis 
>“<h1>asdads</h1>”. 
Sedangkan kalau pakai .innerHTML kan kasilnya “asdasd” jadi heading

## Cara akses element DOM

```javascript
// getElement family........................
let title = document.getElementById("title")
console.log(title)

let items = document.getElementsByClassName("item")
console.log(items[2]);

let list = document.getElementsByClassName("list")
console.log(list[0])
console.log(list[0].children)

let itemByTag = document.getElementsByTagName("li")
console.log(itemByTag[1])
console.log(itemByTag.item(1))
console.log(itemByTag.length)
```

### Akses lewat query

```Javascript
// query selector family...................
let listQuery = document.querySelector(".list")
console.log(listQuery);

let itemQueryAll = document.querySelectorAll(".item")
console.log(itemQueryAll)

for (let i = 0; i < itemQueryAll.length; i++) {
  console.log(itemQueryAll[i])
}

let itemQuery = document.querySelector(".item")
console.log(itemQuery);
```

### akses element parent

```sh
// ===================== traversing ke atas =======================

console.log(itemQuery.parentElement);
console.log(itemQuery.closest(".list"));


### akses element disamping
// ===================== traversing ke samping =====================

console.log(itemQuery.previousElementSiblingc);
console.log(itemQuery.nextElementSibling);
```

### DOM Manipulasi

```sh
let app = document.getElementById("app")

// =========== memberikan content ============
// app.innerText = "<h1>apa kabs</h1>"
app.innerHTML = "<h1>Hallo</h1>"

// ========== membuat element ===============
let p = document.createElement("p")
p.innerText = "ini adalah paragraf"

// menambahkan child kedalam parent
app.append(p)

// proses yg sama
let p2 = document.createElement("p")
p2.innerText = "paragraf ke-2"
app.appendChild(p2)

// append vs appendChild
// appendChild ga bisa input data string
app.append("menggunakan append")
// app.appendChild("appendChild") // error

// =============== remove element ==========
let end = document.getElementById("end")
end.remove()

let link = document.getElementsByClassName("link")[0]

// =============== attribute ======================
console.log(link.attributes) // [] list attribute
console.log(link.getAttribute("href")); // ambil isi attribute
link.setAttribute("id", "google") // add attribute


// =============== memberikan style =====================
link.style.color = "black"
link.style.border = "1px solid black"
link.style.padding = "5px 20px"
link.style.backgroundColor = "aqua"
link.style.removeProperty("border") // menghapus style property

// =============== mendapatkan style dari element =======
let tess = document.getElementById("tess")
let tessStyle = getComputedStyle(tess)
console.log(tessStyle.height)


// =============== class =======================
let container = document.getElementsByClassName("container")[0]
console.log(container.classList); // [] list of class
container.classList.add("home") // menambahnkan class
container.classList.remove("container") // menghapus class
```

## DOM Event
__event__ = interaksi yg dilakukan user pada website

### Cara pakai DOM events
```sh
let paragraf = document.getElementById("paragraf")

// cara ke-2 
paragraf.onclick = function () {
  alert("ini dari paragraf")
}
// paragraf.onclick = tampilkanAlert

function tampilkanAlert () {
  alert("ini alert")
}

// cara ke-3
// addEventListener bisa multiple event
let button = document.getElementById("btn")
button.addEventListener("click", function (event) {
  console.log(event.target)
  alert("ini dari button")
})

// button.addEventListener("click", function () {
//   confirm("apakah ini dari button?")
// })
```

**Project 1**
Menyiapkan HTML Form
```sh
<div class="container">
      <form id="sign-in">
        <h1>Sign In</h1>

        <div class="field">
          <label for="username">username</label>
          <input type="text" id="username" name="username" />
        </div>

        <div class="field">
          <label for="password">password</label>
          <input type="text" id="password" name="password" />
        </div>

        <button type="submit">login</button>
      </form>
```

### Menyiapkan JS

```sh
let loginForm = document.querySelector("#sign-in")
let inputUsername = document.querySelector('#username')
let inputPassword = document.querySelector('#password')

let user = {
  username: "auzan",
  password: "123"
}

loginForm.addEventListener("submit", (event) => {
  event.preventDefault()

  let userLogin = {
    username: inputUsername.value,
    password: inputPassword.value
  }

  console.log(userLogin);

  let login = userLogin.username == user.username && 
              userLogin.password == user.password;

  if (login) {
    console.log("selamat anda berhasil login")
  } else {
    console.log("username dan password anda salah");
  }
    
  // Membersihkan form
  // cara 1
  loginForm.reset()

  // cara 2
  // inputUsername.value = ""
  // inputPassword.value = ""

  // console.log("ini dari form yg di submit");
})
```


