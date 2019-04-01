---
layout: post
title: Basic CSS Selector
published: true
---

Perhatikan baik-baik pembahasan tentang CSS selector ini. Ada tiga hal basic yang perlu dipahami tentang CSS Selector yaitu:
1. Element
2. ID
3. Class

Masih ingat dengan aturan umum CSS yang ini?

```css
selector {
  property: value;
  anotherProperty: value;
}
```

Nah, kita akan coba gunakan berbagai macam CSS Selector yang ada. Yang tiga hal tadi.

### Praktek CSS Selector
Ikuti langkah-langkah berikut ini:

- Buat halaman HTML baru, beri nama tasklists.html, yang isinya sebagai berikut:

```html
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Daftar Tugas</title>
</head>

<body>
    <h1>Daftar Tugas Harian</h1>
    <ul>
        <li>
            <input type="checkbox">Membuat laporan keuangan
        </li>
        <li>
            <input type="checkbox">Mengisi absensi
        </li>
        <li>
            <input type="checkbox">Mengirimkan paket dokumen
        </li>
    </ul>

</body>

</html>
```

- kalau sudah, buka file tasklists.html tersebut, hasilnya akan seperti ini:

![File tasklists.html](/images/tasklistweb.png "File tasklists.html")

- silahkan coba ceklist daftar tugasnya, untuk memastikan bahwa input checkbox berfungsi.

- Selanjutnya, masih di halaman tasklists.html. Tambahkan script berikut tepat dibawah title.

```css
<link rel="stylesheet" type="text/css" href="task.css">
```

- Script diatas untuk mengkoneksikan file css dan file html. Setelah itu kita buat file css baru dengan nama task.css
- Simpan file task.css pada direktori yang sama dengan file tasklists.html

Selanjutnya kita akan styling halaman tasklists.html melalui file task.css, menggunakan metode Element Selector, ID Selector, dan Class Selector.

--

### Element Selector
Nama lain dari Element Selector adalah selektor tag atau tipe selector. Selektor ini akan memilih elemen berdasarkan nama Tag HTML.

Tambahkan script ini pada file task.css:
```css
li {
    border: 2px solid blue;
}
```

Hasilnya akan seperti ini:

![File tasklists.html](/images/tagselector.png "Element selector pada tasklists.html")


### ID Selector
Selector ID bersifat unik. Hanya boleh digunakan oleh satu element pada sebuah halaman web. Tapi, selektor ID boleh lebih dari satu pada satu halaman web. Selector ID ditandai dengan tanda (#).

Ubah file tasklists.html di tag "li: Mengirimkan paket dokumen" menjadi seperti ini:

```html
        <li id="special">
            <input type="checkbox">Mengirimkan paket dokumen
        </li>
```

Kita boleh kasih nama lain misalnya _li id="unique"_ atau _li id="specific"_
Terserah kita. Asal jangan ngasal ngasih nama aja. Dalam hal ini, kita kasih nama _id="special"_

Sekarang kita buka file task.css, lalu tambahkan script berikut:

```css
#special {
    background: orange;
}
```

Hasilnya akan menjadi seperti ini:

![File tasklists.html](/images/idselector.png "ID selector pada tasklists.html")


### Class Selector
Hampir sama dengan selector ID, selector Class digunakan untuk memilih elemen berdasarkan nama class yang diberikan. Selektor class ditandai dengan tanda titik "."

Ubah file tasklists.html pada tag "li: Membuat laporan keuangan" dan "li: Mengisi absensi" menjadi seperti ini:

```html
    <ul>
        <li class="completed">
            <input type="checkbox">Membuat laporan keuangan
        </li>
        <li class="completed">
            <input type="checkbox">Mengisi absensi
        </li>
        <li id="special">
            <input type="checkbox">Mengirimkan paket dokumen
        </li>
    </ul>
```
Kita boleh kasih nama lain misalnya li class="Finished".
Pada contoh kali ini, kita gunakan nama class nya: li class="completed".

Sekarang buka file task.css, lalu tambahkan script berikut:

```css
.completed {
    text-decoration: line-through;
}
```

Sebelum melihat hasilnya, pada file tasklist.html tambahkan atribut "checked" pada tag input type="checkbox"
Seperti ini:

```html
        <li class="completed">
            <input type="checkbox" checked>Membuat laporan keuangan
        </li>
        <li class="completed">
            <input type="checkbox" checked>Mengisi absensi
        </li>
```

Save files, lalu lihat hasilnya menjadi seperti ini:

![File tasklists.html](/images/selectorclass.png "Class selector pada tasklists.html")












