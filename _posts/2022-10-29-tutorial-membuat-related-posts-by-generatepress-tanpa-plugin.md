---
id: 157
title: 'Tutorial Membuat Related Posts by GeneratePress, Tanpa Plugin'
date: '2022-10-29T22:00:00+00:00'
author: admin
layout: post
guid: 'http://localhost/wordpress/index.php/2022/10/29/tutorial-membuat-related-posts-by-generatepress-tanpa-plugin/'
permalink: /index.php/2022/10/29/tutorial-membuat-related-posts-by-generatepress-tanpa-plugin/
blogger_blog:
    - webidevloper.blogspot.com
blogger_author:
    - IDEV.My.ID
blogger_internal:
    - /feeds/2636143461486592706/posts/default/5647023549922093968
categories:
    - TutorialBlogger
---

<div><div>HasilkanTekan (GP) adlah *tema* berbasis *editor blok* cukup *kuat*. Ringan, mudah dikendalikan, dan didukung oleh dokumentasi yang baik. GP juga cocok untuk para pengembang tema WordPress yang ingin membuat situs web untuk klien tanpa harus *pengkodean dari awal*.

Namun, dengan cukup banyak kelebihan, *tema* yang satu ini juga punya kekurangan. Salah satunya, tidak dilengkapi dengan fitur *Pos terkait*. Padahal, ini fitur yang cukup berguna untuk para blogger.

Ada dua cara untuk membuat fitur ini: dengan plugin, tanpa plugin. Saya memilih opsi kedua karena dua alasan:

- **Cara membuatnya cukup sederhana.** rasanya *berlebihan* kalau harus menambah *pengaya* hanya untuk membuat fitur yang tidak terlalu rumit dan bisa dikerjakan sendiri.
- **Menghemat ruang disk.** Menambah plugin artinya menambah beban <s>hidup</s> server. Jadi, agar tidak terlalu banyak *pengaya*saya memilih ngoding sendiri.

- - - - - -

## Cara Membuat Related Post di GeneratePress

Saya berasumsi Anda sudah menggunakan *tema anak*. Bila belum, silakan buat terlebih dahulu. Oh ya, Anda bisa membuat *Pos terkait* berdasarkan kategori atau berdasarkan *menandai*.

<span><svg fill="currentColor" height="16" viewbox="0 0 16 16" width="16" xmlns="http://www.w3.org/2000/svg"> <path d="M8 16A8 8 0 1 0 8 0a8 8 0 0 0 0 16zm.93-9.412-1 4.705c-.07.34.029.533.304.533.194 0 .487-.07.686-.246l-.088.416c-.287.346-.92.598-1.465.598-.703 0-1.002-.422-.808-1.319l.738-3.468c.064-.293.006-.399-.287-.47l-.451-.081.082-.381 2.29-.287zM8 5.5a1 1 0 1 1 0-2 1 1 0 0 1 0 2z"></path> </svg></span><span>**Prasyarat:** PHP, CSS, HTML.</span>

1. Tambahkan hook di file functions.php

tambah *naskah* ini di file **function.php** *tema anak*. ganti *domain teks* menjadi *tema domain teks* Anda. Untuk penamaan *fungsi* dan *kelas* juga bisa diganti dan disesuaikan.

**Berdasarkan kategori:**

```
// Related Post Berdasarkan Kategori<br></br>add_action( 'generate_before_comments_container','langit_related_post' ); <br></br>function langit_related_post() <br></br>	if ( is_single() ) : ?><br></br><div class="related-post__container"><br></br>	<h2 class="related-post__header">Related Posts</h2><br></br>	<div class="related-post__content"><br></br>		<?php<br></br> global $post;<br></br> $orig_post = $post;<br></br> $categories = get_the_category($post->ID);<br></br> <br></br> if ($categories) <br></br> $categories_ids = array();<br></br> foreach($categories as $individual_category) $category_ids[] = $individual_category->term_id;<br></br> $args=array(<br></br> 'category__in' => $category_ids,<br></br> 'post__not_in' => array($post->ID),<br></br> 'posts_per_page' => 3, // Number of related posts to display.<br></br> 'ignore_sticky_posts' => 1<br></br> );<br></br> <br></br> $related_query = new wp_query( $args );<br></br> <br></br> while( $related_query->have_posts() ) <br></br> $related_query->the_post();<br></br> ?><br></br><br></br>		<div class="related-post__item"><br></br>			<div class="related-post__item--thumb"><br></br>				<a rel="nofollow" href="<? the_permalink()?>"><?php the_post_thumbnail(array(300,150)); ?><br></br>				</a><br></br>			</div><br></br>			<h3 class="related-post__item--title"><br></br>				<a href="<? the_permalink()?>"><?php the_title(); ?></a><br></br>			</h3><br></br>		</div><br></br><br></br>		<? <br></br> <br></br> $post = $orig_post;<br></br> wp_reset_query();<br></br> ?><br></br>	</div><br></br></div><br></br><?php <br></br>	endif;<br></br>
```

**Berdasarkan tag:**

