
# Asynchronous
Asynchronous sebuah teknik yang menyelesaikan fungsi secara paralel
Penggunaan asynchronous dapat dilakukan jika kita ingin mengambil data dari database

## Mengapa perlu
menggunakan asynchronous? Asynchronous dibutuhkan ketika ada proses yangg membutuhkan waktu lama. Jadi kita bisa mengerjakan proses yg lain secara paralel.
## Callbacks 
adalah suatu function namun cara pengeksekusiannya yang berbeda yaitu hanya mengeksekusi pada point tertentu.
Salah satu function yang digunakan untuk mengatur penjadwalan asynchronous adalah `setTimeout function`

## Asynchronous ada dua bisa pakai objeck promise bisa juga pakai async awai
- Contoh
buat dulu object promisesnya
```
// promise creation (membuat object promise)
let nonton = (kondisi) => {
  return new Promise((resolve, reject) => {
    if (kondisi == "jalan") {
      resolve("nonton terpenuhi")
    }
    reject("batal nonton")
  })
}
```
nah supaya kita tau bunyi janjinya kita bisa pakai cara kode promise di diatas ada 2 cara
- promise (then catch)
- async await
```
// ===================== Promise ===================
// promise
// namaPromis.then().catch()
nonton("jalan")
.then(result => {
  console.log(result);
}).catch(err => {
  console.log(err)
})
```
```
// ===================== async await ===============
// async await -> car utk nangkep obj promise
// buat async function
async function asyncNonton() {
  try {
    let result = await nonton("jalan")
    console.log(result);
  } catch (error) {
    console.log(error)
  }
}
asyncNonton()

// async arrow
// let asyncNonton = async () => { }

```

## Mengambil API dari WEB API
dengan menggunakan fetch kita bisa mengambil data API WEB diluar website kita
```
// ==================== FETCH ========================
// fetch -> obj promise
// di handle menggunakan promise atau async await
// API -> jembatan komunikasi ke server untuk mendapatkan data

// medapatkan data digimon
fetch("https://digimon-api.vercel.app/api/digimon")
.then(result => result.json())
.then(result => {
  console.log(result)
})

```

## Responsive Web Design
- Responsive Web Desin yaitu suatu tampilan website yang dapat menyesuikan dengan perangkat yang digunakan
- Untuk mengakses Chrome Dev Tools yaitu
                    ```ctrl + shift + j```
- Dalam menggunakan Responsive Web Design pada bagian HTML perlu ditambahkan viewport pada bagian head agar tampilan website dapat menyesuaikan dengan berbagai device
-        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
- **Media Query** salah satu cara untuk mengatur suatu website agar bisa terdiri dari beberapa jenis
Penggunaan media query yang umum digunakan adalah `min-width dan max-width`
Contoh penerapan media query 
- > @media screen and (max-width: 500px)
- Breakpoint yaitu istilah saat terjadi perubahan ukuran pada suatu website ketika berganti device
- Terdapat 3 jenis breakpoint yaitu desktop, tablet, dan mobile phone
Penggunaan breakpoint pada media query dapat dilakukan dengan membuat range ukuran sesuai dengan tampilan device yang ingin dibuat
- Contoh
```@media (max-width: 600px ) {
  .menu {
    display: none;
}
```

## CSS Units
### Relative Lengths
Satuan panjang relatif menentukan panjang relatif terhadap properti panjang lainnya
- em	Relatif terhadap ukuran font elemen (2em berarti 2 kali ukuran font saat ini)
- rem	Relatif terhadap ukuran font elemen root	
- vw	Relatif terhadap 1% dari lebar viewport*	
- vh	Relatif terhadap 1% dari ketinggian viewport*	
- vmin	Relatif terhadap 1% dari area pandang* dimensi yang lebih kecil
- vmax	Relatif terhadap 1% dari viewport* dimensi yang lebih besar	
- %	Relatif terhadap elemen induk

## Flexbox
Flexbox bertujuan untuk membuat website yang lebih efisien dalam mengatur, menata dan item pada dalam sebuah wadah bahkan ketika ukurannya tidak diketahui dan/atau dinamis (dengan menggunakan kata "flex").

## Flexbox properties :
- Flex direction : menetapkan sumbu utama item, sehingga menentukan arah item fleksibel ditempatkan di wadah fleksibel.
    - Row : Kiri ke kanan
    - Row-Reverse : Kanan ke kiri
    - Column : Atas ke bawah
    - Column-Reverse : Bawah ke atas
- Flex Wrap : Secara default, semua item pada flexbox akan mencoba berada dalam satu baris. Maka dengan flex wrap kita dapat mengubah hal tersebut.
    - nowrap : semua item flex akan berada dalam satu baris
    - wrap : item fkex akan membungkus ke beberapa baris, dari atas ke bawah.
    - wrap-reverse :item flex akan membungkus beberapa baris dari bawah ke atas.
    - Flex flow : cara singkat untuk properti flex-direction dan flex-wrap, yang bersama-sama menentukan sumbu utama dan sumbu silang container flex. Nilai default adalah baris nowrap.
    Align items
- justify-content : bisa berisi start,space-betweens,space-evenly
- flex -basis : berisi 1-100% ukuran columns item 
- flex shrink : mengambil ruang kosong didalam item lalu melebarkan tempatnya
- flex grow : membuat column menjadi rapat full width 

# Bootstrap
- Bootstrap adalah salah satu framework opensource yang berfungsi membuat suatu responsive website

- Komponen utama bootstrap :
    - bootstrap.css
    - bootstrap.js

