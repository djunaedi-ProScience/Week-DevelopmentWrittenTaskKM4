# React JavaScript
> React adalah library atau framework yang dikhususkan bagi client/user untuk membuat tampilan website

- React membuat aplikasi menjadi lebih cepat
- React dapat digunakan pada skala yang kecil maupun besar
- React sangat populer dan memiliki komunitas yang besar
- Untuk menjalankan react dapat menggunakan node.js
## Step menggunakan React JS :
- Menginstall node js
- Menginstall npm install -g create-react-app
- Membuat project dengan npx create-react-app [name-project]
- File extension dari javascript pada react adalah JSX
- Rules JSX
- Hanya boleh memiliki 1 parent
- Memiliki DOM manipulation
- Atribut class di tag HTML harus menggunakan className
- Menggunakan curly braces untuk mengakses variabel JSX

Virtual DOM : sebuah javascript object (virtual) yang merepresentasikan DOM yang sebenarnya (real DOM)
Component pada React JS merupakan core pada React JS yang bersifat enkapsulasi atau pembungkus pada react dimana dalam 1 page dapat terdiri dari beberapa component

## Cara membuat component :
- Menggunakan function
- Menggunakan class

Functional Component hanya bisa menggunakan props itu sebabnya function component disebut stateless component

Clasas Component dapat menggunakan props dan state

props & state digunakan untuk menghandle data di dalam component.

Props merupakan data yang dapat kita kirimkan dari suatu component ke component lain

State digunakan untuk menghandle data yang sifatnya berubah-ubah dan data yang bersifat private yang hanya dapat diakses oleh component tersebut saja

Stateless dan Statefull Component

Stateless Component adalah component yang tidak memiliki state internal sendiri, melainkan data yang didapatkan oleh komponen tersebut berasal dari luar

Statefull Component adalah component yang memiliki state sendiri sehingga stateful component harus menggunakan fungsi setState/useState di dalam tubuh fungsi

Lifecycle adalah siklus hidup pada React js

## Struktur Lifecycle :
- Constructor: inisialisasi struktur data pada suatu component
- function : fungsi yg dibutuhkan pada komponen
- Render: proses return atau mengembalikan component asli

## Jenis - jenis Lifecycle Component Class:
- Mounting : Siklus ketika aplikasi sesaat sebelum component dibuka.
  - componentDidMount adalah ketika memuat aplikasi sebelum di render
  - componentWillMount adalah ketika aplikasi dimuat setelah proses render dilakukan.
- Updating : Ketika component di update atau diubah
- Unmount : Proses menghancurkan component yang sebelumnya di definisikan
## Styling pada React JS

- Styling Inline : menggunakan style ini, nilainya harus berupa object JavaScript
```
  class MyHeader extends React.Component {
  render() {
  return (
  <div>
  <h1 style={{color: "red"}}>Hello Style!</h1>
  <p>Add a little style!</p>
  </div>
  );
 }
}
```
```
Penulisan Nama properti menggunakan camelCased
    class MyHeader extends React.Component {
    render() {
    return (
    <div>
    <h1 style={{backgroundColor: "lightblue"}}>Hello Style!</h1>
    <p>Add a little style!</p>
    </div>
    );
   }
  }
Stylesheet CSS
   background-color: #282c34;
   color: white;
   padding: 40px;
   font-family: Arial;
   text-align: center;
```