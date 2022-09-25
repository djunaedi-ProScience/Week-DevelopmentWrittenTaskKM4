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




 

