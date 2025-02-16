# Apa itu Flexbox?
Flexbox (Flexible Box Layout) adalah model layout dalam CSS yang dirancang untuk memudahkan pengaturan tata letak elemen dalam satu dimensi (baik secara horizontal maupun vertikal). Flexbox sangat berguna untuk membuat layout yang responsif dan dinamis.

## Konsep Dasar Flexbox
Flexbox bekerja dengan dua komponen utama:
1. **Flex Container**: Elemen yang menjadi wadah (container) untuk elemen-elemen lain.
2. **Flex Items**: Elemen-elemen yang berada di dalam flex container.

## Cara Menggunakan Flexbox
Untuk menggunakan Flexbox, kita perlu mengatur properti `display` pada flex container menjadi `flex` atau `inline-flex`.
<br><br>
Contoh:

```css
.container {
    display: flex; /* Membuat container menjadi flex container */
}
```

## Properti untuk Flex Container
Berikut adalah properti-properti yang bisa digunakan pada flex container:
1. `flex-direction`
    - Mengatur arah penempatan flex items (secara horizontal atau vertikal).
    - Nilai:
        - `row` (default): Penampatan secara horizontal (kiri ke kanan).
        - `row-reverse`: Penempatan secara horizontal (kanan ke kiri)
        - `column`: Penempatan secara vertikal (atas ke bawah).
        - `column-reverse`: Penempatan secara vertikal (bawah ke atas).
    - **Contoh:**
    ```css
    .container {
        flex-direction: row; /* Penempatan horizontal */
    }
    ```

2. `justify-content`
    - Mengatur penempatan flex items sepanjang sumbu utama (main axis).
    - Nilai:
        - `flex-start` (default): Items ditempatkan di awal container.
        - `flex-end`: Items ditempatkan di akhir container.
        - `center`: Items ditempatkan di tengah container.
        - `space-between`: Ruang di antara items dibagi rata.
        - `space-around`: Ruang di sekitar items dibagi rata.
        - `space-evenly`: Ruang di antara dan sekitar items dibagi rata.
    - **Contoh:**
    ```css
    .container {
        justify-content: space-between; /* Ruang di antara items dibagi rata */
    }
    ```

3. `align-items`
    - Mengatur penempatan flex items sepanjang sumbu silang (cross axis).
    - Nilai:
        - `stretch` (default): Items direntangkan untuk mengisi container.
        - `flex-start`: Items ditempatkan di awal sumbu silang.
        - `flex-end`: Items ditempatkan di akhir sumbu silang.
        - `center`: Items ditempatkan di tengah sumbu silang.
        - `baseline`: Items disejajarkan berdasarkan baseline teks.
    - **Contoh:**
    ```css
    .container {
        align-items: center; /* Items ditempatkan di tengah sumbu silang */
    }
    ```

4. `flex-wrap`
    - Mengatur apakah flex items boleh pindah ke baris baru jika tidak muat dalam satu baris.
    - Nilai:
        - `nowrap` (default): Items tidak akan pindah ke baris baru.
        - `wrap`: Items akan pindah ke baris baru jika tidak muat.
        - `wrap-reverse`: Items akan pindah ke baris baru secara terbalik.
    - **Contoh:**
    ```css
    .container {
        flex-wrap: wrap; /* Items akan pindah ke baris baru jika tidak muat */
    }
    ```

5. `align-content`
    - Mengatur penempatan baris flex items sepanjang sumbu silang jika ada ruang extra.
    - Nilai:
        - `stretch` (default): Baris direntangkan untuk mengisi ruang yang tersedia.
        - `flex-start`: Baris ditempatkan di awal sumbu silang.
        - `flex-end`: Baris ditempatkan di akhir sumbu silang.
        - `center`: Baris ditempatkan di tengah sumbu silang.
        - `space-between`: Ruang di antara baris dibagi rata.
        - `space-around`: Ruang di sekitar baris dibagi rata.
    - **Contoh:**
    ```css
    .container {
        align-content: space-between; /* Ruang di antara baris dibagi rata */
    }
    ```

## Properti untuk Flex Items
Berikut adalah properti-properti yang bisa digunakan pada flex-items:
1. `order`
    - Mengatur urutan tampilan flex items.
    - Nilai: Angka (default: 0). Semakin kecil angkanya, semakin awal item ditampilkan.
    - **Contoh:**
    ```css
    .item {
        order: 2; /* Item ini akan ditempilkan setelah item dengan order 1 */
    }
    ```

2. `flex-grow`
    - Mengatur seberapa besar item dapat tumbuh (mengisi ruang yang tersedia).
    - Nilai: Angka (default: 0).
    - **Contoh:**
    ```css
    .item {
        flex-grow: 1; /* Item akan mengisi ruang yang tersedia */
    }
    ```

3. `flex-shrink`
    - Mengatur seberapa kecil item dapat menyusut jika tidak ada cukup ruang
    - Nilai: Angka (default: 1).
    - **Contoh:**
    ```css
    .item {
        flex-shrink: 0; /* Item ini tidak akan menyusut */
    }
    ```

4. `flex-basis`
    - Mengatur ukuran awal item sebelum ruang tersisa dibagikan.
    - Nilai: Panjang (px, %, em, dll) atau `auto` (default).
    - **Contoh:**
    ```css
    .item {
        flex-basis: /* Ukuran awal item adalah 200px */
    }
    ```

5. `align-self`
    - Mengatur penempatan item secara individual sepanjang sumbu silang.
    - Nilai: `auto`, `flex-start`, `flex-end`, `center`, `baseline`, `stretch`.
    - **Contoh:**
    ```css
    .item {
        align-self: flex-end; /* Item ini ditempatkan di akhir sumbu silang */
    }
    ```

## Studi Kasus: Membuat Layout Sederhana dengan Flexbox

**HTML:**
```html
<!DOCTYPE html>
<html>
<head>
    <title>Studi Kasus Flexbox</title>
    <link rel="stylesheet" type="text/css" href="styles.css">
</head>
<body>
    <div class="container">
        <div class="item">Item 1</div>
        <div class="item">Item 2</div>
        <div class="item">Item 3</div>
    </div>
</body>
</html>
```

**CSS:**
```css
/* Flex Container */
.container {
    display: flex; /* Membuat container menjadi flex container */
    justify-content: space-between; /* Ruang di antara items dibagi rata */
    align-items: center; /* Items ditempatkan di tengah sumbu silang */
    background-color: lightblue;
    padding: 20px;
}

/* Flex Items */
.item {
    background-color: lightcoral;
    padding: 20px;
    margin: 10px;
    text-align: center;
    flex-grow: 1; /* Items akan mengisi ruang yang tersedia */
}
```
### Hasil Studi Kasus
- **Flex Container:** Sebuah kotak dengan latar belakang biru muda yang menampung tiga item.
- **Flex Items:** Tiga kotak dengan latar belakang merah muda yang ditempatkan secara horizontal dengan jarak yang rata.


## Tips
1. **Gunakan Developer Tools**:<br>
    Buka Developer Tools di browser (tekan `F12` atau `Ctrl+Shift+I)` dan inspect elemen untuk melihat bagaimana Flexbox bekerja.
2. **Coba Kombinasi Properti**:<br>
   Coba ubah nilai-nilai properti seperti `flex-direction`, `justify-content`, dan `align-items` untuk memahami pengaruhnya.
3. **Praktik Langsung**:<br>
   Buat layout sederhana seperti navbar, card, atau grid menggunakan Flexbox.

---

Happy coding! 😊
