## Pradipta Arya Pramudita - 2206083685
### Module 8
*Subscriber*
1. what is amqp? <br> 
AMQP adalah singkatan dari Advanced Message Queuing Protocol. AMQP adalah standar terbuka untuk mengirimkan pesan bisnis antara aplikasi atau organisasi. AMQP mendefinisikan protokol tingkat kabel biner yang memungkinkan negosiasi yang handal dan transmisi pesan yang efisien di antara aplikasi yang tersebar. Protokol ini memfasilitasi berbagai kemampuan perpesanan, termasuk antrian, perutean, keandalan, dan keamanan. <br> 

2. what it means? guest:guest@localhost:5672 , what is the first quest, and what is the second guest, and what is localhost:5672 is for? 
- 'guest' pertamaa adalah nama pengguna yang digunakan untuk menghubungkan ke layanan perpesanan. Dalam banyak sistem, "guest" adalah nama pengguna default yang disediakan untuk pengaturan awal atau pengujian.
- 'guest' kedua adalah kata sandi yang terkait dengan nama pengguna. Dalam hal ini, kata sandi juga adalah "guest".
- localhost:5672 merujuk ke komputer lokal tempat layanan perpesanan berjalan dan nomor port di mana layanan AMQP mendengarkan.
<br> <br>

![CargoRun](https://media.discordapp.net/attachments/784424703447400489/1232331447876980807/image.png?ex=66291198&is=6627c018&hm=80f81cf62fbfab0ff3bd2f15f0c645114139e7a8b77f8e5eba72d1a5bd903d39&=&format=webp&quality=lossless&width=1250&height=671)

Berdasarkan gambar, terdapat 10 queued messages. Hal ini terjadi karena "cargo run" pada publisher terkirim sebanyak 3 kali. Karena program publisher akan mengirimkan 5 data ke message broker dalam sekali run. Kemudian, karena yang queued ada 2 program publisher, sehingga queued messagesnya menjadi 2*5=10.

