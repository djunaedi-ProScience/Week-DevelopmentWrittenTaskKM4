# Javascript Intermediate

## Array
Array merupakan pengorganisasian data dan tempat penyimpanan data
Array adalah tipe data list order yang dapat menyimpan tipe data apapun dialamnya seperti string, number, boolean dan lainnya
### contoh Array
    Let randomData = ['ini string', 20, true];
    console.log(randomData);
    Membuat Array : Array didefinisikan dengan square brackets []
    Mengakses Array : Array pada javascript dihitung mulai dari index ke- 0
    Let randomData = ['ini string', 20, true];
    console.log(randomDaData[1]); //Output : 20
### Update Array
    let arrayData =[1,2,3,4,5]

    console.log("sebelum diupdate:" arrayData[0]]);

    arrayData[0] = 15
    console.log("sesudah diupdate:" arrayData[0]]); 
### Const in Array
Apabila menggunakan let, array dapat diubah dengan nilai yang baru
Const tidak dapat melakukan update data. Namun dapat melakukan update konten nilai di dalam array
Tidak dapat mengubah array dengan array baru jika menggunakan const
contoh penggunaan const

    const cars = ['tesla', 'honda', 'toyota'];
    cars[2] = ['nissan'];

    console.log(cars)// output : ['tesla','honda','nissan']
   
### Array Properti. Array memiliki 5 properti yang sering digunakan yaitu :
- constructor
- length
- index
- input
- prototype

### length yaitu mengembalikan nilai dari jumlah panjang data suatu array
```
let cars = ['tesla', 'honda', 'toyota'];
console.log(cars.length) // output 3
```
**Array Method atau biasa disebut dengan built in methods**

### Contoh array built in method :
.push adalah method untuk menambahkan item array pada urutan yang paling akhir
```
 let cars = ['tesla', 'honda', 'toyota'];
 cars.push('hyundai')
 console.log(cars) // output:['tesla','honda','toyota','hyundai']
 ```
### pop adalah method yang menghapus item array index terakhir
```
 let cars = ['tesla', 'honda', 'toyota'];
 cars.pop()
 console.log(cars) // output: ['tesla','honda']
 ```
### .shift adalah method untuk menghapus item array pada index pertama
```
 let cars = ['tesla', 'honda', 'toyota'];
 cars.shift()
 console.log(cars) // output: ['honda','toyota']
 ```
### .unshift adalah method untuk menambahkan array pada index pertama
```
 let cars = ['tesla', 'honda', 'toyota'];
 cars.unshift('hyundai')
 console.log(cars) // output:['hyundai','tesla','honda','toyota',]
 ```
### sort adalah method untuk mengurutkan array secara ascending atau descending
```
const numbers = [1,3,5,2,4];
numbers.sort();
console.log(numbers) // output : [1,2,3,4,5]
```
### Looping pada Array.
Built in methods untuk melakukan looping pada array ada .map dan .forEach
```
.forEach adalah method untuk melakukan looping pada setiap elemen array
const cars = ['tesla', 'honda', 'toyota'];
cars.forEach(element => {
console.log(element);
});

```
### .map adalah method untuk melakukan perulangan dengan membuat array baru
```
let arr = [1,2,3,4,5];

let doubled = arr.map(num => {
    return num * 2;
});
console.log(doubled);
```
### Multidimensional Array
Multidimensional array bisa dianalogikan sebagai array of array

Multidimensional array sama seperti matriks yaitu memiliki 2 dimensi (x,y)
```
let inventory = [
    ['Kaos Polos' , 10],
    ['Jaket' , 5],
    ['Topi' , 12],
    ['Celana' , 4],
];
console.log(inventory);
```
### Mengakses multidimensional array
```
let inventory = [
   ['Kaos Polos' , 10],
   ['Jaket' , 5],
   ['Topi' , 12],
   ['Celana' , 4],
];
console.log(inventory[1][0]);
```
### Penggunaan built in method pada multidimensional array
```
let inventory = [
    ['Kaos Polos' , 10],
    ['Jaket' , 5],
    ['Topi' , 12],
    ['Celana' , 4],
];
inventory.push(['Hoodie', 2]);
console.log(inventory);
```
### Operation using map in multidimensional array
```
let inventory = [
    ['Kaos Polos' , 10],
    ['Jaket' , 5],
    ['Topi' , 12],
    ['Celana' , 4],
];
inventory.map(dataInventory => {
    let terjual = 100 - dataInventory[1];
    dataInventory[2] = terjual;
});
console.table(inventory);
```
### map array
Looping pada Multidimensional array
```
let inventory = [
    ['Kaos Polos' , 10],
    ['Jaket' , 5],
    ['Topi' , 12],
    ['Celana' , 4],
];
inventory.forEach((baris) => {
    baris.forEach((column) => {
        console.table(column);
    });
});

```

# Object
object adalah sebuah tipe data pada variabel yang menyimpan properti dan fungsi (method)

- Properti adalah data lengkap dari sebuah object.
- Method adalah action dari sebuah object. Apa saja yang dapat dilakukan dari suatu object.


## Assign Object
```
let hewan = {
  nama: "kucing",
  kaki: 4,
  warna: "putih",
};
```

**Memanggil Object**
ada dua cara bisa menggunakan [] atau mengunakan titik (.)
```
hewan.nama = "kelinci";
hewan["kaki"] = 2;
// memanggil nama objek dengan variable
let properti = "umur";
console.log(siswa[properti]);

// Mengakses Object key atau value
console.log(Object.keys(siswa));
console.log(Object.values(siswa));
```

