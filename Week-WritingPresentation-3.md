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