- Cara konfigurasi bootstrap :
    - Membuat tag boostrap di head. Pakai CDN agar bisa mengakses Online
        - `<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.2/dist/css/bootstrap.min.css" rel="stylesheet"`
        
- Breakpoints merupakan suatu cara yang dilakukan untuk membuat desain responsif dengan mengontrol kapan tata letak yang disesuaikan dengan ukuran perangkat tertentu.
B-reakpoints pada bootstrap ada 
5 yaitu 
`sm, `
`md, `
`lg, `
`xl dan `
`xxl.`
Setiap breakpoint dipilih untuk menampung container yang lebarnya 12 dengan sehingga tersusun rapi. Breakpoint juga mewakili subset ukuran perangkat umum dan dimensi area pandang.

- __Container__ adalah blok dasar atau pembungkus boostrap yang terdiri dari contain, pad dan align yang menyelaraskan konten website dalam perangkat atau area
pandang tertentu.

  - Terdapat 3 container pada boostrap yaitu :
    - container, yang menerapkan lebar maksimum pada setiap breakpoint responsif
    - container-{breakpoint}, menerapkan lebar 100% sampai dengan breakpoint yang ditentukan.
    - container-fluid, menerapkan 100% ukurannya dari breakpoints
    
Grid System pada bootstrap yang terdiri dari 12 kolom default.

Grid system pada bootstrap menggunakan container,baris dan kolom untuk menata dan menyelaraskan konten,yang dibangun menggunakan flexbox dan itu sudah responsive.

contoh penggunaan grid system
```
  <div class="container text-center">
  <div class="row">
   <div class="col">
     Column
   </div>
   <div class="col">
     Column
   </div>
   <div class="col">
     Column
   </div>
  </div>
  </div>
```
### Grid system bootstrap :
.col-lg digunakan untuk mengatur grid pada ukuran monitor yang besar
.col-md digunakan pada monitor komputer berukuran sedang
.col-sm digunakan untuk mengatur monitor pada tablet
.col-xs digunakan untuk mengatur monitor pada handphone


# Git & Github Advanced
## Branch
Branch adalah sebuah cabang dari repository. Branch digunakan untuk mengembangkan fitur baru tanpa mengganggu branch utama. Branch juga digunakan untuk mengembangkan fitur baru secara bersamaan. Branch juga digunakan untuk mengembangkan fitur baru secara bersamaan.

## Merge
Merge adalah sebuah proses untuk menggabungkan branch yang berbeda. Merge hanya dapat dilakukan jika branch yang akan digabungkan memiliki parent. Merge hanya dapat dilakukan jika branch yang akan digabungkan memiliki parent.

## Merge Conflict
Merge conflict adalah sebuah kondisi dimana branch yang akan digabungkan memiliki parent yang berbeda

## Rebase
Rebase adalah sebuah proses untuk menggabungkan branch yang berbeda.

## Rebase Conflict
Rebase conflict adalah sebuah kondisi dimana branch yang akan digabungkan memiliki parent yang berbeda.

## Pull Request
Pull request adalah sebuah proses untuk menggabungkan branch yang berbeda. Pull request hanya dapat dilakukan jika branch yang akan digabungkan memiliki parent. 

## Pull Request Conflict
Pull request conflict adalah sebuah kondisi dimana branch yang akan digabungkan memiliki parent yang berbeda.

## Fork
Fork adalah sebuah proses untuk menggabungkan branch yang berbeda. 

## Fork Conflict
Fork conflict adalah sebuah kondisi dimana branch yang akan digabungkan memiliki parent yang berbeda.

## Clone
Clone adalah sebuah proses untuk menggabungkan branch yang berbeda.

## Clone Conflict
Clone conflict adalah sebuah kondisi dimana branch yang akan digabungkan memiliki parent yang berbeda. 

## Remote
Remote adalah sebuah proses untuk menggabungkan branch yang berbeda

## Remote Conflict
Remote conflict adalah sebuah kondisi dimana branch yang akan digabungkan memiliki parent yang berbeda. 

## Push
Push adalah sebuah proses untuk menggabungkan branch yang berbeda. 

## Push Conflict
Push conflict adalah sebuah kondisi dimana branch yang akan digabungkan memiliki parent yang berbeda.

## Pull
Pull adalah sebuah proses untuk menggabungkan branch yang berbeda.

## Pull Conflict
Pull conflict adalah sebuah kondisi dimana branch yang akan digabungkan memiliki parent yang berbeda..

## Fetch
Fetch adalah sebuah proses untuk menggabungkan branch yang berbeda. 

## Fetch Conflict
Fetch conflict adalah sebuah kondisi dimana branch yang akan digabungkan memiliki parent yang berbeda.

## Checkout
Checkout adalah sebuah proses untuk menggabungkan branch yang berbeda. Checkout tidak memiliki parent.

## Checkout Conflict
Checkout conflict adalah sebuah kondisi dimana branch yang akan digabungkan memiliki parent yang berbeda.

## Reset
Reset adalah sebuah proses untuk menggabungkan branch yang berbeda.

## Reset Conflict
Reset conflict adalah sebuah kondisi dimana branch yang akan digabungkan memiliki parent yang berbeda.

## Revert
Revert adalah sebuah proses untuk menggabungkan branch yang berbeda. 

## Revert Conflict
Revert conflict adalah sebuah kondisi dimana branch yang akan digabungkan memiliki parent yang berbeda. 

## Squash
Squash adalah sebuah proses untuk menggabungkan branch yang berbeda. 

## Squash Conflict
Squash conflict adalah sebuah kondisi dimana branch yang akan digabungkan memiliki parent yang berbeda


