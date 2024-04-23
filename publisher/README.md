*Publisher*
1. How many data your publlsher program will send to the message broker in one run? <br>
5 message, Setiap message adalah sebuah event UserCreatedEventMessage yang berisi user_id dan user_name yang unik untuk setiap pesan. <br>
2. The url of: “amqp://guest:guest@localhost:5672” is the same as in the subscriber program, what does it mean? <br>
Jika URL "amqp://guest:guest@localhost:5672" digunakan baik dalam program pengirim maupun penerima (pelanggan), itu berarti bahwa baik pengirim (pengirim) maupun penerima (pelanggan) pesan terhubung ke broker AMQP yang sama, yang dihosting di mesin lokal ('localhost') menggunakan kredensial yang sama (nama pengguna "guest" dan kata sandi "guest") dan port AMQP standar (5672).

*RabbitMQ*

![RabbitMQ](https://media.discordapp.net/attachments/784424703447400489/1232028210926059671/rabbitmq.png?ex=6627f72f&is=6626a5af&hm=f336b2c080b997173436262cb461e04a450239faa5641528558f953d9d2b2583&=&format=webp&quality=lossless&width=1193&height=671)

![CargoRun](https://media.discordapp.net/attachments/784424703447400489/1232325327741780001/cargoRunSubs.png?ex=66290be5&is=6627ba65&hm=1bf1f087821abeca4700e19f41d586792d6653892842009480bc49f71267189d&=&format=webp&quality=lossless&width=1253&height=671)

Berdasarkan screenshots, dijalankan program subscriber lalu menjalankan program publisher. Kemudian memeriksa terminal pada program subscriber. Pada terminal program subscriber, dapat dilihat bahwa berhasil menerima 5 message sesuai yang dikirimkan pada program publisher. Dapat dilihat juga bahwa queued messagesnya 0, hal ini karena program ayng dijalankan hanya 1 dan cukup kecil.
