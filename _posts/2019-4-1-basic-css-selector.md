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

#### Element Selector
Nama lain dari Element Selector adalah selektor tag atau tipe selector. Selektor ini akan memilih elemen berdasarkan nama Tag HTML.

Tambahkan script ini pada file task.css:
```css
li {
    border: 2px solid blue;
}
```

Hasilnya akan seperti ini:

![File tasklists.html](/images/tagselector.png "Element selector pada tasklists.html")





