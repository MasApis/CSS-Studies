# Color and Background Color

## 1. Properti `Color`
Properti `color` digunakan untuk mengatur warna **teks** di dalam elemen HTML.
<br><br>
Nilai yang Dapat Digunakan:

- **Nama Warna**: Misalnya `red`, `blue`, `green`, dll.
<br>
Contoh:

```css
p {
    color: red;
}
```

- **Kode Hex**: Misalnya `#FF0000` (merah), `#00FF00` (hijau), `#0000FF` (biru).
<br>
Contoh:

```css
p {
    color: #FF0000;
}
```

- **RGB/RGBA**:
  * `rgb(red, green, blue)`: Nilai merah, hijau, dan biru dalam rentang 0-255. 
  * `rgba(red, green, blue, alpha)`: Sama seperti RGB, tetapi dengan tambahan alpha(transparansi) dalam rentang 0-1.
  <br>
  Contoh:

```css
p {
    color: rgb(255, 0, 0); /* merah */
}
span {
    color: rgba(255, 0, 0, 0.5); /* merah dengan transparansi 50% */
}
```

- **HSL/HSLA**:
  * `hsl(hue, saturation, lightness)`: Hue(warna) dalam rentang 0-360, saturation(kejenuhan) dan lightness (kecerahan) dalam presentase.
  * `hsla(hue, saturation, lightness, alpha)`: Sama seperti HSL, tetapi dengan tambahan alpha(transparansi) dalam rentang 0-1.
  <br>
  Contoh:

```css
p {
    color: hsl(120, 100%, 50%); /* Hijau cerah */
}
span {
    color: hsla(120, 100%, 50%, 0.5); /* Hijau cerah dengan transparansi 50% *? */
}
```


## Properti `background-color`
Properti `background-color` digunakan untuk mengatur warna **latar belakang** dari elemen HTML.
<br><br>
Nilai yang Dapat Digunakan:

Sama seperti `color`, nilai yang dapat digunakan adalah:

- Nama warna (misalnya `yellow`).
- Kode hex (misalnya `#FFFF00`).
- RGB/RGBA (misalnya `rgb(255, 255, 0)`).
- HSL/HSLA (misalnya `hsl(60, 100%, 50%)`).
<br>
Contoh:

```css
div {
    background-color: yellow; /* Latar belakang kuning */
}
p {
    background-color: #00FF00; /* Latar belakang hijai (kode hex) */
}
span {
    background-color: rgba(0, 0, 255, 0.3); /* Latar belakang biru dengan transparansi 30% */
}
```


## Perbedaan Utama `color` dan `background-color`
- `color`: Mengatur warna teks.
- `background-color`: Mengatur warna latar belakang elemen.

## Contoh Gabungan `color` dan `background-color`
Ada terdapat di file index.html yaaaa

---

Happy coding! 😊
