# Pengertian Properti teks dalam CSS
Properti teks dalam CSS adalah sekumpulan aturan yang digunakan untuk mengatur tampilan teks pada elemen HTML. Dengan properti ini, kita bisa mengontrol berbagai aspek teks seperti warna, ukuran, jenis font, perataan, jarak antar huruf atau kata, dan banyak lagi. Tujuannya adalah untuk membuat teks lebih mudah dibaca, menarik, dan sesuai dengan desain yang diinginkan.

## Penjelasan Properti Teks

### 1. `color`
Mengatur warna teks.


**Contoh**
```css
p {
    color: red;
}
```

### 2. `font-family`
Mengatur jenis font yang digunakan.
- Bisa menggunakan nama font seperti `Arial`, `Times New Roman`, atau font generik seperti `serif`, `san-serif`.
- Selalu sediakan font cadangan jika font utama tidak tersedia.
<br><br>

**Contoh**
```css
p {
    font-family: "Arial", sans-serif;
}
```

### 3. `font-size`
Mengatur ukuran font.
- Nilai bisa dalam satuan `px`, `em`, `rem`, `%`, atau kunci seperti `small`, `medium`, `large`.
<br><br>

**Contoh**
```css
p {
    font-size: 16px;
}
h1 {
    font-sze: 2em; /* 2 kali ukuran font parent */
}
```

### 4. `font-weight`
Mengatur ketebalan font.
- Nilai: `normal`, `bold`, `bolder`, `lighter`, atau angak (100-900).
<br><br>

**Contoh**
```css
p {
    font-weight: bold;
}
span {
    font-weight: 700; /* Sama seperti bold */
}
```

### 5. `font-style`
Mengatur gaya font.
- Nilai: `normal`, `italic`, `oblique`.
<br><br>

**Contoh**
```css
p {
    font-style; italic;
}
```

### 6. `text-align`
Mengatur perataan teks secara horizontal.
- Nilai: `left`, `right`, `center`, `justify`.
<br><br>

**Contoh**
```css
p {
    text-align: center;
}
```

### 7. `text-decoration`
Mengatur dekorasi teks seperti garis bawah, garis tengah, atau garis atas.
- Nilai: `none`, `underline`, `overline`, `line-through`.
<br><br>

**Contoh**
```css
a {
    text-decoration: none; /* Menghilangkan garis bawah pada link */
}
span {
    text-decoration: line-through; /* Teks dicoret */
}
```

### 8. `text-transform`
Mengatur kapitalisasi teks
- Nilai: `none`, `uppercase`, `lowercase`, `capitalize`.
<br><br>

**Contoh**
```css
p {
    text-transform: uppercase; /* Teks menjadi huruf kapital */
}
```

### 9. `line-height`
Mengatur jarak antar baris (tinggi baris).
- Nilai: angka (tanpa satuan), `px`, `em`, atau `%`.
<br><br>

**Contoh**
```css
p {
    line-height: 1.5; /* 1.5 kali ukuran font */
}
```

### 10. `letter-spacing`
Mengatur jarak antar huruf.
- Nilai: `normal`, `px`, `em`.
<br><br>

**Contoh:**
```css
p {
    letter-spacing: 2px; /* Jarak antar huruf 2 piksel */
}
```

### 11. `word-spacing`
Mengatur jarak antar kata.
- Nilai: `normal`, `px`, `em`.

**Contoh:**
```css
p {
    word-spacing: 5px; /* Jarak antar kata 5 piksel */
}
```

### 12. `text-shadow`
Menambahkan bayangan pada teks.
- Sintaks: `text-shadow: horizontal vertical blur color;`
<br><br>

**Contoh:**
```css
h1 {
    text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5); /* Bayangan teks */
}
```

### 13. `white-space`
Mengatur bagaimana spasi dan line break ditangani.
- Nilai: `normal`, `nowrap`, `pre`, `pre-wrap`, `pre-line`

**Contoh:**
```css
p {
    white-space: nowrap; /* Teks tidak akan wrap ke baris baru */
}
```

### 14. `text-overflow`
Mengatur bagaimana teks yang melebihi container ditampilkan.
- Nilai: `clip`, `ellipsis`.
- Biasanya digunakan bersama `white-space: nowrap;` dan `overflow: hidden;`
<br><br>

**Contoh**
```css
p {
    white-space: nowrap;
    overflow: hidden;
    text-overflow: ellipsis; /* Teks yang melebihi container akan dipotong dengan ... */
}
```

---

Happy coding! 😊
