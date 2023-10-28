# Tabel

Ada beberapa jenis informasi yang perlu ditampilkan dalam bentuk tabel, contohnya klasemen olahraga atau sebuah jadwal layaknya kalender. Ketika kita membuat sebuah tabel, pastinya kita akan banyak bermain dengan baris dan kolom. Pada materi ini, kita akan belajar cara membuat dan mengorganisasi sebuah tabel pada HTML.

Namun, sebelum itu, apa sih sebenarnya tabel dalam HTML itu? Elemen ```<table>``` pada HTML merepresentasikan data tabular, yaitu informasi yang disajikan dalam sebuah tabel. Tabel sendiri disajikan dalam dua dimensi terdiri dari baris dan kolom (cell) yang berisikan sebuah data. Berikut adalah contoh data sepak bola yang disajikan dalam bentuk tabel.

## Materi
### * Struktur Dasar Table
Tabel pada HTML disusun dari tiga buah elemen, yaitu ```<table>```, ```<tr>``` dan ```<td>``` atau ```<th>```. Elemen ```<table>``` digunakan untuk menandakan dimulainya dan diakhirinya sebuah konten tabel dan juga sebagai wadah untuk tabel itu sendiri. Kemudian elemen ```<tr>``` digunakan untuk membuat sebuah baris baru yang di dalamnya terdapat elemen ```<td>``` atau ```<th>``` sehingga menghasilkan sebuah sel. 

Elemen ```<td>```berarti “table data”. Selain membuat sel, elemen ini juga merupakan tempat menampung data pada tabel, dan elemen ```<th>``` atau “table header” digunakan untuk menentukan sebuah header pada kolom datanya. Untuk lebih jelasnya, perhatikan ilustrasi berikut.




### contoh code pembuatan struktur dasar tabel
```html 
<h1>Pemenang Piala Dunia Tiga Tahun Terakhir</h1>

<table>
  <tr>
    <th>Tahun</th>
    <th>Juara 1</th>
    <th>Juara 2</th>
    <th>Juara 3</th>
  </tr>
  <tr>
    <td>2018</td>
    <td>Prancis</td>
    <td>Kroasia</td>
    <td>Belgium</td>
  </tr>
  <tr>
    <td>2014</td>
    <td>Jerman</td>
    <td>Argentina</td>
    <td>Belanda</td>
  </tr>
  <tr>
    <td>2010</td>
    <td>Spanyol</td>
    <td>Belanda</td>
    <td>Jerman</td>
  </tr>
</table>
```
Hal yang perlu kita ingat lagi, seluruh konten atau data dituliskan pada elemen ```<td>``` ataupun ```<th>```. Kita bisa memberikan konten apa saja di dalamnya, seperti teks, gambar, atau bahkan sebuah tabel lainnya.

## Spanning Cell 
Terkadang kita membutuhkan sebuah sel untuk mencakup dua kolom ataupun dua baris sekaligus. Dalam aplikasi seperti Microsoft Word, hal ini biasa kita kenal sebagai merging cell atau menggabungkan sebuah sel. Ini memang menjadi sebuah fitur dasar dalam membuat sebuah tabel sehingga pada HTML pun kita dapat melakukan hal tersebut. 
1. __Column Spans__
Untuk merentangkan sebuah kolom (column spanning) kita bisa menggunakan atribut colspan pada elemen ```<td>```atau ```<th>```. Berikut adalah contoh untuk penggunaan colspan sehingga sebuah header mencakup dua kolom.
```html
<table>
  <tr>
    <th>18:00</th>
    <th>19:00</th>
    <th>20:00</th>
  </tr>
  <tr>
    <td colspan="2">Avenger Infinity Wars</td>
    <td>It Chapter 2</td>
  </tr>
  <tr>
    <td>One Piece: Stampede</td>
    <td>Weathering With You</td>
    <td>Gundala</td>
  </tr>
  <tr>
    <td>Gundala</td>
    <td colspan="2">Avenger Infinity Wars</td>
  </tr>
</table>

```

2. __Row Spans__ : Untuk merentangkan sebuah baris (row spanning) kita dapat menggunakan atribut rowspan. Mirip seperti column spanning, tetapi atribut ini akan merentangkan sebuah sel ke bawah. Berikut contohnya :
```html
<table border="1">
  <tr>
    <th rowspan="3">18:00</th>
    <td>Avenger Infinity Wars</td>
  </tr>
  <tr>
    <td>One Piece: Stampede</td>
  </tr>
  <tr>
    <td>Gundala</td>
  </tr>
</table>
```
Perhatikan elemen ```<th>``` yang memiliki atribut rowspan. Elemen tersebut berada pada baris pertama dan akan menempati sebanyak tiga baris tabel ke bawah. Jadi, pada baris tersebut membutuhkan dua buah elemen ```(<th> dan <td>)``` dan pada baris selanjutnya (baris dua dan tiga) memerlukan sebuah elemen ```<td>``` saja.

### Elemen dan Atribut pada Tabel
Sejauh ini, Anda sudah mengetahui penerapan dasar untuk sebuah tabel pada HTML. Sebenarnya masih terdapat beberapa anggota elemen dan atributnya yang dapat digunakan pada tabel. Karena elemen ini jarang digunakan sehingga kita akan mengenal secara ringkas dan merangkumnya dalam sebuah tabel berikut:
| Element dan Atribut | Deskripsi |
| ----------- | :---------: |
| table | Menetapkan elemen tabel |
| td | Menetapkan sebuah sel dalam baris tabel|
|  -colspan=”number” | Jumlah kolom yang dicakup oleh sel|
| -rowspan=”number”| Jumlah baris yang dicakup oleh sel |
| -headers=”nama header” | Mengasosiasikan data sel dengan header |
| th | Menetapkan header yang terkait dengan baris atau kolom |
| -colspan=”number” | Jumlah kolom dicakup oleh header |
| -rowspan=”number” | Jumlah row yang dicakup oleh header |
| -headers=”nama header” | Mengasosiasikan header dengan header lain |
| -scope=”row - col - rowgroup - colgroup” | Mengasosiasikan header dengan baris, kelompok baris, kolom, atau kelompok kolom |
| tr | Menetapkan sebuah baris pada tabel |
| caption | Memberikan judul pada sebuah tabel |
| col | Menetapkan sebuah kolom |
| colgroup | Menetapkan sebuah kelompok kolom |
| tbody | Mengidentifikasi sebuah body dalam tabel |
| tfoot | Mengidentifikasi sebuah footer dalam tabel |
| thead | Mengidentifikasi sebuah header dalam tabel |



untuk materi table udah selesai
### latihan
```
coba buat table sederhana tentang mahasiswa
```

