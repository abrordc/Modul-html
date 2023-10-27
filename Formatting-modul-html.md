# inline formatting text 
Sejauh ini, kita sudah mengenal paragraf, heading, dan juga list pada HTML. Tapi masih ada beberapa lagi yang merupakan spesial teks format yang dapat kita gunakan yaitu ```<blockquote>, <pre> dan <figure>.```

## Long Quotations
Jika pada konten kita memiliki sebuah kutipan ataupun sebuah testimonial, kita dapat gunakan format long quotations dengan menggunakan tags ```<blockquote>```. Konten di dalam elemen ``` <blockquote> ``` ini dapat berupa sebuah paragraf, heading, ataupun list.

contoh code :
```html
<blockquote>
  <p>
    Situs web (bahasa Inggris: website) adalah sekumpulan halaman web yang saling berhubungan yang
    umumnya berada pada peladen yang sama berisikan kumpulan informasi yang disediakan secara
    perorangan, kelompok, atau organisasi.
  </p>
</blockquote>
```

Pada elemen ini, kita dapat menggunakan atribut cite untuk menentukan sumber URL dari sebuah kutipan (jika kutipan tersebut bersumber dari sebuah situs website). Namun, tidak ada tampilan yang berbeda pada browser secara kasat mata.
```html
<blockquote cite="https://id.wikipedia.org/wiki/Situs_web">
  <p>
    Situs web (bahasa Inggris: website) adalah sekumpulan halaman web yang saling berhubungan yang
    umumnya berada pada peladen yang sama berisikan kumpulan informasi yang disediakan secara
    perorangan, kelompok, atau organisasi.
  </p>
</blockquote>
```

## Preformatted Text
Pada modul sebelumnya, kita sudah mengetahui bahwa HTML akan mengabaikan spasi yang dituliskan secara berulang dan juga line breaks (garis baru). Namun, pada beberapa tipe konten, seperti contoh kode atau puisi hal tersebut sangat berarti.

Dengan begitu, terdapat sebuah elemen yang dapat kita gunakan untuk menampilkan konten sesuai yang kita tulis pada text editor. Untuk menggunakannya, kita gunakan elemen ``` <pre> ```sebagai pembungkus kontennya. Perhatikan contoh berikut.
```html
<pre>
  SAJAK PUTIH
Bersandar pada tari warna pelangi
Kau depanku bertudung sutra senja
Di hitam matamu kembang mawar dan melati
Harum rambutmu mengalun bergelut senda
Sepi menyanyi, malam dalam mendoa tiba
Meriak muka air kolam jiwa
Dan dalam dadaku memerdu lagu
Menarik menari seluruh aku
Hidup dari hidupku, pintu terbuka
Selama matamu bagiku menengadah
Selama kau darah mengalir dari luka
Antara kita Mati datang tidak membelah...
                  Karya: Chairil Anwar
</pre>
```

## Figure
Elemen ``` <figure> ``` digunakan untuk mempresentasikan konten tersendiri (self-contained content), seperti ilustrasi, diagram, foto, atau bisa juga sebuah baris kode. Banyak hal yang dapat digunakan dalam elemen ini. 

Elemen ini digunakan untuk mengelompokkan blok konten yang dapat dipindahkan posisinya dari blok utama sebuah dokumen tanpa mempengaruhi arti dari induk dokumen.

Dalam elemen figure, kita dapat menuliskan elemen ```<figcaption>```sebagai sebuah caption (judul) untuk konten tersebut. Berikut adalah contoh penggunaan figure pada sebuah konten gambar.
```html
<p>universitas madura</p>

<figure>
  <img
    src="unira.png"
    alt="unira logo"
    width="200px"
  />
  <figcaption>logo unira</figcaption>
</figure>

```

> Kita sudah belajar mengidentifikasi penggunaan elemen pada konten yang mayor (besar) dengan menerapkan semantic HTML untuk mengorganisasi kontennya. Sekarang, kita akan mengenal beberapa formatting text yang digunakan dalam sebuah baris teks (inline teks). 

> Sebelum menjelaskan elemen inline untuk formatting text yang dapat digunakan, sepertinya kita perlu membahas sekilas mengenai block dan inline.

Pada standarnya, elemen HTML memiliki dua sifat, yaitu block dan inline. Elemen yang bersifat block selalu membuat baris baru ketika di-render. Contohnya seperti elemen paragraf, list, heading, dan lainnya. Lawan dari elemen tersebut, yaitu elemen inline. Elemen ini tidak menambahkan baris baru ketika di-render. Apa saja elemen tersebut? Mari kita bahas satu persatu.

## Anchor
Anchor (jangkar) merupakan elemen yang digunakan untuk membuat sebuah hyperlink ke halaman atau website lain, file, alamat email, atau URL lainnya. Untuk menggunakan elemen ini kita gunakan ```<a>``` sebagai tag pembuka dan ```</a>``` sebagai tag penutup. Selain itu, ada atribut wajib agar elemen ini berfungsi dengan baik, yaitu href untuk menetapkan sebuah target yang dituju. 
```html
<p>Hubungi kami di</p>
<ul>
  <li><a href="https://example.com">Website</a></li>
  <li><a href="mailto:info@example.com">Email</a></li>
  <li><a href="tel:+62123456">Telepon</a></li>
  <li><a href="#address">Alamat</a></li>
</ul>
```

