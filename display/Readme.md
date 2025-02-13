# Properti `display` dalam CSS
Properti `display` adalah salah satu properti CSS yang paling penting untuk mengontrol tata letak (layout) elemen HTML. Properti ini menentukan bagaimana sebuah elemen ditampilkan di halaman web.

## Nilai-nilai Utama Properti `display`

### 1. `block`
- Elemen akan ditampilkan sebagai blok, artinya elemen akan mengambil lebar penuh dari parent-nya dan dimulai dari baris baru.
- Contoh elemen block: `<div`>, `<p>`, `<h1>`, hingga `<h6>`.
- **Contoh CSS:**
```css
.block-example {
    display: block;
    background-color: lightblue;
    padding: 10px;
    margin: 10px 0;
}
```

### 2. `inline`
- Elemen akan ditampilkan sebaris dengan elemen lain dan hanya mengambil ruang sesuai dengan kontennya.
- Contoh elemen inline: `<span>`, `<a>`, `<strong>`.
- **Contoh CSS:**Properti display adalah salah satu properti CSS yang paling penting untuk mengontrol tata letak (layout) elemen HTML. Properti ini menentukan bagaimana sebuah elemen ditampilkan di halaman web.
```css
.inline-example {
    display: inline;
    background-color: lightcoral;
    padding: 5px;
}
```

### 3. `inline-block`
- Gabungan dari `inline` dan `block`. Elemen akan ditampilkan sebaris seperti `inline`, tetapi bisa diatur lebar dan tingginya seperti `block`.
- **Contoh CSS:**
```css
.inline-block-example {
    display: inline-block;
    width: 100px;
    height: 50px;
    background-color: lightgreen;
    padding: 10px;
    margin: 5px;
}
```

### 4. `none`
- Elemen tidak akan ditampilkan sama sekali dan tidak mengambil ruang di halaman.
- **Contoh CSS:**
```css
.none-example {
    display: none;
}
```

### 5. `flex`
- Elemen akan menjadi flex container, dan anak-anaknya (child elements) akan mengikuti aturan flexbox.
- **Contoh CSS:**
```css
.flex-example {
    display: flex;
    justify-content: space-between;
    background-color: lightyellow;
    padding: 10px;
}
```

### 6. `Grid`
- Elemen akan menjadi grid container, dan anak-anaknya akan mengikuti aturan grid layout.
- **Contoh CSS:**
```css
.grid-example {
    diplay: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 10px;
    background-color: lightpink;
    padding: 10px;
}
```

## Studi Kasus: Membuat Layout Sederhana
Kita akan membuat layout sederhana menggunakan properti `display` dan Box Model. Layout ini terdiri dari:
1. Sebuah header.
2. Sebuah sidebar dan konten utama yang ditata secara horizontal
3. Sebuah footer.

### HTML:
Ada terdapat di file index.html

### CSS:
Ada terdapat di file style.css

### Hasil Studi Kasus
1. **Header**: Sebuah kotak dengan latar belakang warna merah dan teks "Header" di tengah.
2. **Container**: Menggunakan `display: flex` untuk menata sidebar dan konten utama secara horizontal.
    * **Sidebar**: Kotak dengan lebar 300px dan latar belakang merah muda.
    * **Konten Utama**: Kotak yang mengisi sisa ruang dengan latar belakang hijau muda.
3. **Footer**: Kotak dengan latar belakang merah muda dan teks "Footer" di tengah.

### Tips untuk Praktek
1. **Coba Ubah Nilai `display`**:
    * Ganti `display: flex` pada `.container` menjadi `display: block` atau `display: grid` dan lihat perubahannya.
2. **Tambahkan Margin dan Padding**:
    * Coba tambahkan margin atau padding pada elemen-elemen yang ada untuk memamahami pengaruhnya terhadap Box Model.
3. **Gunakan Developer Tools**:
    * Buka Developer Tools di browser (tekan `F12` atau `Ctrl+Shift+I`) dan inspect elemen untuk melihat Box Model dan tata letaknya.

---

Happy coding! 😊
