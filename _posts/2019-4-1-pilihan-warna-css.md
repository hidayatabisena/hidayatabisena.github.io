---
published: true
layout: post
title: Pilihan Warna CSS
---

Di contoh-contoh sebelumnya untuk pemilihan warna, kita baru menggunakan warna-warna plain. Pada kenyataannya, para desainer website suka membuat warna-warna yang spesifik. Tidak cukup hanya dengan mendeklarasikan Red, atau Green, atau Blue, tapi ada semacam color palletes yang bisa kita gunakan. 


Ada beberapa cara untuk menggunakan warna di CSS:

### CSS HEXADECIMAL
Contoh: Warna hitam kode hexadecimal-nya adalah #000000.

Ada banyak pilihan warna di CSS, dan kita tidak harus menghapal kode-kode warnanya. Kita bisa menggunakan [Color Picker Website](https://www.webfx.com/web-design/color-picker/ "Color Picker Website")

Silahkan buka website tersebut. 


### CSS RGB
Contoh: Warna Purple, bila ditulis dalam kode RGB akan menjadi seperti ini -> rgb(100, 0, 100);


### CSS RGBA
Hampir sama dengan CSS RGB, hanya saja untuk RGBA, ada tambahan Alpha yaitu untuk transparan.

contoh: warna hijau yang ditambahkan alpha transparant -> rgba(11, 99, 150, .2);

Silahkan berkesperimen untuk alpha-nya dari angka 1 s.d angka .9. Misal rgba(11, 99, 150, .9)

--

Praktek. 
Silahkan edit file style.css yang sebelumnya dibuat, menjadi seperti ini:

```css
h1 {
    color: #176DB7;
}

li {
    color: rgb(133, 190, 67);
}

h4 {
    color: rgba(11, 99, 150, .2);
}
```

Save. Kemudian buka lagi file websatu.html, hasilnya menjadi seperti ini:

![File websatu.html dengan style.css](/images/colorcss.png "File websatu.html dengan style.css")









