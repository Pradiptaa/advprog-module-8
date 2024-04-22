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

*Publisher*
1. How many data your publlsher program will send to the message broker in one run? <br>
5 message, Setiap message adalah sebuah event UserCreatedEventMessage yang berisi user_id dan user_name yang unik untuk setiap pesan. <br>
2. The url of: “amqp://guest:guest@localhost:5672” is the same as in the subscriber program, what does it mean? <br>
Jika URL "amqp://guest:guest@localhost:5672" digunakan baik dalam program pengirim maupun penerima (pelanggan), itu berarti bahwa baik pengirim (pengirim) maupun penerima (pelanggan) pesan terhubung ke broker AMQP yang sama, yang dihosting di mesin lokal ('localhost') menggunakan kredensial yang sama (nama pengguna "guest" dan kata sandi "guest") dan port AMQP standar (5672).

*RabbitMQ*

![RabbitMQ](https://media.discordapp.net/attachments/784424703447400489/1232028210926059671/rabbitmq.png?ex=6627f72f&is=6626a5af&hm=f336b2c080b997173436262cb461e04a450239faa5641528558f953d9d2b2583&=&format=webp&quality=lossless&width=1193&height=671)
