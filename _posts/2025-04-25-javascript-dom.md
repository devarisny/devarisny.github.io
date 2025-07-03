---
layout: post
title: "Pratikum 5 - HTML Link dan List"
---

Penjelasan Tentang Link dan List pada HTML

![HTML Link dan Lists](/assets/images/ror.jpg)

# HTML: Link dan List

##  Link (Tautan) di HTML
Link di HTML digunakan untuk menghubungkan ke halaman lain atau situs lain. Tag yang digunakan adalah `<a>`.
```html
<a href="https://www.google.com">Buka Google</a>
- `href` → Menentukan URL tujuan.
- Bisa berupa **absolute URL** (misalnya `https://`) atau **relative URL** (`/halaman.html`).

 **Contoh:**
```html
<a href="https://google.com" target="_blank">Buka Google di tab baru</a>
<a href="halaman.html">Link ke halaman lokal</a>
<a href="mailto:email@example.com">Kirim Email</a>
```
- `target="_blank"` → Buka link di tab baru.
- `mailto:` → Membuka aplikasi email dengan alamat tertentu.

---

##  HTML List
HTML punya dua jenis list utama: 

### 1️ **Ordered List (Daftar Berurutan)**
Menggunakan `<ol>` dengan item `<li>`, secara default diberi nomor.  
```html
<ol>
  <li>HTML</li>
  <li>CSS</li>
  <li>JavaScript</li>
</ol>
```
**Bentuk lain (angka romawi, alfabet, dsb.):**
```html
<ol type="A">
  <li>Item A</li>
  <li>Item B</li>
</ol>
```
- `type="1"` → Angka (default).
- `type="A"` → Huruf kapital.
- `type="a"` → Huruf kecil.
- `type="I"` → Angka Romawi besar.
- `type="i"` → Angka Romawi kecil.


### 2️ **Unordered List (Daftar Tidak Berurutan)**
Menggunakan `<ul>` dengan item `<li>`, ditandai dengan bullet (•).  
```html
<ul>
  <li>Jeruk</li>
  <li>Apel</li>
  <li>Semangka</li>
</ul>
```

 **Custom Bullet List dengan CSS:**
```html
<ul style="list-style-type: square;">
  <li>Python</li>
  <li>Java</li>
</ul>
```
- `list-style-type: disc;` → Default (bulat).
- `list-style-type: square;` → Kotak.
- `list-style-type: circle;` → Lingkaran kosong.
- `list-style-type: none;` → Tanpa bullet.

---

##  Link di dalam List
Bisa menggabungkan `<a>` ke dalam `<li>`:
```html
<ul>
  <li><a href="https://github.com">GitHub</a></li>
  <li><a href="https://stackoverflow.com">Stack Overflow</a></li>
</ul>
```

---

##  Kesimpulan
- **Link (`<a>`)** digunakan untuk membuat tautan ke halaman lain.
- **Ordered List (`<ol>`)** digunakan untuk daftar bernomor.
- **Unordered List (`<ul>`)** digunakan untuk daftar dengan bullet.
- Bisa dikombinasikan dengan **CSS** untuk tampilan lebih menarik.

