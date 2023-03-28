---
id: 127
title: '4 Cara Memperbaiki Error Breadcrumb Pada Blogger'
date: '2022-11-24T12:00:00+00:00'
author: admin
layout: post
guid: 'http://localhost/wordpress/index.php/2022/11/24/4-cara-memperbaiki-error-breadcrumb-pada-blogger/'
permalink: /index.php/2022/11/24/4-cara-memperbaiki-error-breadcrumb-pada-blogger/
blogger_blog:
    - webidevloper.blogspot.com
blogger_author:
    - IDEV.My.ID
blogger_internal:
    - /feeds/2636143461486592706/posts/default/1959338086541875075
categories:
    - Uncategorized
---

Hi Sobat idev.my.id kali ini aku mau bahas 4 Cara Memperbaiki Error Breadcrumb Pada Blogger

<div>**4 Cara Memperbaiki Error Breadcrumb Pada Blogger** – Setelah sekian lama tidak aktif dalam menjalankan aktivitas blogging, dan mulai kembali menerbitkan artikel baru. Admin sedikit terkejut, karena dalam hasil pelaporan coverage indexes google search console ternyata banyak sekali error yang ditemukan oleh google dalam situs yang admin kelola. Salah satunya kesalahan remah roti.

<div style="clear: both; text-align: center;">[![4 Cara Memperbaiki Error Breadcrumb Pada Blogger](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEiyDkayZRTi63nbgbQAD-XaMzQPmon91g78YzR65NQfAGQPjayhEP7aua7pdp-zyDh-lLSjDfceS7ewt3H0saMeJ7NOCBfb-AyNyvHy3cAKk-1Z82aQq5A7CBY1G7lVUMND7uF_oPRJeIg0rG4rfsA4CdoSw8rcFONpkSytLveejC2F2ZsyxMmH5UGSgQ/w640-h306/4-cara-memperbaiki-error-breadcrumb-pada-blogger-paling-lengkap.png "4 Cara Memperbaiki Error Breadcrumb Pada Blogger")](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEiyDkayZRTi63nbgbQAD-XaMzQPmon91g78YzR65NQfAGQPjayhEP7aua7pdp-zyDh-lLSjDfceS7ewt3H0saMeJ7NOCBfb-AyNyvHy3cAKk-1Z82aQq5A7CBY1G7lVUMND7uF_oPRJeIg0rG4rfsA4CdoSw8rcFONpkSytLveejC2F2ZsyxMmH5UGSgQ/s600/4-cara-memperbaiki-error-breadcrumb-pada-blogger-paling-lengkap.png)</div><div><div style="text-align: justify;"></div><div style="text-align: justify;"> **Daftar Isi**<span><label></label></span> </div></div>Karena pihak google member pelapak ini, tentu saja sebagai seorang blogger yang bertanggung jawab penuh terhadap situs yang dikelola. Admin langsung saja mengecek masalahnya dimana. Sebab jika sudah masuk ke tenaga kerja sudah pasti ini berkaitan erat dengan SEO website, jika dibiarkan berlarut-larut tentu juga akan memberikan danfak buruk terhadap kesehatan serta kinerja blog. Terutama masalah kepercayaan mesin pencari.

Supaya teman-teman tidak bingung, dan sedikit mengerti tentang apa itu breadcrumb. Dan mengapa pihak google memberikan tenaga kerja khusus terkait masalah ini. Silakan lihat definisi dan fungsinya di bawah ini.

### Apa itu remah roti

Breadcrumbs adalah salah satu elemen pada website yang memiliki fungsi sebagai navigasi halaman, yang berbentuk seperti teks kecil berisi link halaman website. Breadcrumbs juga bisa dianggap sebagai navigasi sekunder dalam website, karena breadcrumbs menunjukan urutan struktur halaman-halaman yang sudah dibuka oleh pengunjung website. Dengan adanya breadcrumbs bisa membantu para pengunjung agar tidak perlu repot-repot apabila ingin kembali ke halaman awal.

### Fungsi breadcrumb

Seperti yang telah kami jelaskan dalam pengertian breadcrumb di atas, fungsi utama dari breadcrumb adalah sebagai navigasi tambahan, yang memudahkan pembaca untuk mengakses artikel atau konten serupa tampa perlu melakukan pencarian atau kembali kehalaman awal lagi.

Jika sobat juga menemukan error terkait dengan remah roti maka solusinya kalian bisa melakukan beberapa langkah di bawah ini.

### Cara Mengatasi Error Breadcrumb Khusus Blogger

