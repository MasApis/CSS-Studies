# Pengertian Selector CSS
Selector CSS adalah pola atau cara untuk memilih elemen HTML yang ingin diberi gaya (styling). Dengan selector, kita bisa menentukan elemen mana yang akan diubah warnanya, ukurannya, atau properti CSS lainnya.

## Jenis-Jenis Selector CSS

### 1. Selector Elemen (Type Selector)
- Memilih elemen berdasarkan nama tag HTML
- **Contoh:**
```css
p {
    color: blue; /* Semua elemen <p> akan berwarna biru */ 
}
```

### 2. Selector Class (Class Selector)
- Memilih elemen berdasarkan nilai atribut `class`
- Diawali dengan tanda titik (`.`).
- **Contoh:**
```css
.text-red {
    color: red; /* Semua elemen dengan class="text-red" akan berwarna merah */
}
```
- **Contoh HTML:**
```html
<p class="text-red">Teks ini berwarna merah.</p>
```

### 3. Selector ID (ID Selector)
- Memilih elemen berdasarkan nilai atribut `id`.
- Diawali dengan tanda pagar (`#`).
- **Catatan:** ID harus unik dalam satu halaman.
- **Contoh:**
```css
#header {
    background-color: yellow; /* Elemen dengan id-"header" akan memiliki latar belakang kuning */
}
```
- **Contoh HTML:**
```html
<div id="header">Ini adalah header.</div>
```

### 4. Selector Universal (Universal Selector)
- Memilih semua elemen di halaman.
- Dilambangkan dengan tanda bintang (`*`).
- **Contoh:**
```css
* {
    margin: 0; /* Menghapus margin default dari semua elemen */
}
```

### 5. Selector Atribut (Atribute Selector)
- Memilih elemen berdasarkan atribut tertentu.
- **Contoh:**
```css
a[target="_blank"] {
    color: green; /* Semua link dengan target="_blank" akan berwarna hijau */
}
```
- **Contoh HTML:**
```html
<a href="https://example.com" target="_blank">Link ini berwarna hijau.</a>
```

### 6. Selector Pseudo-class
- Memilih elemen berdasarkan keadaan tertentu.
- **Contoh:**
```css
a:hover {
    color: orange; /* Warna teks berubah menjadi oranye saat dihover */
}
li:first-child {
    font-weight: bold; /* Anak pertama dari <li> akan tebal */
}
```

### 7. Selector Pseudo-element
- Memilih bagian tertentu dari elemen.
- **Contoh:**
```css
p::first-line {
    font-size: 20px; /* Baris pertama teks dalam <p> akan berukuran 20 piksel */
}
p::before {
    content: ">> "; /* Menambahkan teks sebelum konten <p> */
}
```

### 8. Selector kombinasi
- Menggabungkan Kombinasi
- **Contoh:**
```css
div p {
    color: purple; /* Semua elemen <p> di dalam <div> akan berwarna ungu */
}
.container > p {
    font-size: 18px; /* Hanya <p> yang merupakan anak langsung dari .container yang memiliki ukuran font sebesar 18 piksel */
}
h1 + p {
    margin-top: 0; /* <p> yang langsung mengikuti <h1> akan memiliki margin-top 0 */
}
```

### 9. Selector Grup (Grouping Selector)
- Mengelompokkan beberapa selector yang memiliki deklarasi CSS yang sama.
- **Contoh:**
```css
h1, h2, h3 {
    color: navy; /* Semua <h1>, <h2>, dan <h3> akan berwarna navy */
}
```

## Kesimpulan 
Selector CSS adalah alat yang sangat penting untuk mengontrol tampilan elemen HTML. Dengan memahami berbagai jenis selector, kalian bisa membuat styling yang lebih spesifik dan terorganisir. Selamat mencoba!😊

---

Happy coding! 😊
