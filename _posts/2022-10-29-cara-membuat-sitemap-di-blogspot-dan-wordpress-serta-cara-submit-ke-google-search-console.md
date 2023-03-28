---
id: 158
title: 'Cara Membuat Sitemap di Blogspot dan WordPress Serta Cara Submit ke Google Search Console'
date: '2022-10-29T21:49:00+00:00'
author: admin
layout: post
guid: 'http://localhost/wordpress/index.php/2022/10/29/cara-membuat-sitemap-di-blogspot-dan-wordpress-serta-cara-submit-ke-google-search-console/'
permalink: /index.php/2022/10/29/cara-membuat-sitemap-di-blogspot-dan-wordpress-serta-cara-submit-ke-google-search-console/
blogger_blog:
    - webidevloper.blogspot.com
blogger_author:
    - IDEV.My.ID
blogger_internal:
    - /feeds/2636143461486592706/posts/default/556207105934711491
categories:
    - TutorialBlogger
---

<div><div>Cara membuat peta situs merupakan artikel kedua dalam seri Google Search Console. Bagi Anda yang belum memiliki dan mengintegrasikan GSC dengan blog/website, silakan buat dulu.

**Seri Google Search Console:**

1. Membuat dan Memasang Google Search Console
2. Tutorial Membuat Sitemap (artikel ini)
3. Fitur-Fitur Google Search Console dan Cara Membaca Laporannya
4. Robot.txt
5. menambahkan properti dan menambah user
6. Change of Address Tool: Pindah Domain TLD atau Migrasi dari Blogspot ke WordPress
7. Tolak tautan balik &amp; penghapusan URL
8. Optimasi SEO dari data-data yang ada di GSC