Untuk kalian yang saat ini mencari panduan cara memperbaiki error breadcrumb dengan masalah “data-vocabulary.org schema deprecated”, silakan gunakan salah satu cara yang kami sajikan di bawah ini untuk mengatasinya.

#### Ganti data-vocabulary.org dengan schema.org

Caranya gampang, kalian hanya perlu mengakses menu template &gt;&gt;&gt; Edit HTML &gt;&gt;&gt; cari kode “data-vocabulary.org”, jika sudah ketemu hapus semua yang ada dan ganti dengan schema.org. Lalu Klik simpan template.

#### Ganti Scrip Breadcrumb Lama Dengan Yang Baru

Untuk kawan-kawan yang selama ini menggunakan template yang sudah terpasang remah roti, kemungkinan besar akan mendapatkan laporan error dalam cakupan indeksnya dari Google. Berikut car mengatasinya.

**Cara Pertama #Ganti Script Breadcrumb**

1\. Klik Tema &gt; Edit HTML

2\. Carry code seperti di bawah ini:

<div><a expr:href=" itemprop='url' title=" home=""><span itemprop="title">Rumah</span></a>

<loop values="data:post. labels" var="label"> »</loop>

<span expr:title="data:label.name" itemprop="url" itemscope="" itemtype=" expr:href="><span itemprop="title "><label.name></label.name></span></span>

 » <span><post.title></post.title></span>

</div>Jika sudah ketemu, hapus lalu ganti dengan kode berikut:

<div style="text-align: justify;"> <textarea rows="7" width="100%"><div>Rumah  
<loop values="data:post.labels" var="label"> »  
<label.name></label.name>  
</loop> » <span><post.title></post.title></span>

</div></textarea>  
<button data-clipboard-target="#bc1">Klik untuk Menyalin</button></div>Untuk memastikan tidak terjadi kesalahan, silakan klik preview. Lalu Simpan.

**Cara Kedua # Ganti Kode Breadcrumbs Lama Untuk Atasi Error**

Masuk ke dashboard Blogger

Klik menu Tema &gt;&gt; Edit HTML

Cari &amp; temukan kode berikut <includable var="posts"> dengan cara tekan tombol Ctrl+F pada keyboard kalian.</includable>

Pastekan kode berikut ini tepat di bawah <includable var="posts">, jika pada tema yang kalian gunakan sudah ada kode yang agak mirip dengan script di bawah ini. Maka hapus kode lama yang ada mulai dari <includable> sampai</includable>.</includable>

Berikut script breadcrumbs barunya.

<div style="text-align: justify;"> <textarea rows="30" width="100%"><includable>  
<if cond="data:view.isPost">  
 <loop values="data:posts" var="post"><div itemscope="itemscope" itemtype="https://schema.org/BreadcrumbList"> <span itemprop="itemListElement" itemscope="itemscope" itemtype="https://schema.org/ListItem"> <span itemprop="name"><switch var="data:blog.locale"><case value="id"></case>Beranda<default></default>Rumah</switch></span>

 <if cond="data:post.labels">  
 <loop index="nomor" values="data:post.labels" var="label"> ›   
 <span itemprop="itemListElement" itemscope="itemscope" itemtype="https://schema.org/ListItem"></span></loop></if>

 <span itemprop="name"><label.name></label.name></span>

</span>  
 <else></else> › <span itemprop="name"><blog.pagename></blog.pagename></span>  
   
   
   
<elseif cond="data:view.isPage"></elseif>

<div itemscope="itemscope" itemtype="https://schema.org/BreadcrumbList"> <span itemprop="itemListElement" itemscope="itemscope" itemtype="https://schema.org/ListItem"> <span itemprop="name"><switch var="data:blog.locale"><case value="id"></case>Beranda<default></default>Rumah</switch></span>  
 ›   
 <span itemprop="itemListElement" itemscope="itemscope" itemtype="https://schema.org/ListItem"></span>

 <span itemprop="name"><blog.pagename></blog.pagename></span>

</span>  
</div></div><button data-clipboard-target="#bc2">Klik untuk Menyalin</button>

</loop>#### Pasang Breadcrumb

Kalau thema yang kalian pakai belum ada fitur breadcrumb, tapi terdeteksi error “data-vocabulary.org schema deprecated”, di google search console. Maka solusinya kawan-kawan tinggal pasang kode breadcrumb di dalam tempalate yang sedang digunakan saat ini. adapun caranya adalah sebagai berikut.

