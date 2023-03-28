---
id: 194
title: 'Cara mengatasi This PC Can’t Run Windows 11'
date: '2021-06-25T01:00:00+00:00'
author: admin
layout: post
guid: 'http://localhost/wordpress/index.php/2021/06/25/cara-mengatasi-this-pc-cant-run-windows-11/'
permalink: /index.php/2021/06/25/cara-mengatasi-this-pc-cant-run-windows-11/
blogger_blog:
    - webidevloper.blogspot.com
blogger_author:
    - IDEV.My.ID
blogger_internal:
    - /feeds/2636143461486592706/posts/default/7123182542692951525
categories:
    - Windows
---

<div style="clear: both; text-align: center;">[![](https://1.bp.blogspot.com/-pMiKYYZyyxw/YNUpvQJ95yI/AAAAAAAABds/nTuZ0CWr6QEW0kwG8xnsqcxDFWTeqc4-ACLcBGAsYHQ/w640-h360/maxresdefault.jpg)](https://1.bp.blogspot.com/-pMiKYYZyyxw/YNUpvQJ95yI/AAAAAAAABds/nTuZ0CWr6QEW0kwG8xnsqcxDFWTeqc4-ACLcBGAsYHQ/s1280/maxresdefault.jpg)</div><span style="color: #222222; font-family: "Open Sans", serif; font-size: 16px; vertical-align: inherit;"><span style="vertical-align: inherit;">Jika Anda telah </span></span>[<span style="vertical-align: inherit;"><span style="vertical-align: inherit;">menjalankan Microsoft’s PC Health Check</span></span>](https://www.idev.my.id/2021/06/windows-11-sudah-rilis-download.html)<span style="color: #222222; font-family: "Open Sans", serif; font-size: 16px; vertical-align: inherit;"><span style="vertical-align: inherit;"> dan menerima pesan “This PC Can’t Run Windows 11”, ada kemungkinan Anda perlu mengaktifkan TPM dan Secure Boot di PC Anda. </span><span style="vertical-align: inherit;">Begini caranya.</span></span>

## <span style="vertical-align: inherit;"><span style="vertical-align: inherit;">Windows 11 Membutuhkan TPM 2.0 dan Boot Aman</span></span>

<span style="vertical-align: inherit;"><span style="vertical-align: inherit;">Untuk beberapa PC, akar masalah dengan Pemeriksaan Kesehatan PC adalah Boot Aman dan TPM dinonaktifkan di </span></span>[<span style="vertical-align: inherit;"><span style="vertical-align: inherit;">UEFI</span></span>](https://www.howtogeek.com/56958/htg-explains-how-uefi-will-replace-the-bios/)<span style="vertical-align: inherit;"><span style="vertical-align: inherit;"> , yang merupakan sistem dasar yang memungkinkan sistem operasi Anda bekerja dengan perangkat keras PC Anda. </span><span style="vertical-align: inherit;">Banyak orang masih menyebut UEFI sebagai “BIOS”, meskipun istilah itu secara teknis mengacu pada standar yang lebih lama.</span></span>

<span style="vertical-align: inherit;"><span style="vertical-align: inherit;">Setelah mengaktifkan TPM dan Secure Boot, kemungkinan PC Anda akan lulus pemeriksaan kompatibilitas Windows 11 jika memenuhi semua </span></span>[<span style="vertical-align: inherit;"><span style="vertical-align: inherit;">persyaratan sistem lainnya</span></span>](https://www.howtogeek.com/737029/what-are-the-minimum-system-requirements-to-run-windows-11/)<span style="vertical-align: inherit;"><span style="vertical-align: inherit;"> .</span></span>

<span style="vertical-align: inherit;"><span style="vertical-align: inherit;">  
</span></span>

## <span style="vertical-align: inherit;"><span style="vertical-align: inherit;">Cara Mengaktifkan TPM dan Boot Aman di UEFI</span></span>

<span style="vertical-align: inherit;"><span style="vertical-align: inherit;">Untuk mengaktifkan TPM dan Secure Boot di UEFI Anda, pertama-tama Anda harus mematikan perangkat Anda. </span><span style="vertical-align: inherit;">Saat Anda menyalakannya kembali, akan ada tombol atau tombol keyboard khusus yang harus Anda tekan pada waktu yang tepat untuk </span></span>[<span style="vertical-align: inherit;"><span style="vertical-align: inherit;">masuk ke pengaturan UEFI Anda</span></span>](https://www.idev.my.id/2021/06/windows-11-sudah-rilis-download.html)<span style="vertical-align: inherit;"><span style="vertical-align: inherit;"> .</span></span>

<span style="vertical-align: inherit;">Kunci persis yang harus Anda tekan bervariasi tergantung pada pabrikannya, jadi Anda harus berkonsultasi dengan manual pengoperasian perangkat Anda atau melakukan pencarian web untuk nama perangkat Anda bersama dengan “kunci bios” atau “kunci UEFI.” </span><span style="vertical-align: inherit;">Untuk beberapa motherboard (terutama jika Anda membuat PC sendiri), Anda mungkin melihat pesan kecil di layar saat boot yang memberi tahu Anda tombol mana yang perlu Anda tekan untuk masuk ke pengaturan BIOS.</span>

<span style="vertical-align: inherit;"><span style="vertical-align: inherit;">Misalnya, pada laptop Acer Spin 3 yang kami miliki, Anda mengakses menu konfigurasi UEFI dengan menyalakan laptop dan menekan F2 pada keyboard ketika Anda melihat layar splash “Acer”.</span></span>

<span style="vertical-align: inherit;"><span style="vertical-align: inherit;">Setelah Anda berada di layar pengaturan UEFI Anda, instruksi juga akan bervariasi secara dramatis tentang cara mengaktifkan Boot Aman dan TPM, tetapi secara umum, Anda mencari opsi “Keamanan” atau “Boot”.</span></span>

<span style="vertical-align: inherit;">Dalam contoh ini Setup Utility oleh American Megatrends (pengaturan Anda kemungkinan akan terlihat berbeda), Anda dapat menemukan opsi TPM di bawah tab “Keamanan”. </span><span style="vertical-align: inherit;">Cari “TPM” dan pastikan itu diaktifkan. </span><span style="vertical-align: inherit;">Jika tidak, ubah pengaturan di UEFI khusus Anda untuk mengaktifkannya.</span>

<figure style="background-color: white; color: #222222; font-family: "Open Sans", serif; font-size: 16px; margin: 0px 0px 24px;"><amp-img alt="Di menu "Keamanan" UEFI Anda, cari "TPM" dan "Diaktifkan."" height="488" i-amphtml-auto-lightbox-visited="" i-amphtml-layout="responsive" lightbox="i-amphtml-auto-lightbox-3" sizes="(min-width: 640px) 640px, 100vw" src="https://www.howtogeek.com/wp-content/uploads/2021/06/tpm_enabled.jpg?trim=1,1&bg-color=000&pad=1,1" style="--loader-delay-offset: 3ms !important; display: block; max-width: 100%; overflow: hidden; position: relative; width: 100vw;" width="650"><i-amphtml-sizer slot="i-amphtml-svc" style="display: block; padding-top: 246.25px;"></i-amphtml-sizer>![Di menu "Keamanan" UEFI Anda, cari "TPM" dan "Diaktifkan."](https://www.howtogeek.com/wp-content/uploads/2021/06/tpm_enabled.jpg?trim=1,1&bg-color=000&pad=1,1)</amp-img><figcaption style="color: #555555; font-family: -apple-system, BlinkMacSystemFont, "Open Sans", "Segoe UI", Roboto, Oxygen-Sans, Ubuntu, Cantarell, "Helvetica Neue", sans-serif; font-size: 14px; margin-top: 0px; padding: 10px 10px 10px 5px;"></figcaption></figure><span style="vertical-align: inherit;"><span style="vertical-align: inherit;">Demikian pula, dalam contoh UEFI kami, kami dapat menemukan pengaturan Boot Aman kami di bawah tab “Boot”. </span><span style="vertical-align: inherit;">Cari opsi “Boot Aman” dan pastikan itu diaktifkan.</span></span>

<figure style="background-color: white; color: #222222; font-family: "Open Sans", serif; font-size: 16px; margin: 0px 0px 24px;"><amp-img alt="Di menu "Boot" UEFI Anda, cari "Boot Aman" dan "Diaktifkan."" height="213" i-amphtml-auto-lightbox-visited="" i-amphtml-layout="responsive" lightbox="i-amphtml-auto-lightbox-2" sizes="(min-width: 640px) 640px, 100vw" src="https://www.howtogeek.com/wp-content/uploads/2021/06/secure_boot_enabled.jpg?trim=1,1&bg-color=000&pad=1,1" style="--loader-delay-offset: 3ms !important; display: block; max-width: 100%; overflow: hidden; position: relative; width: 100vw;" width="650"><i-amphtml-sizer slot="i-amphtml-svc" style="display: block; padding-top: 107.479px;"></i-amphtml-sizer>![Di menu "Boot" UEFI Anda, cari "Boot Aman" dan "Diaktifkan."](https://www.howtogeek.com/wp-content/uploads/2021/06/secure_boot_enabled.jpg?trim=1,1&bg-color=000&pad=1,1)</amp-img><figcaption style="color: #555555; font-family: -apple-system, BlinkMacSystemFont, "Open Sans", "Segoe UI", Roboto, Oxygen-Sans, Ubuntu, Cantarell, "Helvetica Neue", sans-serif; font-size: 14px; margin-top: 0px; padding: 10px 10px 10px 5px;"></figcaption></figure><span style="vertical-align: inherit;"><span style="vertical-align: inherit;">Setelah itu, pastikan Anda menyimpan perubahan yang telah Anda buat pada UEFI sebelum Anda keluar dari utilitas konfigurasi (biasanya Anda dapat memilih “simpan dan keluar” sebagai salah satu opsi).</span></span>

> **<span style="vertical-align: inherit;"><span style="vertical-align: inherit;">Catatan:</span></span>**<span style="vertical-align: inherit;"><span style="vertical-align: inherit;"> Jika Anda tidak melihat apa pun tentang TPM atau Boot Aman di layar pengaturan UEFI atau BIOS komputer Anda, PC Anda mungkin terlalu tua untuk memiliki fitur ini.</span></span>

<span style="vertical-align: inherit;"><span style="vertical-align: inherit;">Setelah keluar, PC Anda akan restart dan Windows akan memuat. </span><span style="vertical-align: inherit;">Saat Anda menjalankan pemeriksaan lagi, semoga Anda lulus ujian. </span><span style="vertical-align: inherit;">Jika fitur ini diaktifkan dan PC Anda masih tidak lulus pemeriksaan, ada </span></span>[<span style="vertical-align: inherit;"><span style="vertical-align: inherit;">alasan lain mengapa</span></span>](https://www.idev.my.id/search/label/seputar%20komputer)<span style="vertical-align: inherit;"><span style="vertical-align: inherit;"> mesin Anda tidak kompatibel dengan Windows 11.</span></span>

<span style="vertical-align: inherit;"><span style="vertical-align: inherit;">[Jika sudah mencoba cara seperti diatas namun gagal, coba pakai cara yang kedua ini](https://www.idev.my.id/2021/06/mengatasi-pc-cant-run-windows-11.html)</span></span>