<div data-htoc-state="expanded"><span><span>Daftar isi</span><span><svg height="16" width="16" xmlns="http://www.w3.org/2000/svg"><g fill="#444"><path d="M15 7H1c-.6 0-1 .4-1 1s.4 1 1 1h14c.6 0 1-.4 1-1s-.4-1-1-1z"></path><path d="M15 1H1c-.6 0-1 .4-1 1s.4 1 1 1h14c.6 0 1-.4 1-1s-.4-1-1-1zM15 13H1c-.6 0-1 .4-1 1s.4 1 1 1h14c.6 0 1-.4 1-1s-.4-1-1-1z"></path></g></svg></span></span><div>- [Apa Itu Peta Situs?](http://webidevloper.blogspot.com/#htoc-a)
    - [Format Peta Situs](http://webidevloper.blogspot.com/#htoc-m1)
    - [Mengapa Peta Situs Diperlukan?](http://webidevloper.blogspot.com/#htoc-m)
- [Peta Situs Blogspot](http://webidevloper.blogspot.com/#htoc-membuat-sitemap-blogspot)
    - [Cara Membuat Peta Situs di Blogger](http://webidevloper.blogspot.com/#htoc-1)
    - [Cara Submit Sitemap Blogspot ke Google Search Console](http://webidevloper.blogspot.com/#htoc-2)
- [Peta Situs WordPress.com](http://webidevloper.blogspot.com/#htoc-sitemap-wordpress-com)
    - [Cara Membuat Peta Situs WordPress.com](http://webidevloper.blogspot.com/#htoc-car)
- [Peta Situs WordPress Self-hosted](http://webidevloper.blogspot.com/#htoc-sitemap-wordpress-self-hosted)
    - [Cara Membuat Sitemap di WordPress Self-Hosted](http://webidevloper.blogspot.com/#htoc-membuat-sitemap-blogspot1)
    - [Cara Submit Sitemap WordPress Self-hosted ke Google Search Console](http://webidevloper.blogspot.com/#htoc-c)
- [Cara Menghapus Peta Situs di Google Search Console](http://webidevloper.blogspot.com/#htoc-c1)
- [Pertanyaan yang Sering Diajukan](http://webidevloper.blogspot.com/#htoc-fre)

</div></div>- - - - - -

## Apa Itu Peta Situs?

Peta Situs adalah peta situs, *mengajukan* yang digunakan untuk memberi tahu Google tentang semua laman di web kita, baik konten berupa tulisan maupun media seperti foto dan video.

***Peta situs adalah file di situs Anda yang memberi tahu Google halaman mana di situs Anda yang harus kami ketahui.***  
– GSC

Isi sitemap kira-kira seperti ini:

<figure>![Contoh peta situs](https://ik.imagekit.io/langit/2022-09/sitemap/contoh-sitemap.webp?ik-sdk-version=javascript-1.4.3&updatedAt=1662948960006)<figcaption>Contoh peta situs</figcaption></figure><figure>![Contoh indeks peta situs](https://ik.imagekit.io/langit/2022-09/sitemap/contoh-sitemap-index.webp?ik-sdk-version=javascript-1.4.3&updatedAt=1662949100711)<figcaption>Contoh indeks peta situs</figcaption></figure>### Format Peta Situs

Ada beberapa format peta situs:

- XML
- RSS
- Atom
- Teks

Format peta situs apa yang paling bagus?

Saya merekomendasikan XML karena lebih *“portabel”* dan mudah dibaca baik oleh *mesin pencari* maupun oleh manusia.

*Peta situs file* harus berada di *tuan rumah* yang sama dengan semua data web kita. Artinya, Anda tidak bisa membuat peta situs lalu menyimpannya di Google Drive, misalnya. Tapi tidak perlu khawatir, kita tidak perlu membuat *file peta situs* sendiri karena platform (Blogspot dan WordPress) sudah men-*menghasilkan* peta situs untuk kita.

### Mengapa Peta Situs Diperlukan?

Sebetulnya, jika web kita cukup kecil, dengan atau tanpa sitemap pun web kita akan tetap terindeks. Tetapi, peta situs, tetap diperlukan, terutama aabila:

- Web kita berukuran cukup besar dan kompleks. Misalnya, ratusan *pos*banyak *halaman*ada *toko*dan sebagainya.
- Terdapat halaman yang tidak nge-*tautan* satu dengan yang lainnya *(terpencil)*.
- JIka web kita relatif baru.
- Jika konten web sering berubah atau *memperbarui* dengan cepat. Misalnya, situs berita.

Sebagai catatan, seperti yang dikatakan Daniel Waisberg (Google Search Advocate), peta situs **tidak menjamin** Pencarian Google akan menelusuri (*Merangkak*dan mengindeks halaman-halaman web kita. Namun, adanya sitemap dapat membantu mesin pencari untuk memutuskan apa saja yang akan mencari dan kapan mereka melakukannya.

Bila Anda masih bingung dengan *merangkak* dan *pengindeksan*silakan jalan-jalan dulu ke “Bagaimana Search Engine Bekerja“.

- - - - - -

## Peta Situs Blogspot

Ada tiga jenis *peta situs* yang di-*menghasilkan* secara otomatis oleh Blogspot: XML, RSS, dan Atom. Di tutorial kali ini kita menggunakan sitemap XML.

Cara membuat sitemap dan submit ke Google Search Console yang saya bahas di sini mencakup blog yang masih menggunakan subdomain dan blog yang sudah menggunakan TLD. Alias, cara membuat dan *Kirimkan* *peta situs*-nya sama.

### Cara Membuat Peta Situs di Blogger

Anda hanya perlu menambahkan sufiks (akhiran) “sitemap.xml” (tanpa tanda kutip) di belakang nama domain Anda. Bisa diketikkan langsung di *browser bilah alamat*.

**Contoh:**

- Nama domain https://www.example.com
- tambah jadi https://www.example.com/**peta situs.xml**

**URL di *bilah alamat* inilah yang nanti kita salin dan masukkan di Google Search Console.**

<figure>![Cara membuat peta situs blogger](https://ik.imagekit.io/langit/2022-09/sitemap/sitemap-1.webp?ik-sdk-version=javascript-1.4.3&updatedAt=1662948960019)</figure>### Cara Submit Sitemap Blogspot ke Google Search Console

1. Masuk ke Google Search Console

Salin URL sitemap yang sudah kita persiapkan lalu masuk ke Google Search Console index sitemaps.

<div><figure>![Cara submit sitemap blogger ke Google Search Console](https://www.langitamaravati.com/wp-content/uploads/2021/07/sitemap-5.webp)</figure></div>2. Tambahkan Peta Situs Baru

 Tambahkan peta situs baru tempel URL kirim.

<div><figure>![Cara submit sitemap blogger ke Google Search Console](https://www.langitamaravati.com/wp-content/uploads/2021/07/sitemap-6.webp)</figure></div>3. selesai

Setelah peta situs di-*Kirimkan* ke Google Search Console, tunggu beberapa menit lalu tiriskan. Euh, udah mulai ngaco. Ha ha ha. Oke, setelah sukses maka akan terlihat status “success” di “Submitted sitemaps”.

<div><figure>![Cara submit sitemap blogger ke Google Search Console](https://ik.imagekit.io/langit/2022-09/sitemap/sitemap-success.webp?ik-sdk-version=javascript-1.4.3&updatedAt=1662950167522)</figure></div>- - - - - -

## Peta Situs WordPress.com

Teman-teman pengguna wordpress.com yang *paket gratis* sekalipun bisa diintegrasikan dengan Search Console.

### Cara Membuat Peta Situs WordPress.com

1. Masuk ke dashboard wordpress.com

Di WordPress.com, Anda bisa mengakes sitemap dari dashboard tools marketing.

<figure>![Cara membuat peta situs di wordpress.com](https://ik.imagekit.io/langit/2022-09/sitemap/sitemap-wpcom-1.webp?ik-sdk-version=javascript-1.4.3&updatedAt=1662962684439)</figure>2. Pilih “Lalu Lintas” gulir ke bawah peta situs

<figure>![Cara membuat peta situs di wordpress.com](https://ik.imagekit.io/langit/2022-09/sitemap/sitemap-wpcom-2.webp?ik-sdk-version=javascript-1.4.3&updatedAt=1662962684388)</figure>**Anda akan menemukan 2 macam sitemap:**

- sitemap.xml untuk mesin pencari. **Sitemap ini yang akan kita gunakan.**
- news-sitemap.xml untuk Google News.

<figure>![Cara membuat peta situs di wordpress.com](https://ik.imagekit.io/langit/2022-09/sitemap/sitemap-wpcom-3.webp?ik-sdk-version=javascript-1.4.3&updatedAt=1662962684395)</figure>Untuk mobil *kirim peta situs* wordpress.com ke Google Search Console, sama dengan cara submit sitemap *wordpress self-hosted*. Jadi, Anda bisa melihat caranya di bab selanjutnya.

- - - - - -

## Peta Situs WordPress Self-hosted

Di WordPress self-hosted, Anda bisa menggunakan banyak sekali metode untuk membuat peta situs. Anda bisa menggunakan fitur yang ada di Yoast atau menggunakan metode manual.

### Cara Membuat Sitemap di WordPress Self-Hosted

Saya menggunakan metode seperti sitemap Blogspot, tidak memakai *pengaya* apa-apa. Isi sitemap masing-masing web mungkin akan sedikit berbeda, tergantung seberapa kompleks web Anda. Kebetulan, di tutorial kali ini saya menggunakan sitemap blog saya sendiri sebagai contoh.

1. Tambahkan sufiks “sitemap.xml” di url blog kita.

<div><figure>![Cara membuat peta situs di WordPress self-hosted](https://www.langitamaravati.com/wp-content/uploads/2021/07/sitemap-2.webp)</figure></div>Tunggu, kok URL-nya jadi “wp-sitemap.xml”? Kok, bukan “sitemap.xml” saja?

Itu karena selain WordPress sebagai platform, banyak pihak juga yang bisa men-*menghasilkan* peta situs untuk kita, misalnya *pengaya*. Untuk menghindari konflik, sitemap bawaan WordPress menggunakan sufiks (akhiran) yang berbeda, jadi ada “wp”-nya.

2. Pilih peta situs yang akan digunakan

Dalam contoh, Anda bisa melihat bahwa ada 8 URL sitemap, ini disebut sitemaps index. Secara otomatis, WordPress men-*menghasilkan* beberapa tipe peta situs. Misal, post.xml untuk post/artikel blog kita, posts-project.xml untuk *jenis posting khusus* “proyek” (ini karena saya punya *jenis posting khusus*di blog Anda bisa jadi tak ada), users-1.xml untuk user.

Sitemap mana yang harus dipilih? Jika Anda ingin memasukkan semuanya, cukup pilih peta situs utama yaitu “wp-sitemap.xml”. Bila misalnya Anda ingin memasukkan *posting* dan *kategori*gunakan URL yang itu.

### Cara Submit Sitemap WordPress Self-hosted ke Google Search Console

1. Masuk ke Google Search Console

Salin URL sitemap yang sudah kita persiapkan lalu masuk ke Google Search Console index sitemaps.

<figure>![Cara submit sitemap wordpress ke google search console](https://ik.imagekit.io/langit/2022-09/sitemap/sitemap-wp-org-1.webp?ik-sdk-version=javascript-1.4.3&updatedAt=1662951973880)</figure>2. Tambahkan peta situs baru.

Tambahkan peta situs baru tempel URL kirim.

<figure>![Cara submit sitemap wordpress ke google search console](https://ik.imagekit.io/langit/2022-09/sitemap/sitemap-wp-org-1.webp?ik-sdk-version=javascript-1.4.3&updatedAt=1662951973880)</figure>Jika Anda memperhatikan, url blog kita sudah otomatis ada, tidak seperti Blogspot yang menggunakan domain property. Jadi, kita hanya perlu memasukkan sufiks “wp-sitemap.xml”. Untuk WordPress.com, masukkan sufiks “sitemap.xml”.

3. selesai

Tunggu beberapa menit, jika sukses, akan terlihat status “success” dan jumlah “Discovered URLs”.

<figure>![Cara submit sitemap wordpress ke google search console](https://ik.imagekit.io/langit/2022-09/sitemap/sitemap-wp-org-2.webp?ik-sdk-version=javascript-1.4.3&updatedAt=1662952359620)</figure>- - - - - -

## Cara Menghapus Peta Situs di Google Search Console

*Dalam hal* Anda ingin menghapus peta situs lama dan menggantinya dengan yang baru. Untuk menghapus sitemap di Blogspot atau WordPress, caranya sama.

1. Search Console indeks peta situs klik peta situs yang akan dihapus.

<figure>![Cara menghapus peta situs di Google Search Console](https://ik.imagekit.io/langit/2022-09/sitemap/remove-stiemapt-1.webp?ik-sdk-version=javascript-1.4.3&updatedAt=1662955556395)</figure>2. Klik menu ikon dot di sebelah kanan atas hapus peta situs.

<figure>![Cara menghapus peta situs di Google Search Console](https://ik.imagekit.io/langit/2022-09/sitemap/remove-sitemap-2.webp?ik-sdk-version=javascript-1.4.3&updatedAt=1662955556442)</figure><figure>![Cara menghapus peta situs di Google Search Console](https://ik.imagekit.io/langit/2022-09/sitemap/remove-sitemap-3.webp?ik-sdk-version=javascript-1.4.3&updatedAt=1662955556277)</figure>3. Akan muncul popup konfirmasi klik “hapus”.

<figure>![Cara menghapus peta situs di Google Search Console](https://ik.imagekit.io/langit/2022-09/sitemap/remove-stitemap-4.webp?ik-sdk-version=javascript-1.4.3&updatedAt=1662955556431)</figure>3. selesai 
    - Peta Situs telah berhasil dihapus. Bila Anda ingin memasukkan sitemap baru, ulangi langkah cara submit sitemap di subbab sebelumnya.

- - - - - -

## Pertanyaan yang Sering Diajukan

<div><div>**Apakah kita bisa membuat sitemap sendiri tanpa menggunakan sitemap yang di-generate oleh platform atau plugin?**Bisa.

</div><div>**Bagaimana caranya?**Terus terang, saya tidak tahu. Tapi kalau Anda cukup jago Python dan suka memperumit hidup, coba saja.

</div><div>**Apakah bisa menyimpan peta situs di tempat lain? Misal, di cloud atau Google Drive?**TIDAK. Sitemap harus berada di hosting/server yang sama dengan data-data web kita.

</div><div>**Kalau tidak submit sitemap, apakah blog kita akan tetap diindeks?**Tentu saja. Blog kita akan tetap diindeks. Tetapi dengan adanya peta situs, prosesnya bisa lebih tepat dan sedikit lebih cepat.

</div><div>**Apakah sitemap yang sama juga bisa di-submit ke Bing atau Yandex?**ya.

</div><div>**Untuk web dengan awalan URL seperti WordPress, apakah perlu mengirimkan peta situs untuk setiap properti?***Pertanyaan bagus.* IMO, tidak ada urgensi untuk melakukan itu, cukup *kirim peta situs* untuk *Properti* utama saja karena walau misalnya ada *pengguna* yang mengakses *Properti* lain, kan, akan tetap di-*mengalihkan* ke *Properti* utama.

</div><div>**Untuk Blogspot, jika kita sudah submit sitemap format XML, apakah kita perlu submit format RSS atau atom?**Boleh-boleh saja.

</div><div>**Perlukah kita link sitemap di footer blog seperti privacy policy?**Tergantung seberapa besar blog atau website kita. Kalau untuk bloger, saya kira itu hanya masalah preferensi, mau dipasang silakan, tidak pun tidak masalah. Sedangkan untuk web-web besar, bisa jadi itu diperlukan.

</div><div>**Jadi, orang lain pun bisa mengakses sitemap kita hanya dengan menambahkan sufiks “sitemap.xml” di domain kita?**ya.

</div><div>**Apakah itu menjadi masalah?**sejauh ini tidak.

</div><div>**Bagaimana bila kita submit sitemap web orang lain ke GSC kita?**pertama, *rek nanaonan ari maneh?* Kedua, manfaatkan manfaat, kita TIDAK BISA submit sitemap milik web lain.

</div></div>- - - - - -

Oke, cukup ngobrol-ngobrol kita tentang cara membuat *peta situs* di Blogger dan WordPress. Semoga membantu dan sampai jumpa di artikel selanjutnya. **(eL/Foto: eL)**

</div><span><svg aria-hidden="true" height="1em" role="img" viewbox="0 0 640 512" width="1em" xmlns="http://www.w3.org/2000/svg"><path d="M497.941 225.941L286.059 14.059A48 48 0 0 0 252.118 0H48C21.49 0 0 21.49 0 48v204.118a48 48 0 0 0 14.059 33.941l211.882 211.882c18.744 18.745 49.136 18.746 67.882 0l204.118-204.118c18.745-18.745 18.745-49.137 0-67.882zM112 160c-26.51 0-48-21.49-48-48s21.49-48 48-48 48 21.49 48 48-21.49 48-48 48zm513.941 133.823L421.823 497.941c-18.745 18.745-49.137 18.745-67.882 0l-.36-.36L527.64 323.522c16.999-16.999 26.36-39.6 26.36-63.64s-9.362-46.641-26.36-63.64L331.397 0h48.721a48 48 0 0 1 33.941 14.059l211.882 211.882c18.745 18.745 18.745 49.137 0 67.882z" fill="currentColor"></path></svg></span><span><span>Google Search Console</span> <span>Peta Situs</span> <span>Alat Webmaster</span></span>

</div>