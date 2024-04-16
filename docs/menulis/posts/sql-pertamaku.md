---
slug: sql-pertamaku
date: 2011-01-06 10:10:00
comments: true
authors:
  - mrofi
categories:
  - Programming
tags:
  - SQL
---

# SQL Pertamaku

Entah kapan harinya dan tanggal pun ku lupa. Aku sadar bahwa microsoft excel mempunyai fitur macro. Macro adalah fasilitas yang disediakan oleh microsoft office untuk dapat memanipulasi software aplikasi buatannya, terutama di microsoft office. Tapi macro juga berjalan baik untuk memanipulasi software microsoft lainnya, bahkan di windows sebuah operating system buatan microsoft. Maka munculah apa yang dinamakan virus macro. Virus macro hanya aktif jika user membuka file office yang mengandung macro.

<!-- more -->

![SQL Pertamaku](../assets/images/sql-pertamaku-20171206081123_thumbnail1280x_.png)

Yah, dengan macro inilah ku membuat listing code program untuk melihat isi dari sebuah database SQL Server. SQLServer adalah database server buatan microsoft hanya terkenal cukup handal. Tapi menurutku masih kalah dengan MySQL karena suatu alasan non-logis bahwa SQLServer adalah aplikasi berbayar sedangkan MySQL merupakan software open source yang bisa kita ubah sesuai keinginan kita dan itu legal.

Tentu saja karena sama-sama buatan microsoft, microsft excel dapat melakukan interaksi secara mudah dengan database SQLServer. Manipula data pun dengan mudah dilakukan dengan membuat sambungan DSN dan semua itu sudah disediakan oleh microsoft di sistem operasi Windows. <br />Untuk melihat semua user id dan password orang-orang yang tersimpan di database tersebut misalnya, ku cuma butuh membutuhkan microsoft excel untuk merequest data dari database. Lewat menu external data yang sediakan kita tinggal membuat koneksi ke database dan memilih data dari tabel mana saja.

Setiap sambungan ke database SQLServer, kita akan ditanya user id dan password karena SQLServer perlu sebelum memperboleh masuk dan memanipulasi data di dalamnya. Entah karena kecerobohan si programer atau memang untuk alasan ke-praktis-an, pada menu konfigurasi di program client, user id dan password tertulis dengan jelasnya. Ini sangat menggelitik bahkan bagiku yang masih pemula. Tapi apa pun itu, yang namanya user id dan password selalu menarik perhatian. Mungkin sang programer benar-benar tidak menyadarinya.

Dan koneksi ke database server pun terjadi, kemudian ku telusuri satu per satu tabel data yang ada di dalamnya. Harus membuka puluhan tabel sebelum menemukan tabel yang memuat data user name dan password semua orang. Dan tidak terasa senyumku pun melebar dan respon berteriak "Yeah!. Ku berhasil. Huhu"

