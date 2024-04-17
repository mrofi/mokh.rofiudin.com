---
slug: laravel-8-mengatur-environment-variable-agar-bisa-menjalankan-multiple-instance-untuk-development
date: 2021-06-01 14:05:27
comments: true
authors:
  - mrofi
categories:
  - Programming
tags:
  - Laravel
---

# Laravel 8 : Mengatur Environment Variable Agar Bisa Menjalankan Multiple Instance (Untuk Development)


Jika Anda seorang developer Laravel yang mengerjakan banyak project sekaligus pastinya ingin app-app tersebut bisa diakses bersamaan. Ketika ingin menjalankan beberapa instance sekaligus biasanya akan muncul error dikarenakan kesamaan port-port yang digunakan.

<!-- more -->

Contoh kasus misal Anda harus menjalankan 2 instance laravel. 1 Untuk API dan 1 nya untuk app yang consume API tersebut. App pertama berjalan dengan baik, ketika akan menjalankan app kedua maka muncul error dikarenakan <strong><em>"port is already allocated".</em></strong>


Solusinya adalah mengatur tiap instance agar menggunakan port-port yang berbeda.

Caranya cukup dengan menambahkan di environment variable, nilai port-port yang akan digunakan.
Untuk variable-variable apa saja bisa dilihat di file <strong>"docker-compose.yml"</strong>.
Di file tersebut ada banyak variable yang bisa diubah via file .env.
Misalnya, di situ ada variable <code>${APP_PORT:-80}</code> artinya variable <strong>APP_PORT</strong> mempunya nilai default <strong>80</strong>.
Jika app Anda ingin berjalan di port selain <strong>80</strong> tinggal tambahkan variable <strong>APP_PORT=10009</strong> di file .env Anda untuk membuat app Anda berjalan di <strong>port 10009</strong>.

Variable-variable lain di-antaranya yang sering digunakan adalah :</p>
<code>${FORWARD_DB_PORT:-3306}</code>


<code>${FORWARD_REDIS_PORT:-6379}</code>


<code>${FORWARD_MAILHOG_PORT:-1025}</code>


<code>${FORWARD_MAILHOG_DASHBOARD_PORT:-8025}</code>
 

Anda pun bisa mengganti value lain di file <strong>"docker-composer.yml"</strong> dan diganti menjadi variable kemudian tambahkan di file .env

Selamat mencoba :)

<blockquote markdown>
Lihat juga :

<a href="/menulis/laravel-8-cara-install-yang-elegant-dan-handy-dandy">Laravel 8 : Cara Install Yang Elegant dan Handy-Dandy</a>

<a title="Laravel 8 : Install Package Apt, Node, dan Lain-lain di Laravel Sail" href="/menulis/laravel-8-install-package-apt-node-dan-lain-lain-di-laravel-sail">Laravel 8 : Install Package Apt, Node, dan Lain-lain di Laravel Sail</a>
</blockquote>
