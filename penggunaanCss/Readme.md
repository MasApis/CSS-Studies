# 3 Cara Menggunakan CSS di HTML
Ada tiga cara utama untuk menerapkan CSS ke dalam HTML:

## 1. Inline CSS
CSS ditulis langsung di dalam atribut `style` pada elemen HTML. <br>
Contoh:
```css
<p style="color: blue; font-size: 16px;">Ini adalah teks berwarna biru.</p>
```
### Kelebihan 
- Cepat dan mudah untuk perubahan kecil.

### Kekurangan
- Tidak efisien untuk banyak elemen.
- Sulit dikelola jika website besar.

## 2. Internal CSS
CSS ditulis di dalam tag `<style>` di bagian `<head>` dokumen HTML. <br>
Contoh:
```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            p {
                color: green;
                font-size: 18px;
            }
            h1 {
                color: red;
            }
        </style>
    </head>
    <body>
        <h1>Judul</h1>
        <p>Ini adalah teks berwarna merah.</p>
    </body>
</html>
```
### Kelebihan
- Cocok untuk styling satu halaman.
- Lebih terorganisir daripada inline CSS.

### Kekurangan
- Tidak efisien untuk banyak halaman

## 3. External CSS
CSS ditulis di file terpisah dengan extensi `.css`, lalu dihubungkan ke HTML menggunakan tag `<link>` di bagian `<head>`.
- File HTML:
```html
<!DOCTYPE html>
<html>
    <head>
        <link rel="stylesheet" type="text/css" href="styles.css">
    </head>
    <body>
        <h1>Judul</h1>
        <p>Ini adalah teks dengan gaya dari file CSS eksternal.</p>
    </body>
</html>
```
- File CSS (`styles.css`):
```css
p {
    color: purple;
    font-size: 20px;
}
h1 {
    color: orange;
}
```

### Kelebihan:
- Paling efisien untuk website besar.
- Mudah dikelola dan diubah.
- File CSS bisa digunakan di banyak halaman.

### Kekurangan:
- Membutuhkan file terpisah.


## Cara Mana yang Harus Dipilih?
- Gunakan **Inline CSS** hanya untuk perubahan kecil atau testing.
- Gunakan **Internal CSS** jika styling hanya dibutuhkan di satu halaman.
- Gunakan **External CSS** untuk website besar atau multi-halaman.

---

Happy coding! 😊
