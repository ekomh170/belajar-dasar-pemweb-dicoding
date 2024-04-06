# Pengenalan CSS

CSS (Cascading Style Sheet) adalah standar dari W3C yang digunakan untuk mengatur tampilan suatu halaman web yang ditulis dalam HTML. Dengan CSS, kita dapat mengontrol layout, warna, font, dan berbagai aspek visual lainnya dari elemen-elemen HTML. Berikut ini adalah rangkuman materi Pengenalan CSS yang telah dipelajari:

## Keuntungan dan Cara CSS Bekerja

### Keuntungan CSS:
1. **Mengontrol Layout Secara Presisi:** CSS memungkinkan pengaturan layout yang tepat dan presisi.
2. **Menghindari Pekerjaan Berulang:** Styling dapat diterapkan pada beberapa berkas HTML menggunakan satu berkas CSS.
3. **Didukung oleh Banyak Browser:** Mayoritas browser saat ini mendukung CSS versi 2, dengan beberapa browser populer juga mendukung CSS versi 3.

## Menulis Aturan Styling

Dalam CSS, aturan styling terdiri dari dua bagian: selector (identitas elemen yang akan diatur) dan deklarasi (instruksi yang diterapkan pada selector).

![Aturan Styling CSS](dos:d62420ba96cd1b764eab1ad1f644e42b20231130101852.jpeg)

## Melampirkan Styling pada Dokumen HTML

Ada tiga cara untuk melampirkan styling pada dokumen HTML:

### 1. External Style Sheet
Berkas terpisah (.css) yang dihubungkan dengan dokumen HTML menggunakan tag `<link>` di dalam bagian `<head>`.

```html
<head>
  <meta charset="UTF-8" />
  <title>Judul Dokumen</title>
 
  <!-- Impor berkas CSS Anda -->
  <link rel="stylesheet" href="style.css">
</head>
```

### 2. Embedded Style Sheet
Aturan styling ditulis di dalam elemen `<style>` di dalam bagian `<head>` pada dokumen HTML.

```html
<head>
  <meta charset="UTF-8" />
  <title>Judul Dokumen</title>
 
  <style>
    h1 {
      color: green;
    }
  </style>
</head>
```

### 3. Inline Style
Styling langsung diterapkan pada elemen HTML menggunakan atribut `style`.

```html
<nama-elemen style="color: green">Konten dari Elemen HTML</nama-elemen>
```

## CSS Conception

### 1. Inheritance
Properti style tertentu dapat diwariskan dari sebuah elemen ke elemen-elemen di dalamnya. Contohnya, styling yang ditetapkan untuk elemen `<body>` akan diterapkan pada seluruh child-elements.

### 2. Group Selector
Jika beberapa selector memiliki penerapan properti yang sama, mereka dapat digabungkan menggunakan group selector untuk meminimalkan penulisan kode yang berulang.

### 3. Rule Order
Aturan dalam CSS mengalir dari atas ke bawah, sehingga urutan penulisan aturan sangat penting, terutama saat terjadi konflik.

```css
p {
  color: red;
}
 
p {
  color: blue;
}
```

Dalam kasus di atas, warna teks akan menjadi biru karena aturan terakhir yang dideklarasikan.

Dengan pemahaman tentang CSS ini, kita dapat membuat tampilan yang menarik dan terstruktur pada halaman web kita.