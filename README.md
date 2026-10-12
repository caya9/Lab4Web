# 🌐 LAPORAN PRAKTIKUM 4
## CSS Layout — Pemrograman Web

<p align="center">
  <img src="https://img.shields.io/badge/Praktikum-04-blue?style=for-the-badge" alt="Praktikum 04">
  <img src="https://img.shields.io/badge/HTML-5-orange?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5">
  <img src="https://img.shields.io/badge/CSS-3-blue?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3">
</p>

---

## 👩‍💻 Identitas Mahasiswa

| Keterangan | Informasi |
|---|---|
| Nama | Chaya Aulia |
| NIM | 312510197 |
| Universitas | Universitas Pelita Bangsa |
| Program Studi | Teknik Informatika |
| Mata Kuliah | Pemrograman Web |
| Praktikum | Praktikum 4 — CSS Layout |

---

## 📌 1. Pendahuluan

### 1.1 Latar Belakang

Dalam pengembangan website, tata letak atau *layout* merupakan bagian penting untuk menyusun elemen agar halaman web terlihat rapi, terstruktur, dan mudah dipahami oleh pengguna.

HTML digunakan untuk membentuk struktur halaman web, sedangkan CSS digunakan untuk mengatur tampilan dan posisi elemen. Salah satu teknik yang dipelajari dalam praktikum ini adalah penggunaan properti `float` dan `clear` untuk mengatur posisi elemen.

Selain itu, HTML menyediakan elemen semantik seperti `header`, `nav`, `section`, `article`, `aside`, dan `footer` yang membantu membagi halaman berdasarkan fungsinya.

### 1.2 Tujuan Praktikum

Tujuan pelaksanaan praktikum ini adalah:

1. Memahami struktur dokumen HTML.
2. Memahami penggunaan elemen `div` untuk membentuk kotak.
3. Mempelajari penggunaan CSS `float` dan `clear`.
4. Memahami penggunaan elemen semantik HTML5.
5. Membuat layout website sederhana menggunakan HTML dan CSS.
6. Menambahkan konten, sidebar, widget, dan footer.
7. Membuat halaman About dan Contact.
8. Melakukan validasi HTML serta mendokumentasikan hasil praktikum menggunakan GitHub.

### 1.3 Dasar Teori

**HTML (HyperText Markup Language)** merupakan bahasa markup yang digunakan untuk membangun struktur halaman web.

**CSS (Cascading Style Sheets)** digunakan untuk mengatur tampilan halaman web, seperti warna, ukuran, jarak, posisi, dan tata letak elemen.

Beberapa properti dan elemen yang digunakan dalam praktikum ini adalah:

| Elemen/Properti | Fungsi |
|---|---|
| `div` | Mengelompokkan elemen ke dalam sebuah blok. |
| `float` | Mengatur elemen agar mengapung ke kiri atau kanan. |
| `clear` | Mengatur posisi elemen terhadap elemen yang menggunakan `float`. |
| `header` | Menandai bagian kepala halaman. |
| `nav` | Menandai bagian navigasi. |
| `section` | Mengelompokkan bagian konten yang berkaitan. |
| `article` | Menandai konten artikel yang berdiri sendiri. |
| `aside` | Menandai konten tambahan, misalnya sidebar. |
| `footer` | Menandai bagian kaki halaman. |

---

## 🛠️ 2. Alat dan Bahan

Perangkat dan aplikasi yang digunakan dalam praktikum ini meliputi:

- 💻 **Visual Studio Code** — untuk menulis dan mengedit kode HTML dan CSS.
- 🌐 **Web Browser** — untuk melihat dan menguji hasil halaman web.
- ✅ **W3C Markup Validation Service** — untuk memeriksa validitas HTML.
- 🐙 **Git dan GitHub** — untuk menyimpan, mengelola, dan mengumpulkan hasil praktikum.

---

## 🚀 3. Langkah-Langkah Praktikum

### 3.1 Persiapan Dokumen HTML

Langkah pertama adalah membuat folder `Lab4Web` sebagai tempat penyimpanan seluruh file praktikum. Selanjutnya, dibuat file `lab4_box.html` sebagai dokumen awal untuk mempelajari elemen kotak.

Dokumen HTML terdiri dari deklarasi `DOCTYPE`, elemen `html`, bagian `head`, dan bagian `body`. Elemen `header` digunakan untuk menampilkan judul Box Element.

