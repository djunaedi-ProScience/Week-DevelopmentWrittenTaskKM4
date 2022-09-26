## Javascript Dasar
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