```
// Related Post Berdasarkan Tags<br></br>add_action( 'generate_before_comments_container','langit_related_post' ); <br></br>function langit_related_post() <br></br>	if ( is_single() ) : ?><br></br><div class="related-post__container"><br></br>	<h2 class="related-post__header">Related Posts</h2><br></br>	<div class="related-post__content"><br></br>		<?php<br></br> global $post;<br></br> $orig_post = $post;<br></br> $tags = get_the_tag($post->ID);<br></br> <br></br> if ($tags) <br></br> $tags_ids = array();<br></br> foreach($tags as $individual_tag) $category_ids[] = $individual_tag->term_id;<br></br> $args=array(<br></br> 'tag__in' => $tag_ids,<br></br> 'post__not_in' => array($post->ID),<br></br> 'posts_per_page' => 3, // Number of related posts to display.<br></br> 'ignore_sticky_posts' => 1<br></br> );<br></br> <br></br> $related_query = new wp_query( $args );<br></br> <br></br> while( $related_query->have_posts() ) <br></br> $related_query->the_post();<br></br> ?><br></br><br></br>		<div class="related-post__item"><br></br>			<div class="related-post__item--thumb"><br></br>				<a rel="nofollow" href="<? the_permalink()?>"><?php the_post_thumbnail(array(300,150)); ?><br></br>				</a><br></br>			</div><br></br>			<h3 class="related-post__item--title"><br></br>				<a href="<? the_permalink()?>"><?php the_title(); ?></a><br></br>			</h3><br></br>		</div><br></br><br></br>		<? <br></br> <br></br> $post = $orig_post;<br></br> wp_reset_query();<br></br> ?><br></br>	</div><br></br></div><br></br><?php <br></br>	endif;<br></br>
```

<span><svg fill="currentColor" height="16" viewbox="0 0 16 16" width="16" xmlns="http://www.w3.org/2000/svg"> <path d="M8 16A8 8 0 1 0 8 0a8 8 0 0 0 0 16zm.93-9.412-1 4.705c-.07.34.029.533.304.533.194 0 .487-.07.686-.246l-.088.416c-.287.346-.92.598-1.465.598-.703 0-1.002-.422-.808-1.319l.738-3.468c.064-.293.006-.399-.287-.47l-.451-.081.082-.381 2.29-.287zM8 5.5a1 1 0 1 1 0-2 1 1 0 0 1 0 2z"></path> </svg></span><span>**Catatan:** saya sengaja meletakkan hook di `generate_before_comments_container` agar related post tidak menjadi bagian dari `<article>.` IMO, secara semantik ini lebih masuk akal. Kalau Anda mau, bisa juga mengganti tag HTML `<div class="related-post__container>` menjadi `<region>` atau `<aside>`.</span>

2. Atur tampilan dengan CSS

Atur tampilan. tambah ini di **CSS tambahan** atau di **style.css** *tema anak*.

```
/* Related Post */<br></br>.related-post__content <br></br>	display: flex;<br></br>	justify-content: space-between;<br></br><br></br><br></br>.related-post__item <br></br>	flex-basis: 30%;<br></br><br></br><br></br>.related-post__item--thumb <br></br>	background-color: var(--contrast);<br></br>	height: 200px;<br></br>	width: 100%;<br></br>	margin-bottom: 10px;<br></br><br></br><br></br>.related-post__item--thumb a:hover <br></br>	opacity: 0.5;<br></br><br></br><br></br>.related-post__item--thumb img <br></br>	height: 200px;<br></br>	width: 100%;<br></br>	object-fit: cover;<br></br><br></br><br></br>.related-post__item--title <br></br>	font-size: 16px;<br></br>	text-align: center;<br></br><br></br><br></br>.related-post__item--title a <br></br>	color: var(--contrast-2);<br></br>	text-decoration: none;<br></br><br></br><br></br>.related-post__item--title a:hover <br></br>	color: var(--accent);<br></br><br></br><br></br>@media only screen and (max-width: 800px ) <br></br>	.related-post__content <br></br>		flex-direction: column;<br></br>	<br></br>
```

3. selesai

Selesai, deh. Tampilannya kira-kira seperti ini:

<figure>![Cara membuat postingan terkait tanpa plugin](https://www.langitamaravati.com/wp-content/uploads/2022/09/contoh-related-post-1024x322.webp)</figure>Bila Anda kurang sreg dengan tampilannya, bisa dimodifikasi sendiri di CSS.

- - - - - -

Sekian tutorial coding kali ini. Semoga membantu. **(eL)**

</div><span><svg aria-hidden="true" height="1em" role="img" viewbox="0 0 640 512" width="1em" xmlns="http://www.w3.org/2000/svg"><path d="M497.941 225.941L286.059 14.059A48 48 0 0 0 252.118 0H48C21.49 0 0 21.49 0 48v204.118a48 48 0 0 0 14.059 33.941l211.882 211.882c18.744 18.745 49.136 18.746 67.882 0l204.118-204.118c18.745-18.745 18.745-49.137 0-67.882zM112 160c-26.51 0-48-21.49-48-48s21.49-48 48-48 48 21.49 48 48-21.49 48-48 48zm513.941 133.823L421.823 497.941c-18.745 18.745-49.137 18.745-67.882 0l-.36-.36L527.64 323.522c16.999-16.999 26.36-39.6 26.36-63.64s-9.362-46.641-26.36-63.64L331.397 0h48.721a48 48 0 0 1 33.941 14.059l211.882 211.882c18.745 18.745 18.745 49.137 0 67.882z" fill="currentColor"></path></svg></span><span><span>HasilkanTekan</span> <span>Tema WordPress</span></span>

</div>