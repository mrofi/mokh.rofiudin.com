---
slug: laravel-8-install-package-apt-node-dan-lain-lain-di-laravel-sail
date: 2021-06-24 13:34:34 
comments: true
authors:
  - mrofi
categories:
  - Programming
tags:
  - Laravel
---

# Laravel 8 : Install Package Apt, Node, dan Lain-lain di Laravel Sail

Terkadang, kita butuh untuk menambahkan beberapa package di environment system. 
Contoh kasus, ketika saya akan menggunakan package Laravel Medialibrary, saya harus menginstall beberapa optimization tools, : JpegOptim, Optipng, Pngquant 2, SVGO dan Gifsicle.
<!-- more -->

Untuk install di system (linux) cukup dengan 
<pre>sudo apt install -y jpegoptim optipng pngquant gifsicle
npm install -g svgo</pre>


Bagaimana jika menggunakan Laravel Sail.
Caranya cukup akses container menggunakan user ''<strong>root</strong>''.

Syntax nya kurang lebih seperti ini :
<pre>docker exec -u root {container_name} apt update
docker exec -u root {container_name} apt install -y jpegoptim optipng pngquant gifsicle
docker exec -u root {container_name} npm install -g svgo

</pre>

Selamat mencoba :)

<blockquote markdown>
Lihat juga :

<a href="/menulis/laravel-8-cara-install-yang-elegant-dan-handy-dandy">Laravel 8 : Cara Install Yang Elegant dan Handy-Dandy</a>

<a title="Laravel 8 : Mengatur Environment Variable Agar Bisa Menjalankan Multiple Instance (Untuk Development)" href="/menulis/laravel-8-mengatur-environment-variable-agar-bisa-menjalankan-multiple-instance-untuk-development">Laravel 8 : Mengatur Environment Variable Agar Bisa Menjalankan Multiple Instance (Untuk Development)</a>
</blockquote>
