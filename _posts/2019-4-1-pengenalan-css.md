---
published: true
layout: post
---

Poin-poin yang akan kita bahas adalah:
1. Memahami fungsi CSS didalam Web Development.
2. Memperlihatkan sebuah website sebelum dan sesudah pakai CSS.
3. Mengerti tentang aturan main menggunakan CSS. Biar ngga bingung nanti.

--

**CSS kependekkan dari Cascading Style Sheet.**
Cascading itu artinya urutan prioritas. Style Sheet artinya Bahasa Desain. Jadi si CSS ini gunanya untuk mengatur format tampilan sebuah website (menggunakan bahasa desain / style sheet language) berdasarkan urutan-urutan tertentu. Kenapa harus ada urutannya? Karena setiap element HTML pada suatu website, itu bisa diterapkan berbagai style. Jadi bukan satu style satu element, melainkan satu element bisa banyak style. Hal tersebut tentu bisa membuat konflik style, nah si CSS ini berperan penting dalam menentukan urutan style yang mana yang akan dipakai berdasarkan prioritasnya. 

Gak perlu khawatir kalau masih bingung. Nanti sambil praktek juga bakalan ketemu maksudnya. 

--

**Contoh website sebelum dan sesudah memakai CSS.**

Ini adalah halaman website sebelum menggunakan CSS
![HTML Page](/images/html.png "Halaman HTML only")

_Gambar diatas kalo kita cek source code-nya, isinya cuma file HTML._

Dan ini adalah halaman website yang sama, tapi udah diterapkan CSS
![CSS Page](/images/css.png "Halaman HTML yang sudah di format menggunakan CSS")

Terlihat jauh berbeda bukan? Dan yang kita ubah bukanlah struktur file HTML nya, melainkan file CSS nya. 


## Aturan Umum CSS ##

Format penulisan syntax CSS seperti ini:

```CSS
selector {
  property: value;
  anotherProperty: value;
}
```

Keterangan:
selector itu yang di HTML. Contohnya: h1, body, span, table, dsb.
property itu adalah style css yang ingin di terapkan kedalam suatu selector. Didalam suatu selector, bisa ada banyak property. 

--

Contoh:
Buatlah element h1 dan image di HTML dengan ketentuan sebagai berikut:
1. h1 berwarna biru, dan ukuran font sebesar 24 pixel
2. image border menggunakan warna kuning dengan ketebalan border 2 pixel.

Implementasinya:
```css
h1 {
  color: blue;
  font-size: 24px;
}

img {
  border-color: yellow;
  border-width: 2px;
}
```

Pada postingan berikutnya akan dibahas cara menempatkan file CSS di HTML.

  
 

