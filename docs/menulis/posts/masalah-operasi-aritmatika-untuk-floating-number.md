---
slug: masalah-operasi-aritmatika-untuk-floating-number
date: 2022-02-19 17:26:50
comments: true
authors:
  - mrofi
categories:
  - Programming
tags:
  - Floating Number
---

# Masalah Operasi Aritmatika untuk Floating Number

Di beberapa bahasa pemrograman, operasi aritmatika <strong>(tambah, kurang, kali, bagi, dll)</strong> untuk bilangan decimal <em>dalam hal ini khusus tipe data <strong>float</strong></em> menjadi sebuah momok. Floating number ini kadang juga menjadi masalah ketika disimpan di database.

<!-- more -->

Contohnya operasi berikut :
<pre data-params="php">var_dump(9.95 * 100 - 993);
// PHP &lt;= 7.4.x, hasilnya : float(1.9999999999999)
// PHP &gt;= 8.0.x, hasilnya : float(1.9999999999998863)</pre>
<pre data-params="javascript"><code>console.log(9.95 * 100 - 993);
// 1.9999999999998863
// </code></pre>

Solusinya sederhananya bisa dengan cara merubahnya dari tipe float menjadi tipe data decimal atau yang lebih extreme merubahnya jadi integer ketika disimpan dan ketika melakukan operasi.

Tapi, ternyata tiap bahasa pemrograman ada fitur atau extension khusus untuk menghandle floating number.

Ada sebuah website yang membahas hal tersebut : <a href="https://floating-point-gui.de">https://floating-point-gui.de</a>

Di website tersebut juga dibahas solusi di spesifik bahasa pemrograman, seperti :

PHP : <a href="https://floating-point-gui.de/languages/php/">https://floating-point-gui.de/languages/php/</a>

Javascript : <a href="https://floating-point-gui.de/languages/javascript/">https://floating-point-gui.de/languages/javascript/</a>

Java : <a href="https://floating-point-gui.de/languages/java/">https://floating-point-gui.de/languages/java/</a>

SQL : <a href="https://floating-point-gui.de/languages/sql/">https://floating-point-gui.de/languages/sql/</a>
