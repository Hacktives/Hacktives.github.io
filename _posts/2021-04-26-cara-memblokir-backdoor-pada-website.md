---
id: 198
title: 'Cara Memblokir Backdoor Pada Website'
date: '2021-04-26T01:31:00+00:00'
author: admin
layout: post
guid: 'http://localhost/wordpress/index.php/2021/04/26/cara-memblokir-backdoor-pada-website/'
permalink: /index.php/2021/04/26/cara-memblokir-backdoor-pada-website/
blogger_blog:
    - webidevloper.blogspot.com
blogger_author:
    - IDEV.My.ID
blogger_permalink:
    - /2021/04/cara-memblokir-backdoor-pada-website.html
blogger_internal:
    - /feeds/2636143461486592706/posts/default/5315230029131063589
categories:
    - CyberSecurity
---

<div style="clear: both; text-align: center;">[<span style="font-family: Fira Sans; font-size: medium;">![](https://1.bp.blogspot.com/-dNBcJfaTTLY/YIYFVYj3r0I/AAAAAAAAA4I/CnyIMo2iFJgZSJ6UZp_Mj5UmrR4viDHRACLcBGAsYHQ/w640-h430/idev.jpeg)</span>](https://1.bp.blogspot.com/-dNBcJfaTTLY/YIYFVYj3r0I/AAAAAAAAA4I/CnyIMo2iFJgZSJ6UZp_Mj5UmrR4viDHRACLcBGAsYHQ/s520/idev.jpeg)</div><span style="font-family: Fira Sans; font-size: medium;">  
</span>

<span style="font-family: Fira Sans; font-size: medium;"><span>**Halo**</span> sahabat Developer, Apa kabar? Baru baru ini saya sering sekali melihat website berjatuhan karena serangan *Peretas* atau Defacer Sebenarnya ada banyak sekali cara untuk mencegah si Hacker menyisipkan backdoor pada *Uploader,* Tetapi banyak juga yang kecolongan atas ulah si peretas yang masuk menggunakan <u>Backdoor</u>.</span>

<span style="font-family: Fira Sans; font-size: medium;">Apakah cara ini ampuh? Menurut saya ya ampuh sekali untuk mencegahnya dari pihak ketiga mengencripsikan file file berbahaya seperti Backdoor atau Shell.</span>

**<span style="font-family: Fira Sans; font-size: medium;">  
</span>**

<span style="font-family: Fira Sans; font-size: medium;">**Backdoor** sesuai namanya yaitu *Pintu Belakang*, Fungsi Backdoor ini biasanya untuk mengubah ubah file didalam atau menambahkannya dengan sesuka hati si Hacker, *Dengan* *Backdoor* ini Hacker/Peretas dapat leluasa loncat kesana kemari dari domain satu ke domain lain atau dari domain subdo ke domain utama, banyak sekali fungsi *Backdoor* ini seperti Mengcrack WordPress, Crack Database, Memasukan Adminer, Mengubah file atau halaman demi halaman tampilan pada website, Mengupload file dll.</span>

<span style="font-family: Fira Sans; font-size: medium;">Bahkan fitur si Peretas ini lebih leluasa dibanding si Owner atau pembuat Website tersebut.</span>

<span style="font-family: Fira Sans; font-size: medium;">Bagaimana bisa si Peretas *mengencripsikan* code backdoor kedalam Website kalian? Biasanya si Hacker/peretas ini mengupload sebuah File Backdoor dari suatu uploader seperti Upload image, File Drag n Drop.</span>

**<span style="font-family: Fira Sans; font-size: medium;">  
</span>**

<span style="font-family: Fira Sans; font-size: medium;">**Tahu gak sih** bahwa si Peretas bisa Mengupload File php ke sebuah *uploader*, Yaa saya lihat banyak sekali yang menggunakan cara seperti ini Cara ini biasanya dinamakan *<span>Bypass Extension Shell</span>*</span>

<span style="font-family: Fira Sans; font-size: medium;">  
</span>

<span style="font-family: Fira Sans; font-size: medium;"></span>

<div style="-moz-border-radius: 10px; -webkit-border-radius: 10px; background-color: #f3f3f3; border-left: 5px solid gray; border-radius: 10px; padding: 10px; t-align: left;">Baca Juga..  
[ Peradaban Hacker Defacer di Indonesia](https://www.idev.my.id/2021/04/peradaban-hacker-defacer-di-indonesia.html)</div><span style="font-family: Fira Sans; font-size: medium;">  
</span>

<span style="font-family: Fira Sans; font-size: medium;">Ada berbagai cara untuk *Bypas Extension* Shell ini, dengan mengubah extensi si file atau shell tersebut sudah mempunyai fitur Bypassnya tersendiri, ada juga yang Mengbypass dengan Browser Firefox yang sudah mempunyai fitur tersebut.</span>

<div style="clear: both; text-align: center;">[<span style="font-family: Fira Sans; font-size: medium;">![](https://1.bp.blogspot.com/-0jPtZTAn5Pg/YIYKpzKdFKI/AAAAAAAAA4Q/a0qtpQadiaQnxc1HJv32ZDJOSNZxhJnBwCLcBGAsYHQ/w640-h426/images%2B%252837%2529.jpeg)</span>](https://1.bp.blogspot.com/-0jPtZTAn5Pg/YIYKpzKdFKI/AAAAAAAAA4Q/a0qtpQadiaQnxc1HJv32ZDJOSNZxhJnBwCLcBGAsYHQ/s626/images%2B%252837%2529.jpeg)</div><span style="font-family: Fira Sans; font-size: medium;">  
</span>

<u><span style="font-family: Fira Sans; font-size: medium;">Bisa saja Situs web kamu sudah *tertanam* Backdoor..</span></u>

<span style="font-family: Fira Sans; font-size: medium;">Nah bagaimana cara mencegah hal yang tidak di inginkan tersebut?</span>

<span style="font-family: Fira Sans; font-size: medium;">Nah saya punya Code untuk ditambahkan .**<span>htaccess</span>** kalian Berikut Source Codenya:</span>

<span style="font-family: Fira Sans; font-size: medium;">  
</span>

> <span style="font-family: Fira Sans; font-size: medium;">*&lt;FilesMatch “.(py|exe|php)$”&gt;*</span>
> 
> <span style="font-family: Fira Sans; font-size: medium;"> *Order allow,deny*</span>
> 
> <span style="font-family: Fira Sans; font-size: medium;"> *Deny from all*</span>
> 
> <span style="font-family: Fira Sans; font-size: medium;">*&lt;/FilesMatch&gt;*</span>
> 
> <span style="font-family: Fira Sans; font-size: medium;">*&lt;FilesMatch “^(about.php|login.php|index.php|content.php|newnamefile.php)$”&gt;*</span>
> 
> <span style="font-family: Fira Sans; font-size: medium;"> *Order allow,deny*</span>
> 
> <span style="font-family: Fira Sans; font-size: medium;"> *Allow from all*</span>
> 
> <span style="font-family: Fira Sans; font-size: medium;">*&lt;/FilesMatch&gt;*</span>
> 
> <span style="font-family: Fira Sans; font-size: medium;">*&lt;IfModule mod\_rewrite.c&gt;*</span>
> 
> <span style="font-family: Fira Sans; font-size: medium;">*RewriteEngine On*</span>
> 
> <span style="font-family: Fira Sans; font-size: medium;">*RewriteBase /*</span>
> 
> <span style="font-family: Fira Sans; font-size: medium;">*RewriteRule ^index.php$ – \[L\]*</span>
> 
> <span style="font-family: Fira Sans; font-size: medium;">*RewriteCond %{REQUEST\_FILENAME} !-f*</span>
> 
> <span style="font-family: Fira Sans; font-size: medium;">*RewriteCond %{REQUEST\_FILENAME} !-d*</span>
> 
> <span style="font-family: Fira Sans; font-size: medium;">*RewriteRule . /index.php \[L\]*</span>
> 
> <span style="font-family: Fira Sans; font-size: medium;">*&lt;/IfModule&gt;*</span>

<span style="font-family: Fira Sans; font-size: medium;"> </span>

<span style="font-family: Fira Sans; font-size: medium;">Jika terjadi eror pada sebuah file, Kamu hanya menambahkan Nama Ekstensi file tersebut di bagian</span>

<span style="font-family: Fira Sans; font-size: medium;"> \[ *&lt;FilesMatch “^(tambahkan nama file disini untuk di izinkan tampil)$”&gt;* \]</span>

**<span style="font-family: Fira Sans; font-size: medium;">  
</span>**

<span style="font-family: Fira Sans; font-size: medium;"><span>**Fungsi code .***htaccess*</span> <span>tersebut untuk memblokir file file yang masuk dari sebuah uploader yang tidak di izinkan, Bisa saja si peretas sudah menaruh Backdoor tersebut sejak lama di dalam web kamu!</span></span>

<span style="font-family: Fira Sans; font-size: medium;">Nah cara yang paling *Tepat* adalah menambahkan Code tersebut kedalam file<span> .</span><span>**htaccess**</span></span>

<span style="font-family: Fira Sans; font-size: medium;">  
</span>

<span style="font-family: Fira Sans; font-size: medium;">Cara diatas bisa kalian lakukan saat website kalian terenkripsi backdoor, nah untuk memblokirnya sementara kalian menggunakan code diatas tersebut jika sudah menemukan backdoor tersebut jangan lupa dihapus dan ubah httacces seperti semula untuk mencegah terjadinya eror pada halaman web anda.</span>

<span style="font-family: Fira Sans; font-size: medium;">Terimakasih sudah membaca sampai sini..</span>

<div>https://www.idev.my.id/feeds/posts/default</div>