---
published: true
layout: post
title: Menempatkan style CSS
---

Kita akan membuat file html di text editor Visual Studio Code, lalu kita coba styling dengan menggunakan CSS. Silahkan ketik html dibawah ini. 

```html
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Document</title>
</head>

<body>
    <h1>Membuat halaman Website sederhana</h1>

    <h4>Ini adalah tag h4 </h4>
    <ul>
        <li>Poin ini adalah list pertama</li>
        <li>Poin ini adalah list kedua</li>
        <li>Poin ini adalah list ketiga</li>
    </ul>
</body>

</html>
```
Simpan file tersebut dengan nama _websatu.html_

Apabila file html tersebut kita buka, akan muncul tampilan ini:

![File websatu.html](/images/Screen%20Shot%202019-04-01%20at%2014.24.24.png "File websatu.html")


--

Nah, sekarang kita akan styling halaman html tersebut dengan CSS.

Ada beberapa cara menempatkan style CSS kedalam website kita. 

Cara pertama:
**Inline CSS**

```html
<h2 style="color: blue;">Ini H2 berwarna Biru </h2>
<h3 style="color: red;">Ini H3 berwarna Merah </h3>

<p style="color: yellow;"> Ini paragraf berwarna kuning </p>
```

Cara kedua:
**Style Tag**

```html
<html>
<head>
  <title>Website Sederhana</title>
  <style type="text/css">
    li {
      color: blue;
    }
  </style>
</head>
```

#### Cara ketiga (recommended):
**Link Tag**

Jadi file CSS nya dipisahkan dengan file HTML. Dan ini adalah cara yang paling direkomendasikan.

--

Mari kita praktekkan! Kita akan styling file websatu.html dengan CSS, menggunakan cara **Link Tag**.

Langkah-langkahnya:

1. Buat file di Visual Studio Code, beri nama style.css atau kasih nama apa aja bebas, asalkan akhirannya ".css"
2. Isi file style.css tersebut dengan script berikut:

```css
h1 {
    color: blue;
}

li {
    color: purple;
}

h4 {
    color: green;
}
```

3. Simpan file tersebut di direktori yang sama dengan file websatu.html
4. Buka file websatu.html, tambahkan script berikut tepat dibawah tag <title>:

```html
<link rel="stylesheet" href="style.css">
```
5. Save file websatu.html. Lihat hasilnya jadi seperti ini:

![File websatu.html dengan style.css](/images/stylecss.png "File websatu.html dengan style.css")