**Hasil:** Dokumen HTML awal berhasil dibuat sebagai dasar latihan.

📸 **Dokumentasi:**

![Membuat dokumen Box Element](screenshot/01-membuat-dokumen-box-element.png)

### 3.2 Membuat Box Element

Pada tahap ini, ditambahkan tiga elemen `div` dengan kelas `div1`, `div2`, dan `div3`. Setiap elemen berisi teks yang menunjukkan identitas kotaknya.

Kelas tersebut digunakan sebagai penanda agar masing-masing kotak dapat diberikan aturan CSS yang berbeda.

**Hasil:** Tiga elemen kotak berhasil ditambahkan ke dalam dokumen HTML.

📸 **Dokumentasi:**

![Membuat Box Element](screenshot/02-membuat-box-element.png)

### 3.3 Menerapkan CSS Float

Properti `float` diterapkan pada elemen `div` agar kotak dapat tersusun berdampingan. Properti `padding` digunakan untuk memberikan jarak antara isi kotak dan batas elemen.

Setiap kelas diberikan warna latar yang berbeda, yaitu merah, kuning, dan hijau.

**Contoh kode CSS:**

```css
div {
    float: left;
    padding: 10px;
}

.div1 {
    background: red;
}

.div2 {
    background: yellow;
}

.div3 {
    background: green;
}
```

**Hasil:** Ketiga kotak ditampilkan berdampingan dengan warna yang berbeda.

📸 **Dokumentasi:**

![Penerapan CSS Float](screenshot/03-menerapkan-css-float.png)

### 3.4 Mengatur Clearfix Element

Pada tahap ini, ditambahkan elemen `div4` dengan warna latar biru. Properti `clear` digunakan untuk mengatur posisi elemen tersebut terhadap elemen sebelumnya yang menggunakan `float`.

```css
.div4 {
    background-color: blue;
    clear: left;
    float: none;
}
```

Nilai `left`, `right`, dan `both` dapat dicoba untuk mengamati perbedaan posisi elemen. `clear: left` menghindari elemen mengalir di samping elemen yang mengapung ke kiri, sedangkan `clear: both` berlaku untuk elemen yang mengapung ke kiri maupun kanan.

**Hasil:** Posisi kotak keempat dapat diatur berdasarkan nilai properti `clear`.

📸 **Dokumentasi:**

![Mengatur Clearfix](screenshot/04-mengatur-clearfix.png)

### 3.5 Membuat Kerangka Layout Sederhana

Selanjutnya dibuat folder `lab4_layout` yang berisi file `home.html` dan `style.css`.

Struktur halaman dibangun menggunakan elemen semantik HTML5. Kerangka layout terdiri dari header, navigasi, hero, wrapper, main content, sidebar, dan footer.

**Hasil:** Struktur dasar halaman website berhasil dibuat sebelum diberikan pengaturan CSS lebih lanjut.

📸 **Dokumentasi:**

![Kerangka Layout](screenshot/05-membuat-kerangka-layout.png)

### 3.6 Mengatur Header Layout

Bagian header berisi judul `Layout Sederhana`. CSS digunakan untuk mengatur jarak bagian header dan tampilan teks judul.

Container juga diatur agar memiliki lebar tertentu dan berada di tengah halaman. Properti `box-shadow` digunakan untuk memberikan efek bayangan pada container.

**Hasil:** Bagian header dan container memiliki susunan yang lebih teratur.

📸 **Dokumentasi:**

![Header Layout](screenshot/06-mengatur-header-layout.png)

### 3.7 Membuat Navigasi

Elemen `nav` digunakan untuk menampilkan menu navigasi yang terdiri dari Home, Artikel, About, dan Kontak.

CSS digunakan untuk memberikan warna latar, jarak antarelemen, warna teks, dan menghilangkan garis bawah tautan. Efek hover digunakan untuk mengubah tampilan menu saat penunjuk diarahkan ke atasnya.

**Hasil:** Menu navigasi tampil dengan lebih rapi dan mudah dikenali.

📸 **Dokumentasi:**

![Navigasi Website](screenshot/07-membuat-navigasi.png)

### 3.8 Membuat Hero Panel