1\. Klik Tema &gt; Edit HTML

2\. Cari kode skin&gt;dengan cara klik dulu di sembarang tempat di dalam area kode template, lalu tekan CTRL + F , masukkan skin&gt; pada kotak kecil yang tersedia. Jika sudah jika sudah ketemu, silakan pastekan kode dibawah ini tepat di atasnya.

<div> <textarea rows="11" width="100%">.breadcrumbsline-height:1.2em;width:auto;overflow:hidden;padding:0;margin:0 auto 20px;font-size:90%;color:#888;font-weight:400;text-overflow: elipsis;-webkit-text-overflow:ellipsis;white-space:nowrap .breadcrumbs adisplay:inline-block;text-decoration:none;transition:all .3s ease-in-out;color:#777;font -weight:400 .breadcrumbs a:hovercolor:blue .breadcrumbs svgwidth:20px;height:20px;vertical-align:-5px;margin:0 -3px .breadcrumbs jalur svgfill:#c8c8c8  
</textarea>  
<button data-clipboard-target="#bc3">Klik untuk Menyalin</button></div>3\. Lanjutkan kode temukan <includable var="posts"> … </includable>

4\. Hapus dan ganti dengan kode breadcrumb tanpa error terbaru di bawah ini:

<div> <textarea rows="30" width="100%"><includable var="posts">  
<if cond="data:view.isSingleItem">  
<loop values="data:posts" var="post">  
<if cond="data:post.labels"><div itemscope="itemscope" itemtype="https://schema.org/BreadcrumbList"><span itemprop="itemListElement" itemscope="itemscope" itemtype="https://schema.org/ListItem"><span itemprop="name">Rumah</span>

<svg viewbox="0 0 24 24"><path d="M8.59,16.58L13.17,12L8.59,7.41L10,6L16,12L10,18L8.59,16.58Z"></path></svg>  
<loop index="num" values="data:post.labels" var="label">  
<span itemprop="itemListElement" itemscope="itemscope" itemtype="https://schema.org/ListItem"></span></loop>

<span itemprop="name"><label.name></label.name></span>

<svg viewbox="0 0 24 24"><path d="M8.59,16.58L13.17,12L8.59,7.41L10,6L16,12L10,18L8.59,16.58Z"></path></svg>

</span>  
<span><post.title></post.title></span>  
  
</div></if>  
</loop>  
</if>  
<button data-clipboard-target="#bc4">Klik untuk Menyalin</button>  
</includable>5\. Save untuk menyimpan perubahan template.

#### Gunakan Template Versi Terbaru

Selain dengan menggunakan tiga cara di atas, kawan-kawan juga dapat dengan mudah mengatasi semua masalah error terkait dengan breadcrumb dengan cara menganti tema lama dengan template seo terbaru. Kalian bisa menggunakan template gratis maupun template berbayar.

Namun sebelum kalian memutuskan untuk menggunakan template tersebut, sebaiknya kalian pastikan kalau temanya sudah di optimasi dengan baik. Jangan sampai setelah ganti template traffik anjlok. Dan amankan kode penting sebelum kalian mengantinya.

Selain mengamankan beberapa kode penting yang sudah terpasang di tema lama, kalian juga harus menghidari beberapa hal yang kemungkinan besar akan memberikan pengaruh buruk untuk situs kawan-kawan kedepannya.

Untuk mengatasi masalah ini silakan kawan-kawan baca tips memilih tema blogspot dan bagaimana cara menganti template blogspot yang baik dan benar yang sudah kami sajikan sebelumnya.

### Remah roti kue 

Setelah menerapkan kode yang telah kami bagikan ke dalam template yang sedang kalian pakai saat ini, kalian wajib untuk mengecek apakah breadcrumb di situs kawan-kawan masih error atau tidak. Berikut langkah-langkah mengecek error breadcrumb menggunakan google webmaster tools.

#### Bagaimana Cara Cek Breadcrumb Errors atau Tidak

Akses google search console yang terkait dengan situs yang sedang kawan-kawan perbaiki.

Masuk menu url inspection &gt;&gt;&gt; pastekan url lengkap salah satu postingan kalian yang terdapat gambarnya, di dalam kotak yang tersedia &gt;&gt;&gt; enter.

Klik Live Test, jika masalah breadcrumbnya sudah diperbaiki. Maka kalian akan melihat karya yang kurang lebih seperti gambar di bawah ini.

