# Modul HTML

Tujuan Modul ini saya buat dari materi yang saya dapat dari program biasiswa dari [IDCAMP](https://idcamp.ioh.co.id)
dan saya merasa harus merangkum materi tersebut agar orang lain bisa mempelajarinya juga

## Persiapan

- kita paham dulu dasar __HTML__ baru  kita jalankan di tools editor masing masing

## Materi

* kita akan mempelajari seperti _paragraf_ , _heading_ , _list_ dan lain²:

### contoh kodingan membuat biografi sebuah daerah
```html 
<!DOCTYPE html>
<html lang="in">
<head>
    <meta charset="UTF-8">
    <title>Judul halaman</title>
</head>
<body>
    <h1>MADURA</h1>
    <P>madura adalah pulai yang ada di jawa timur</P>
    <ul>
        <li>sejarah</li>
        <li>geografis</li>
        <li>wisata</li>
    </ul>
    <h2>sejarah</h2>
    <h2>geografis</h2>
    <h2>wisata</h2>
 </body>
</html>
```
diatas adalah contoh kode sederhana __html__ langsung aja kita memasuki pemahaman maksud kode di atas;

1. __Paragraf__  : Paragraf adalah elemen paling mendasar dari sebuah dokumen teks Pada HTML, kita bisa menunjukkan sebuah paragraf dengan menggunakan elemen ```html<p>``` browser akan menampilkannya dalam baris baru dan sedikit jarak (space) di bawah elemen dalam css juga bisa disebut margin. 
2. __Heading__ : Pada contoh sebelumnya, kita sudah melihat  penggunaan heading yang diterapkan pada konten yang kita siapkan. Kita menggunakan ```html <h1> dan <h2>``` dalam mengindikasi judul dan subjudul pada kontennya. Pada HTML, ada elemen dan ```html <h1> sampai <h6>``` elemen heading yang dapat kita gunakan.
3. __List__ : Sebagaimana yang sudah disebutkan pada pembahasan paragraf, tidak semua teks dibungkus oleh paragraf, salah satunya list. Kita pun terbiasa membuat list dalam kehidupan sehari-hari, baik membuat to-do list maupun daftar yang terstruktur sekalipun.
* pada HTML ada tiga tipe list:
1. Unordered lists: daftar yang ditampilkan tidak memiliki urutan. 
2. Ordered lists: daftar yang ditampilkan secara terurut.
3. Description lists: daftar yang terbuat dari beberapa istilah diikuti dengan deskripsi dari istilah tersebut.

* __Unordered List__ :
Seperti namanya, unordered list merupakan daftar yang tidak mementingkan urutan. Standarnya, unordered list menampilkan bullet pada tiap item list-nya (tetapi kita bisa mengubahnya dengan styling).
```html 
<ul>
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
  <li>Item 4</li>
</ul>
```
Di antara tag elemen ```html <li> ```, kita dapat mengisikan konten apa pun termasuk elemen HTML lain. Contohnya, kita dapat memasukkan sebuah heading atau paragraf pada item.
```html
<ul>
  <li><h1>Sebuah Heading sebagai item list</h1></li>
  <li><h2>Sebuah Heading level 2 sebagai item list</h2></li>
  <li><p>Sebuah paragraf sebagai item list</p></li>
</ul>
```
dan kita bisa juga menambahkan ```<ul>``` di dalam ```<ul``` contoh code berikut 
```html
<ul>
  <li>List item 1</li>
  <li>List item 2</li>
  <li>
    List item 3
    <ul>
      <li>List item 3.1</li>
      <li>List item 3.2</li>
      <li>List item 3.3</li>
    </ul>
  </li>
  <li>List item 4</li>
</ul>
```
* __Ordered List__ : Ordered list bekerja seperti unordered list, tetapi perbedaannya adalah pada tiap item menampilkan angka bukan sebuah bullet. Angka yang ditampilkan, otomatis berurut tiap item-nya sehingga kita tidak perlu menuliskan secara kasar urutan nomornya. Hal ini tentu mempermudah kita untuk mengorganisasi tiap itemnya.
```html
<ol>
  <li>Langkah pertama</li>
  <li>Langkah kedua</li>
  <li>Langkah ketiga</li>
  <li>Langkah selanjutnya</li>
</ol>
```
Pada ordered list, tipe urutan angkanya dapat kita atur melalui sebuah atribut type. Contohnya, selain nomor, urutan angka dapat diganti dengan alfabet ataupun angka romawi tinggal kita kasih attribut ```type```

```html
<!-- untuk angaka romawi-->
<ol type="I">
  <li>Langkah pertama</li>
  <li>Langkah kedua</li>
  <li>Langkah ketiga</li>
  <li>Langkah selanjutnya</li>
</ol>
<!-- untuk huruf alfabet-->
<ol type="A">
  <li>Langkah pertama</li>
  <li>Langkah kedua</li>
  <li>Langkah ketiga</li>
  <li>Langkah selanjutnya</li>
</ol>
```
berikut adalah nilai yang dapat kita gunakan di ```<ol>```
| Nilai | Deskripsi |
| ----------- | :---------: |
| 1 | menggunakan angaka dalam urutan item (default) |
| a | menggunakan huruf kecil dalam urutan item|
| A | menggunakan huruf besar dalam urutan item|
| i | menggunakan huruf romawi kecil dalam urutan item |
| I | menggunakan huruf romawi besar dalam urutan item |



nanti kita bahas lagi simatic __HTML__ di modul yang akan mendatang
### latihan
```
coba buat biografi daerah masing masing menggunak sematic di atas
```