**Menghapus Object**
```
delete hewan.warna;
```

**Memanggil Method**
```
const greeting = {
  welcome: function () {
    return "halo selamat datang";
  },
  afterPay: function () {
    return "Terimakasih sudah membeli produk kami";
  },
};

// Panggil method dalam object
console.log(greeting.welcome());
console.log(greeting.afterPay());

```

**Nested Object**
```
let buku = {
  judul: "tips jago javascript",
  tahun: 2022,
  penulis: {
    penulis1: {
      nama: "Reyhan",
      umur: 28,
      kota: "jakarta",
    },
    penulis2: {
      nama: "aby",
      umur: 25,
      kota: "bandung",
    },
  },
};

// cara mengakses nested object

console.log(buku);
console.log(buku.penulis.penulis1.nama);
console.log(buku.penulis.penulis2.umur);
```

**Iteration Object dan nested object**
```
// for in
let siswa = {
  nama: "Reyhan",
  umur: 22,
  asal: "jakarta",
  hobi: "membaca",
};

console.log(siswa);

//iteration menggunakan for in
for (let key in siswa) {
  console.log(siswa[key]);
  //   console.log(key);
  //siswa[key] -> siswa['nama'] -> siswa['umur'] -> siswa['asal']
}

let buku = {
  judul: "tips jago javascript",
  tahun: 2022,
  penulis: {
    penulis1: {
      nama: "Reyhan",
      umur: 28,
      kota: "jakarta",
    },
    penulis2: {
      nama: "aby",
      umur: 25,
      kota: "bandung",
    },
  },
};

// iteration nested
console.log(buku);
for (let key in buku.penulis.penulis1) {
  console.log(buku.penulis.penulis1[key], "----ini dari nested");
}
```

** Array Object**
```
let users = [
  {
    nama: "dila",
    umur: 17,
    alamat: "bandung",
  },

  {
    nama: "audzan",
    umur: 18,
    alamat: "jakarta",
  },
  {
    nama: "dolton",
    umur: 16,
    alamat: "sulawesi",
  },
];

console.log(users);

// perulangan / iteration. menambahkan properties status dengan value aktif
let data = users.map((el) => {
  // console.log(el.nama);
  el.status = "aktif";
  return el;
});

```

# Rekursive
Recursive adalah function yang memanggil dirinya sendiri sampai kondisi tertentu
**Penggunaan**
Recursive kebanyakan digunakan untuk case matematika, fisika, kimia, dan yang berhubungan dengan calculation

## Contoh Rekursive menghitung pangkat
```
function pow(x,n){
    if (n == 1) {
        return x
    } else {return x * pow(x,n - 1)
 }
}
console.log(pow(2,3));
```

## Asynchronous & Promises
**Asynchronous**
Asynchronous sebuah teknik yang menyelesaikan fungsi secara paralel
Penggunaan asynchronous dapat dilakukan jika kita ingin mengambil data dari database
Mengapa perlu menggunakan asynchronous? Asynchronous dibutuhkan ketika ada proses yangg membutuhkan waktu lama. Jadi kita bisa mengerjakan proses yg lain secara paralel.

**Callbacks** adalah suatu function namun cara pengeksekusiannya yang berbeda yaitu hanya mengeksekusi pada point tertentu.

Salah satu function yang digunakan untuk mengatur penjadwalan asynchronous adalah setTimeout function
contoh penggunaan asynchronous

**Contoh Calback**
```
// ========================= CALLBACK =====================
console.log("CALLBACK")
console.log("A")

// butuh proses yg memakan waktu
// callback -> function yg dijadikan sbg argumen
setTimeout(() => {
  console.log("B")
}, 1000)

console.log("C")
```

## Membuat Promises
Mendefiniskan Promises
```
// ======================== PROMISES =====================
console.log("PROMISES")
// pembuatan promise.............
let nontonPromise = new Promise((resolve, reject) => {
  if (true) {
    resolve("nonton terpenuhi") // berhasil
  } 

  reject("gagal"); // gagal
});

// eksekusi proses..............
console.log("A");

```

## Memanggil promises
```
nontonPromise
  .then((result) => {
    console.log(result);
    return `${result} bareng doi`
  })
  .then((result) => {
    console.log(result)
  })
  .catch((err) => {
    console.log(err);
  });

console.log("C");
```

## Promises tapi dalam function
```
// ================== promise dari function =============
console.log("PROMISES dari function")
let nonton = (kondisi) => {
  return new Promise((resolve, reject) => {
    if (kondisi == "jalan") {
      resolve("nonton terpenuhi")
    }
    reject("batal nonton")
  })
}

nonton("jalan")
.then(result => {
  console.log(result)
})
.catch(err => {
  console.log(err);
})
```



## Web Storage
Web Storage adalah wadah untuk sebuah data yang digunakan untuk penyimpanan data yang terikat di browsernya
Jenis Web Storage yang umum digunakan yaitu :
- Local Storage
- Session storage
- IndexDB
- Cookies
```
Cara menyimpan data pada local storage
    let token = "asdfghjkl" //key
    localStorage.setItem("token", token);
Cara mengambil token
    localstorage.getItem("token", token);
    console.log(localStorage.getItem('token");
Cara menghapus data
    localStorage.removeItem("token");
 ```



