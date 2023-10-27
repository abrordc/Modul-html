# Gambar 
Tanpa gambar, sebuah website tentu tidak akan menarik bukan? Ada beberapa alasan mengapa website perlu gambar. Contohnya kita perlu menampilkan logo perusahaan, ilustrasi, diagram struktur atau data, dan sebagainya.

Pada HTML untuk menampilkan sebuah gambar kita bisa menggunakan tag ```<img>```. Berbeda dengan elemen lain, elemen ```<img>``` tidak menuliskan konten di antara tag pembuka dan tag penutup. Namun, untuk menetapkan gambar yang ditampilkan kita gunakan sebuah atribut.

contoh :
```html 
<img
  src=""
  alt="" 
>
```
Pada contoh kode di atas, perlu kita perhatikan bahwa elemen <img> merupakan sebuah elemen kosong (tidak memiliki konten sehingga tidak ada closing tag). 

Selain itu, hal yang perlu kita perhatikan adalah atribut pada elemen tersebut, terdapat dua elemen yang harus kita gunakan ketika menerapkan elemen <img>.

Pertama, atribut src. Atribut ini berfungsi sebagai sumber dari gambar yang ditampilkan. Atribut ini dapat bernilai url gambar atau path gambar local dari gambar yang digunakan.

Kedua adalah atribut alt. Atribut ini sebenarnya tidak wajib untuk diterapkan, hanya saja atribut ini akan sangat berguna ketika gambar tidak berhasil ditampilkan. Nilai atribut ini merupakan tampilan dari gambar yang ditampilkan dalam bentuk tulisan. Jadi, ketika gambar gagal ditampilkan akan memunculkan teks alternatif yang dapat mewakili arti dari gambar tersebut.

Selanjutnya terdapat atribut lain yang bisa Anda gunakan pada elemen ini, contohnya title. Ia berfungsi sebagai informasi tambahan untuk sebuah gambar. Informasi tersebut akan muncul ketika kita mengarahkan sebuah kursor pada gambar yang ditampilkan.

## Jenis Jenis format Gambar
Berikut adalah jenis format gambar yang umum digunakan pada pembuatan website.

| Nama | Ekatensi format file| Keterangan |
| ----------- | :---------: | ----------- |
| Graphics Interchange Format | .gif | Dapat digunakan untuk gambar animasi. Ukuran file biasanya kecil. Kualitas gambar terbatas. |
| Joint Photographic Expert Group image | .jpg, .jpeg, .jfif, .pjpeg, .pjp | Kualitas teks pada gambar dapat menjadi buruk. Ukuran file lumayan kecil. Pada website biasanya digunakan untuk gambar yang tidak banyak teks. |
| Portable Network Graphics | .png | Teks lebih bisa terbaca dibandingkan jenis jpeg. Ukuran file dapat menjadi besar sehingga mengurangi kecepatan memuat situs.
| WebP | .webp | Dibandingkan dengan gambar berkualitas sama pada jpeg atau png, ukuran file pada webp dapat menjadi lebih kecil. Namun, tidak semua web browser dapat membaca webp. |
| Scalable Vector Graphics | .svg | Kualitas gambar terjaga dan ukuran file kecil. Namun, tidak cocok untuk gambar yang terlalu kompleks, seperti foto. Pada website biasanya digunakan untuk logo atau ikon. |

## Mengatur Ukuran pada Gambar
Untuk mengatur ukuran gambar yang ditampilkan, kita juga tentunya menggunakan sebuah atribut. Untuk menentukan lebar gambar, kita gunakan atribut ```width```, dan untuk menentukan tinggi tentu gunakan atribut ```height```.

Ketika menggunakan atribut ini, disarankan hanya gunakan salah satunya. Terkecuali kita menentukan nilai lebar dan tingginya sesuai dengan rasio dari ukuran gambar aslinya. 

Contohnya, jika kita tetap memaksa untuk menentukan ukuran panjang dan lebar sebuah gambar tanpa menyesuaikan rasionya, gambar yang ditampilkan tidak akan proporsional.
```html 
<!-- Jangan lakukan hal ini! -->
<img src="" alt="" height="" width=""/>
```

