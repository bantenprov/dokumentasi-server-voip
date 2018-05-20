---
date: 2018-05-13
title: Instalasi Server Voip
categories:
  - server-voip
description: Membangun Server Voip
type: Document
---

## Pengenalan VoIP

Perkembangan teknologi telah membawa bisnis Telephony memasuki era baru yang menawarkan penyatuan seluruh komunikasi yang bersifat multimedia dan disalurkan melalui Internet, Perkembangan selanjutnya dari Internet ialah munculnya konsep yang dikenal dengan istilah Internet Telephony. 

Konsep IP ini memungkinkan penggabungan seluruh aplikasi-aplikasi dan layanan-layanan yang ada dalam Internet dan Telephony, sehingga konsep ini diperkirakan pada masa yang akan datang akan dipakai secara luas, digabungkan dengan infrastruktur Telephony yang sudah ada dan dapat diprekdisikan Kemampuan untuk melakukan komunikasi suara melalui Protokol Internet secara umum dikenal dengan istilah “ Suara diatas Protokol Internet”, “IP Telephony”, “Voice over IP” atau VoIP dapat diartikan sebagai kemampuan untuk melakukan hubungan telepon – dan semua kemampuan lainnya yang bisa dilakukan oleh jaringan telepon publik dan mengirimkan faksimili diatas jaringan berbasis IP dengan kualitas layanan yang memadai.

Perkembangan VoIP tersebut telah memacu revolusi dalam industri telekomunikasi. Untuk itu dalam implementasi telepon berbasis IP ini yang diterapkan dalam suatu jaringan lokal dibutuhkan suatu pengaturan dalam penyampaian datagram di jaringan IP yang dikenal dengan istilah routing. Pengaturan routing dapat menentukan kinerja dari suatu jaringan, dimana apabila suatu jaringan intranet membutuhkan suatu kebijakan dalam pembagian alokasi bandwith maupun otorisasi penggunaan komputer.

## Perancangan Server VoIP

VoIP server yang akan dibangun adalah menggunakan sistem operasi Linux server. Sistem Operasi Linux yang akan digunakan untuk pembuatan Server VoIP adalah Briker 2.0.4. Briker adalah distribusi Linux yang didalamnya terdapat aplikasi server yang memungkinkan pengguna mengimplementasikan layanan VoIP, membangun sentral telepon sendiri. Pada perancangan VoIP IP Address yang digunakan adalah IP Address IPV4. Server VoIP yang akan dibangun akan menggunakan protocol  Session  Initiation  Protocol  (SIP).  SIP yang digunakan adalah berupa aplikasi yang berfungsi sebagai Proxy Server, Redirect Server dan Registrar Server. Aplikasi ini dinamakan dengan Asterisk.

Tahap perancangan server yang pertama dilakukan adalah melakukan instalasi system operasi Briker pada computer yang akan dijadikan sebagai server VoIP. Setelah melakukan instalasi kita akan melakukan konfigurasi pada sisi server, dengan melakukan pembagian ekstensi yaitu memberikan penomoran atau alamat pada sisi client untuk bisa saling berkomunikasi antar client yang lain. 

Perancangan yang akan dilakukan pada sisi client adalah dengan menyiapkan sebuah komputer dan handphone yang memiliki system operasi android  yang akan difungsikan untuk melakukan dan menerima panggilan.    

## Instalasi dan Konfigurasi Server VoIP
### Instalasi Server VoIP
Proses Instalasi

![Instalasi](/images/server-voip/install-briker-1.png)
<center> Otomatis memeriksa perangkat keras jaringan, lalu mengkonfigurasi alamat IP secara otomatis </center>

![Instalasi](/images/server-voip/install-briker-2.png)
<center> Otomatis menghapus (format) hardisk dan menggunakan semua isi hardisk. </center>

![Instalasi](/images/server-voip/install-briker-3.png)
<center> Otomatis install base system dan software lainnya.</center>

![Instalasi](/images/server-voip/install-briker-4.png)
<center> Install GRUB boot loader </center>

![Instalasi](/images/server-voip/install-briker-5.png)
<center> Proses Finishing Installation, setelah itu mesin akan restart secara otomatis. </center>

![Instalasi](/images/server-voip/install-briker-6.png)
<center> Instalasi sistem selesai, mesin akan restart kembali. </center>

### Konfigurasi Server VoIP

Web Login
Browse alamat IP Briker melalui web browser, setelah itu akan muncul halaman untuk login seperti gambar di bawah ini.

![Web Login](/images/server-voip/voip-3.png)

---
Tampilan awal setelah kita melakukan Login

![Web Login](/images/server-voip/voip-2.png)

---
Menu-menu untuk mengatur fitur dari Server VoIP, antara lain pengaturan extensions, trunks dan routes. Fitur penting seperti Interactive Voice Response (IVR) dan Ring Group.

![Web Login](/images/server-voip/voip-4.png)

---
Call Detail Record Report, adalah laporan panggilan secara jelas dan lengkap, mulai dari waktu panggilan, tujuan panggilan, lama panggilan, asal panggilan, trunk yang digunakan, tarif panggilan, dan perhitungan keuntungan yang didapat. Menu ini dapat diakses dari menu Call Report, lalu pilih CDR Report.

![Call Record](/images/server-voip/voip-5.png)

---
Server VoIP status adalah menu untuk menampilkan Status Registry user akun yang online.

![Status Registry](/images/server-voip/voip-7.png)