Hero panel merupakan bagian yang ditampilkan setelah navigasi. Bagian ini berisi judul `Hello World!`, paragraf deskripsi, dan tombol `Learn More`.

CSS digunakan untuk mengatur warna latar, jarak dalam elemen, ukuran judul, dan ukuran teks paragraf.

**Hasil:** Halaman memiliki bagian pengenalan yang terlihat jelas di bawah navigasi.

📸 **Dokumentasi:**

![Hero Panel](screenshot/08-membuat-hero-panel.png)

### 3.9 Mengatur Main Content dan Sidebar

Pada tahap ini, dibuat bagian konten utama dengan `id="main"` dan bagian tambahan dengan `id="sidebar"`.

Properti `float: left` digunakan agar konten utama dan sidebar dapat ditempatkan berdampingan. Properti `width` dan `padding` digunakan untuk mengatur lebar dan jarak isi masing-masing bagian.

**Hasil:** Layout utama mulai terbagi menjadi area konten dan sidebar.

📸 **Dokumentasi:**

![Main Content dan Sidebar](screenshot/09-main-content-sidebar.png)

### 3.10 Membuat Sidebar Widget

Sidebar dikembangkan dengan menambahkan dua widget. Widget pertama berisi judul dan daftar tautan, sedangkan widget kedua berisi judul dan paragraf informasi.

CSS digunakan untuk mengatur garis pembatas, warna judul widget, jarak isi, dan efek hover pada tautan.

**Hasil:** Sidebar menampilkan informasi tambahan dalam dua bagian yang terpisah.

📸 **Dokumentasi:**

![Sidebar Widget](screenshot/10-membuat-sidebar-widget.png)

### 3.11 Mengatur Footer

Footer merupakan bagian paling bawah halaman web. Pada praktikum ini, footer menampilkan informasi hak cipta Universitas Pelita Bangsa.

Properti `clear: both` digunakan agar footer berada di bawah elemen yang menggunakan `float`. Warna latar, padding, dan warna teks ditambahkan untuk memperjelas tampilan footer.

**Contoh kode CSS:**

```css
footer {
    clear: both;
    background-color: #1d1d1d;
    padding: 20px;
    color: #eee;
}
```

**Hasil:** Footer ditampilkan di bawah konten utama dan sidebar.

📸 **Dokumentasi:**

![Mengatur Footer](screenshot/11-mengatur-footer.png)

### 3.12 Menambahkan Content Box

Pada bagian main content, ditambahkan beberapa kotak konten yang masing-masing berisi gambar, judul, deskripsi, dan tombol View Detail.

Properti `float` digunakan agar kotak dapat tersusun dalam satu baris. Properti `width` digunakan untuk membagi area menjadi tiga bagian, sedangkan `border-radius: 50%` membuat gambar berbentuk lingkaran.

**Hasil:** Halaman menampilkan tiga kotak konten dengan susunan sejajar.

📸 **Dokumentasi:**

![Content Box](screenshot/12-menambahkan-content-box.png)

### 3.13 Menambahkan Content Artikel

Selanjutnya, ditambahkan dua elemen `article` yang berisi judul, gambar, dan paragraf. Elemen `hr` digunakan sebagai garis pemisah antarkonten.

CSS digunakan untuk mengatur jarak artikel, ukuran teks, posisi gambar, dan bentuk sudut gambar. Gambar pada artikel pertama berada di sebelah kiri, sedangkan gambar pada artikel kedua berada di sebelah kanan.

**Hasil:** Halaman memiliki bagian artikel dengan susunan teks dan gambar yang bervariasi.

📸 **Dokumentasi:**

![Content Artikel](screenshot/13-menambahkan-content-artikel.png)

---

## 🧩 4. Tugas Praktikum

### 4.1 Membuat Halaman About

Halaman About dibuat untuk menampilkan informasi atau deskripsi singkat. Halaman ini menggunakan struktur layout yang konsisten dengan halaman utama agar tampilan website tetap seragam.

Konten About dapat mencakup:
- 👋 Deskripsi singkat.
- 🎯 Tujuan atau informasi website.
- 💼 Portfolio atau informasi pendukung lainnya.

**Hasil:** Halaman About dibuat sesuai dengan kebutuhan tugas praktikum.

📸 **Dokumentasi:**

![Halaman About](screenshot/14-halaman-about.png)

### 4.2 Membuat Halaman Contact

