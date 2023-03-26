---
title: 'Cara Mudah Konfigurasi DNS Blogspot dengan Chname dan A Record di Cloudflare'
date: 2023-02-16T18:41:00.010-08:00
draft: false
url: /2023/02/Cara-Mudah-Konfigurasi-DNS-Blogspot-dengan-Chname-dan-A-Record-di-Cloudflare.html
tags: 
- BLOG
- DNS
- BLOGSPOT
- CLOUDFLARE
- BLOGGER
- DOMAIN
- WORDPRESS
- OPTIMATION
- CDN
---

[![cara seting cloudflare di wordpress dan blogger.webp](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEjpGPbOoBSvAMjAzU7Rr958hjWDJ22m9NqqPi3KO6zWf4t8dsAC8PnZq9JLxlU8e278xdXu7P77lj5ehoE7rxyLXYFRJdzV2RsXoUrB57A7YxlzR_SMvN9vn_9oNgpJ3NGeO72j3eB84BmzNOhksslu-wg3lC6on2ej5Ld87AzINv2VNO3D5X4IOZA-tQ/w640-h336/cara%20seting%20cloudflare%20di%20wordpress%20dan%20blogger.webp)](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEjpGPbOoBSvAMjAzU7Rr958hjWDJ22m9NqqPi3KO6zWf4t8dsAC8PnZq9JLxlU8e278xdXu7P77lj5ehoE7rxyLXYFRJdzV2RsXoUrB57A7YxlzR_SMvN9vn_9oNgpJ3NGeO72j3eB84BmzNOhksslu-wg3lC6on2ej5Ld87AzINv2VNO3D5X4IOZA-tQ/s1200/cara%20seting%20cloudflare%20di%20wordpress%20dan%20blogger.webp)

Mempunyai blog di platform blogspot tentunya memerlukan konfigurasi DNS agar blog dapat diakses dengan mudah oleh pengunjung. Salah satu cara untuk melakukan konfigurasi DNS adalah dengan menggunakan layanan Cloudflare yang terkenal dengan kemampuan caching dan proteksi terhadap serangan DDoS.

  

Dalam artikel ini, kami akan memberikan panduan langkah-demi-langkah tentang bagaimana cara melakukan konfigurasi DNS untuk blogspot menggunakan Chname dan A Record di Cloudflare.

  

Mendaftarkan domain pada Cloudflare

Langkah pertama yang perlu dilakukan adalah mendaftarkan domain pada Cloudflare. Pastikan bahwa domain yang ingin didaftarkan telah Anda miliki dan Anda memiliki akses ke panel kontrol DNS.

  

Setelah Anda mendaftarkan domain pada Cloudflare, sistem akan melakukan scan pada DNS dan menampilkan catatan DNS yang terkait dengan domain yang telah didaftarkan.

  

Mengubah Chname dan A Record

Setelah domain berhasil didaftarkan pada Cloudflare, langkah selanjutnya adalah mengubah Chname dan A Record. Chname diperlukan untuk mengarahkan domain ke subdomain blogspot, sedangkan A Record digunakan untuk menunjukkan alamat IP dari blogspot.

  

Pertama-tama, ubah catatan Chname. Anda dapat melakukan ini dengan mengklik tanda panah pada baris catatan tersebut dan mengubah nilai pada kolom 'Name' menjadi '@' dan nilai pada kolom 'Target' menjadi 'ghs.google.com'. Setelah itu, simpan perubahan yang telah dilakukan.

  

Kedua, ubah catatan A Record. Anda dapat melakukan ini dengan menambahkan catatan baru dengan mengeklik tombol 'Add Record' dan memilih jenis catatan 'A'. Masukkan nilai IP dari blogspot pada kolom 'IPv4 Address', kemudian simpan perubahan yang telah dilakukan.

  

Menunggu DNS Propagation

Setelah semua konfigurasi DNS selesai dilakukan, Anda harus menunggu hingga DNS Propagation selesai. Proses ini memerlukan waktu beberapa jam hingga maksimal 24 jam tergantung dari penyedia layanan DNS yang digunakan.

  

Setelah proses DNS Propagation selesai, blogspot Anda akan dapat diakses melalui domain yang telah didaftarkan dan dikonfigurasi pada Cloudflare.

  

Penutup

  

Itulah cara mudah melakukan konfigurasi DNS untuk blogspot menggunakan Chname dan A Record pada layanan Cloudflare. Dengan melakukan konfigurasi DNS pada blogspot, pengunjung dapat dengan mudah mengakses blog Anda tanpa perlu mengingat alamat IP atau alamat blogspot yang cukup panjang.

  

Jangan lupa untuk selalu melakukan backup catatan DNS sebelum melakukan perubahan pada konfigurasi DNS. Jika ada masalah atau pertanyaan, jangan ragu untuk menghubungi tim support dari Cloudflare. Semoga artikel ini bermanfaat bagi Anda yang ingin mengoptimalkan blogspot Anda.

https://www.idev.my.id/feeds/posts/default