### Atribut khusus untuk elemend di atas
| Nama | Nilai | Deskripsi |
| ----------- | :---------: | ----------- |
| download | filename | Menginstruksikan browser untuk mengunduh pada URL yang ditetapkan dari pada mengarahkannya |
| href | URL | Menetapkan target yang akan diarahkan/unduh ketika pengguna menekan hyperlink |
| hreflang | language_code | Menetapkan bahasa dari dokumen target |
| ping | list_of_URLs | Menetapkan URL yang akan diberitahu dengan mengirimkan post request ping pada body oleh browser (berjalan di belakang layar) ketika target URL pada hyperlink ditekan. Biasanya atribut ini digunakan untuk pelacakan |
| referrerpolicy | no-referrer, no-referrer-when-downgrade, origin, origin-when-cross-origin, unsafe-url | Menetapkan referensi untuk dikirim pada target |
| rel | alternate,author,bookmark,external,help,license,next,nofollow,noreferrer,noopener,prev,search,tag | Menetapkan hubungan antara halaman yang ditampilkan dengan target |
| target | _blank,_parent,_self,_top | Menetapkan lokasi ketika membuka target contohnya pada sebuah tab, window, atau tab itu sendiri |
| media | media_type | Menetapkan tipe media yang digunakan pada target |

## Emphasized text
Gunakan elemen ```<em>``` untuk menunjukkan bagian kata yang perlu kita tekankan. Elemen ini menunjukkan stress emphasis atau konten/kata yang perlu mendapatkan penekanan atau perhatian khusus. Berikut contoh penggunaannya.
```html
<p><em>Oding</em> adalah seorang pelajar</p>
<p>Dia adalah seorang <em>pelajar</em></p>
```

## Important text
Gunakan elemen ```<strong>``` untuk menunjukkan sebuah teks yang begitu penting (strong importance), serius ataupun mendesak. Artinya, teks tersebut harus dapat perhatian lebih dari teks biasa lainnya.
```html
<p>Kesehatan merupakan hal yang penting, jaga pola makan yang teratur dan <strong>jangan sampai makan tengah malam!</strong></p>
```

## Short quotations
Gunakan elemen ```<q>``` untuk menandai sebuah kutipan dalam sebuah teks. Elemen ini berbeda dengan ```<blockquote>```. Elemen ini digunakan untuk kutipan pendek yang terletak di dalam baris (inline).
```html
<p>Sebelum pulang kerja, ia berkata kepadaku: <q>Maaf saya tidak bisa hadir dalam pertemuan nanti</q></p>
```

> Kita sudah belajar banyak formatting text. Namun, ada beberapa sisanya yang belum kita bahas. Tentunya, mereka tidak kalah penting dalam membangun konten halaman web yang lebih baik. Mari kita lengkapi pembahasan ini. Jom!

## Citation
Selain sebuah atribut, ```<cite>``` juga merupakan sebuah elemen yang digunakan untuk sebuah rujukan pada sebuah dokumen, contohnya sebuah buku, majalah, artikel, dan lainnya.
```html
p>Informasi selengkapnya bisa Anda dapatkan di <cite><a href="https://unira.ac.id">unira.ac.id</a></cite>.</p>
```

## Defining Terms
Elemen ```<dfn>``` digunakan ketika mendefinisikan sebuah istilah (term). Elemen ini harus terletak pada elemen lain yang menaunginya. Contohnya pada sebuah elemen ```<p>``` atau elemen ```<section>```. Berikut contoh penggunaannya. 
```html
<p><dfn>Website</dfn> merupakan halaman yang menampilkan informasi melalui teks atau gambar. Website dapat diakses melalui internet dengan menggunakan browser.</p>

```

## Subscript dan Superscript
Subscript ```<sub>``` dan superscript ```<sup>``` adalah elemen yang dapat membuat teks yang ditampilkan tampak kecil, dengan posisi di bawah (sub) atau di atas (sup) dari teks biasanya. Elemen ini digunakan untuk menunjukkan sebuah rumus kimia ataupun matematika.
```html
<p>
  Sukrosa merupakan suatu disakarida yang dibentuk dari monomer-monomernya yang berupa unit glukosa dan fruktosa, dengan rumus molekul C<sub>12</sub>H<sub>22</sub>O<sub>11</sub>.
</p>

<p>Salah satu persamaan paling umum dalam semua fisika adalah E=MC<sup>2</sup></p>
```

## Highlighted text
Untuk menandai atau menyorot sebuah teks kita bisa menggunakan elemen ```<mark>```. Elemen ini digunakan ketika terdapat sebuah teks yang memiliki peran penting, biasanya teks tersebut merupakan bagian yang paling relevan atau penting dalam sebuah konteks kalimat.
```html
<p>
  Ini adalah periode perang saudara. Pesawat ruang angkasa pemberontak, menyerang dari pangkalan
  tersembunyi, telah memenangkan kemenangan pertama mereka melawan Kekaisaran Galactic yang jahat.
  Selama pertempuran,
  <mark>mata-mata Pemberontak berhasil mencuri rencana rahasia </mark>
  ke senjata pamungkas Kekaisaran, STAR DEATH, stasiun ruang angkasa berlapis baja dengan kekuatan
  yang cukup untuk menghancurkan seluruh planet.
</p>
```

> tetap semangat belajarnya dan konsisten

#### latihan
``` 
cobak buatkan artikel sederhana menggunakan formatting di atas 
```