Halaman Contact dibuat untuk menyediakan formulir yang dapat digunakan pengguna untuk mengisi informasi kontak.

Formulir terdiri dari:
- Nama.
- Email.
- Message atau pesan.
- Tombol untuk mengirim formulir.

Elemen formulir disusun menggunakan HTML dan diberikan pengaturan CSS agar lebih rapi dan mudah digunakan.

**Hasil:** Halaman Contact menampilkan formulir isian sesuai dengan instruksi tugas.

📸 **Dokumentasi:**

![Halaman Contact](screenshot/15-halaman-contact.png)

---

## ✅ 5. Validasi HTML

Validasi dilakukan untuk memeriksa apakah struktur HTML sudah sesuai dengan aturan markup yang berlaku.

Langkah validasi:

1. Buka [W3C Markup Validation Service](https://validator.w3.org/).
2. Pilih metode validasi yang sesuai, misalnya unggah file atau masukkan URL jika halaman dapat diakses secara online.
3. Jalankan proses validasi.
4. Periksa pesan kesalahan atau peringatan yang muncul.
5. Perbaiki kode jika ditemukan masalah, kemudian lakukan validasi kembali.

**Hasil:** Proses validasi digunakan untuk memeriksa dan memperbaiki struktur HTML sebelum pengumpulan.

📸 **Dokumentasi:**

![Validasi HTML](screenshot/16-validasi-html.png)

---

## 📁 6. Struktur Folder Proyek

Berikut contoh struktur folder proyek yang digunakan untuk menyimpan file praktikum dan dokumentasinya.

```text
Lab4Web/
├── lab4_box.html
├── lab4_layout/
│   ├── home.html
│   ├── artikel.html
│   ├── about.html
│   ├── kontak.html
│   └── style.css
├── screenshot/
│   ├── 01-membuat-dokumen-box-element.png
│   ├── 02-membuat-box-element.png
│   ├── 03-menerapkan-css-float.png
│   ├── 04-mengatur-clearfix.png
│   ├── 05-membuat-kerangka-layout.png
│   ├── 06-mengatur-header-layout.png
│   ├── 07-membuat-navigasi.png
│   ├── 08-membuat-hero-panel.png
│   ├── 09-main-content-sidebar.png
│   ├── 10-membuat-sidebar-widget.png
│   ├── 11-mengatur-footer.png
│   ├── 12-menambahkan-content-box.png
│   ├── 13-menambahkan-content-artikel.png
│   ├── 14-halaman-about.png
│   ├── 15-halaman-contact.png
│   └── 16-validasi-html.png
└── README.md
```

> 📌 **Catatan:** Sesuaikan struktur dan nama file di atas dengan folder yang benar-benar kamu gunakan. Jika folder `screenshot` berada di dalam `lab4_layout`, alamat gambar di README juga harus disesuaikan.

---

## 📚 7. Hasil dan Pembahasan

Berdasarkan tahapan praktikum, beberapa hal yang dipelajari adalah:

1. Elemen `div` dapat digunakan untuk membentuk kelompok kotak pada halaman web.
2. Properti CSS `float` dapat membantu menyusun elemen secara berdampingan.
3. Properti `clear` digunakan untuk mengatur posisi elemen setelah elemen yang menggunakan `float`.
4. Elemen semantik HTML5 membantu membagi struktur halaman sesuai fungsinya.
5. CSS dapat digunakan untuk mengatur warna, jarak, ukuran, posisi, dan tampilan konten.
6. Halaman About dan Contact melengkapi struktur website sederhana.
7. Validasi HTML membantu menemukan kesalahan markup sehingga kode dapat diperbaiki.

## 📝 8. Kesimpulan

Praktikum 4 memberikan pemahaman mengenai pembuatan layout halaman web menggunakan HTML dan CSS. Melalui latihan ini, saya mempelajari penggunaan elemen kotak, properti `float` dan `clear`, elemen semantik HTML5, serta penyusunan header, navigasi, hero panel, konten utama, sidebar, widget, artikel, dan footer.

Selain itu, saya juga mempraktikkan pembuatan halaman About dan Contact serta melakukan validasi HTML. Seluruh proses didokumentasikan menggunakan screenshot dan disiapkan untuk diunggah ke repository GitHub sebagai bagian dari pengumpulan tugas.

---
