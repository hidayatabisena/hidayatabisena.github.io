---
layout: post
title: CSS Background dan CSS Border
published: true
---

Property Background dan property Border pada CSS digunakan untuk memberikan warna dan border pada sebuah element HTML. 

Contoh:
#### Memberikan warna background ke element <body> dan <h4>
Silahkan buka file style.css, lalu modifikasi menjadi seperti ini:

```css
h4 {
    color: rgba(11, 99, 150, .2);
    background: rgba(198, 73, 166);
}

body {
    background: #C6C449;
}
```

Hasilnya menjadi seperti ini:

![HTML Page](/images/backgroundcss.png "Halaman websatu.html yang telah diberi background")

--

Atau, bisa juga dengan menambahkan Image ke background body. Silahkan modifikasi tag body seperti ini:

```css
body {
    background: url(https://img.freepik.com/free-photo/old-wooden-texture-background-vintage_55716-1138.jpg?size=626&ext=jpg);
    background-repeat: no-repeat;
    background-size: cover;
}
```

Hasilnya menjadi seperti ini:

![HTML Page](/images/backgroundimagecss.png "Halaman websatu.html yang telah diberi background image")

catatan:
- Untuk dapetin url yang di background, itu bisa cari gambar di google, terus copy url image-nya. 
- Coba dihapus si "background-repeat" dan "background-size" nya. Coba bandingkan hasilnya gimana. 

--

Contoh yang Border:
Modifikasi script yang h1 di file style.css menjadi seperti ini:

```css
h1 {
    color: #176DB7;
    border-color: azure;
    border-width: 5px;
    border-style: solid;
}
```

Hasilnya akan menjadi seperti ini:

![HTML Page](/images/bordercss.png "Halaman websatu.html yang telah diberi border")




