# What is CSS ?

## Apa itu sih itu CSS ?
CSS (Cascading Style Sheets) adalah bahasa yang digunakan untuk mengatur tampilan dan gaya dari sebuah halaman web. Jika kita bayangkan sebuah website seperti rumah, maka HTML adalah struktur dasarnya (seperti dinding, pintu, dan jendela), sedangkan CSS adalah dekorasinya (seperti cat dinding, tirai, atau perabotan).

Dengan CSS, kita bisa mengubah warna teks, ukuran font, jarak antar elemen, tataletak, dan banyak lagi. Intinya, CSS membuat website terlihat lebih menarik danrapi sesuai keinginan kita.

## Aturan CSS 
Dalam penulisan CSS juga ada pengaturannya loh. Hampir seluruhnya ditulis dengancara seperti ini:
```css
selector {
    property: value;
}
```

1. Selector
Selector adalah cara untuk memilih elemen HTML yang ingin kita beri gaya. Contohnya:
- `<h1>` -> memilih semua elemen `<h1>`
- `.class` -> Memilih elemen dengan class tertentu (contoh: `<div class="text-red">`).
- `#id` -> Memilih elemen dengan id tertentu (contoh: `<p id="id">`).

2. Declaration Block
Declaration Block adalah bagian yang diawal dengan tanda kurung kurawal `{}` dan berisi satu atau lebih **deklarasi**(property dan value).

3. Property dan Value
- **Property**: Gaya yang ingin diubah, seperti `color`, `font-size`, `margin`, dll.
- **Value**: Nilai dari property tersebut, seperti `red`, `16px`, `20px`, dll.

Contoh:
```css
h1 {
    color: blue;
    font-size: 24px;
}
```

Penjelasan:
- `h1` adalah selector (memilih semua elemen `<h1>`).
- `color: blue;` adalah deklarasi pertama: mengubah warna teks menjadi biru.
- `font-size: 24px;` adalah deklarasi kedua: mengubah ukuran font menjadi 24 piksel.

## Aturan Tambahan dalam penulisan CSS

1. Setiap deklarasi diakhiri dengan titik koma (`;`)
Contoh:
```css
p {
    color: red;
    font-size: 16px;
}
```
2. Selector bisa digabung (grouping)
Jika beberapa selector memiliki deklarasi yang sama, kita bisa menggabungkannya dengan koma (`,`).
Contoh:
```css
h1, h2, h3 {
    color: green;
    font-family: Arial;
}
```

3. Komentar dalam CSS
Komentar digunakan untuk menambahkan catatan yang tidak akan dieksekusi oleh browser. Komentar diawali dengan `/*` dan diakhiri dengan `*/`.
Contoh:
```css
/* Ini adalah komentar */
p {
    color: red;
}
```
4. Case Sensitivity
CSS tidak case-sensitive untuk nama property dan value, tetapi biasanya ditulis dalam huruf kecil untuk konsistensi.
Contoh:
```css
p {
    COLOR: RED; /* Bisa, tapi tidak disarankan */
    color: red; /* Lebih disarankan */
}
```
5. Spasi dan Identasi
Spasi dan identasi tidak mempengaruhi hasil, tetapi membuat kode lebih mudah dibaca.
Contoh:
```css
p {
    color: red;
    font-size: 16px;
}
```

---

Happy coding! 😊