<div style="clear: both; text-align: center;">[![Bagaimana Cara Cek Breadcrumb Errors atau Tidak](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEjA6vp4ZyN1FnSVLRoHBk3VvU0zswYXt84ii1RIwu8w8iBTMkt_zZ2pWUqGPnaqHybOLgkuV-MokYO-XaF6ZW1K35dMm7Fc2VwWh6Fsu4TVLVUaO-l_h0Ygoqm-w_1q1f3OFIlFQXrZP86nM6VpZNdNweYV3L_um0ETXqxhsHCyFVOr0e1kQJD0nEKLSw/w640-h404/hasil-test-breadcrumb-valid-tidak-errors.png "Bagaimana Cara Cek Breadcrumb Errors atau Tidak")](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEjA6vp4ZyN1FnSVLRoHBk3VvU0zswYXt84ii1RIwu8w8iBTMkt_zZ2pWUqGPnaqHybOLgkuV-MokYO-XaF6ZW1K35dMm7Fc2VwWh6Fsu4TVLVUaO-l_h0Ygoqm-w_1q1f3OFIlFQXrZP86nM6VpZNdNweYV3L_um0ETXqxhsHCyFVOr0e1kQJD0nEKLSw/s600/hasil-test-breadcrumb-valid-tidak-errors.png)</div>### Melakukan Validasi Perbaikan Breadcrumb

Jika kawan-kawan sudah menerapkan beberapa perubahan, menggunakan tips yang kami bagikan di atas, dan sudah dipastikan kalau sudah tidak terdeteksi masalah lagi. Supaya kesalahan cakupan indexes di google search console terkait breadcrumb segera teratasi. Maka silakan lakukan validasi perbaikan breadcrumb melalui Google Search Console.

#### Cara Melakukan Validasi Perbaikan Breadcrumb

Akses google search console &gt;&gt;&gt; Breadcrumbs &gt;&gt;&gt; klik “data-vocabulary.org schema deprecated” &gt;&gt;&gt; VALIDATE FIX

<div style="clear: both; text-align: center;">[![Cara Melakukan Validasi Perbaikan Breadcrumb](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEjL0XEQJRQBi9rIToTKCjxKMhNkUWk6l5BbhwsbyOKIJMSwFMi-IYdBqmRufXIzbfuIryqMBKmOFh449JAr6JdDoyh1Gat0ESt7v-RwGleJuD_uXKnjahwIF-a1cX4KwCgJO-VZ0ZZfSd6vXp7I_u2OkD3BUlCcSYP5j3Gu57m9NATTMkcVhTdU05flVw/w640-h134/cara-validasi-perbaikan-errors-breadcrumb-blogger.png "Cara Melakukan Validasi Perbaikan Breadcrumb")](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEjL0XEQJRQBi9rIToTKCjxKMhNkUWk6l5BbhwsbyOKIJMSwFMi-IYdBqmRufXIzbfuIryqMBKmOFh449JAr6JdDoyh1Gat0ESt7v-RwGleJuD_uXKnjahwIF-a1cX4KwCgJO-VZ0ZZfSd6vXp7I_u2OkD3BUlCcSYP5j3Gu57m9NATTMkcVhTdU05flVw/s600/cara-validasi-perbaikan-errors-breadcrumb-blogger.png)</div>Setelah melakukan semua langkah di atas, yang perlu teman-teman lakukan adalah menunggu Google melakukan validasi perbaikan error breadcrumb. Kamu bisa memantau progressnya dengan cara klik SEE DETAIL. Mengenai kapan akan selesai, tergantung dari banyaknya jumlah postingan yang ada di situs.

### penutup

Masalah error breadcrumb dengan laboran yang isinya “data-vocabulary.org schema deprecated”, di google search console dapat di atasi dengan mudah menggukan 4 cara. Diantaranya adala sebagai berikut. 1) Ganti kode “data-vocabulary.org” dengan “schema.org”, 2) Ganti kode breadcrumb yang ada dengan yang baru, 3) Pasang kode breadcrumb, dan 4) Gunakan template versi terbaru.

Demikianlah artikel singkat yang bisa kami sampaikan mengenai **4 Cara Memperbaiki Error Breadcrumb Pada Blogger**, yang bisa sahabat coba praktekkan. Semoga ada salah satu tips di atas yang bisa berguna, terima kasih.

</textarea>  
Gimana sibat idev.my.id semoga pembahasan 4 Cara Memperbaiki Error Breadcrumb Pada Blogger semoha bisa bermanfaat ya jangan lupa kunjungi lagi web kami di idev.my.id

</div></if></includable></textarea></div></div>