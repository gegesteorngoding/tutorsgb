---
title: "Membuat Website Dengan Hugo :D"
description: "Apa itu Hugo dan panduan instalasi"
date: 2025-06-28T11:24:13+07:00
draft: false
showCodeCopyButtons:
cover:
    image: "/images/hugo.png"
---

Kamu ingin membuat sebuah website tapi malas untuk mendesign satu satu. Dari mulai menulis HTML CSS dan bahkan JavaScript (JS) yang paling ribet dan menyusahkan. Tapi ada sebuah alat bernama Hugo yang memungkinkan kita untuk membuat website entah itu blog atau portofolio dengan mudah, tanpa membuat satu satu HTML CSS dan JS-nya, hanya bermodalkan file Markdown (.md).    

Gimana caranya ? lestgoo :D

# Apa itu Hugo ?

Hugo adalah sebuah <i>static site generator</i> (SSG) yang dibuat dengan bahasa Go. Sebuah bahasa yang dikembangkan oleh Google yang mengutamakan efisiensi, kesederhanaan dan kemudahan penggunaan. Fungsi dari Hugo adalah untuk mengcompile file markdown (.md) menjadi <i>static site</i>, tanpa server database.  

# Web Statis ?

Web statis itu web yang kontennya ditampilkan alakadarnya (apa adanya), tanpa dipicu oleh interaksi pengguna. Web jenis statis biasanya cuman dibuat dengan HTML, CSS, JS, dan kawan kawannya, gak ada PHP (Hypertext Preprocessor) bukan yang satunya.  

Dan sekarang kamu tahu apa itu web statis, Hugo cuman bisa bikin web statis jadi jangan ekspektasi yang berlebihan kayak "nanti didalamnya ada Database dsb.".

# Instalasiii

<h2>Windows</h2>

Untuk menginstall Hugo di Windows, kamu bisa menggunakan salah satu dari 3 package manager yang tersedia di Windows.

1. <a href="https://chocolatey.org/">Chocolatey</a>
2. <a href="https://scoop.sh/">Scoop</a>
3. Atau <a href="https://learn.microsoft.com/en-us/windows/package-manager/">Winget</a>

<h3>Chocolatey</h3>
<pre>choco install hugo-extended</pre>
<h3>Scoop</h3>
<pre>scoop install hugo-extended</pre>
<h3>Winget</h3>
<pre>winget install Hugo.Hugo.Extended</pre>

Pilihan lain, yaitu build dari source atau <i>prebuild binaries</i> bisa kamu lihat sendiri di panduan resmi <a href="https://gohugo.io/installation/windows/">Hugo</a>.

<h2>Linux</h2>

Linux punya buaanyak distro, disini saya akan menjelaskan instalasi dari 3 distro yang umum yang yang paling sering dipakai.

<h3>Debian</h3>
<pre>sudo apt install hugo</pre>
<h3>Arch Linux</h3>
<pre>sudo pacman -S hugo</pre>
<h3>Fedora</h3>
<pre>sudo dnf install hugo</pre>

Jika kamu memakai selain 3 distro diatas, kamu bisa mengikuti panduan dari situs web resmi dari <a href="https://gohugo.io/installation/windows/">Hugo</a>.

# Mulai membuat web statismu sendiri :D

Untuk demo saja, ada beberapa langkah yang harus kamu ikuti untuk membuat sebuah web statis yang <i>Masterpiece</i>

1. Buat site hugomu dulu wak.
<pre>hugo new site namaproject</pre>

2. Pergi ke folder situsmu, dan inisialisasi gitmu
<pre>cd namaproject && git init</pre>

3. Install theme, ada banyak sekali theme yang disediakan oleh <a href="https://themes.gohugo.io/">Hugo</a>. Dalam tutorial ini saya akan menggunakan PaperMod.
<pre>git submodule add https://github.com/adityatelange/hugo-PaperMod.git themes/papermod</pre>

Jangan lupa tambahkan ini di config.toml
<pre>themes = "papermod" (sesuai nama thememu)</pre>

4. Tambahkan konten <i>sak karepmu</i> :D  

Buat folder 'content/posts'  
Terus buat file.md  
<pre>hugo new posts/'namakonten'.md</pre>

5. Buat lalu <i>Djalankan</i>  
<pre>hugo && hugo server</pre>

# Penutup

Dann... Yap... kamu sudah membuat sebuah mahakarya dengan Hugo. Aku harap blog ini bermanfaat, dan matur tenkyu :D
  















