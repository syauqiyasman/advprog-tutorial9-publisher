# Reflection

## Publisher
a. How much data your publisher program will send to the message broker in one run? \
Program publisher akan mengirim 5 data ke message broker dalam satu kali dijalankan.

b. The url of: “amqp://guest:guest@localhost:5672” is the same as in the subscriber program, what does it mean? \
URL amqp://guest:guest@localhost:5672 yang digunakan di program publisher dan subscriber menunjukkan bahwa keduanya terhubung ke server RabbitMQ yang sama di komputer lokal. guest:guest adalah username dan password default untuk autentikasi, localhost berarti broker berjalan di komputer sendiri, dan 5672 adalah port standar RabbitMQ. Karena menggunakan alamat yang sama, publisher bisa mengirim pesan dan subscriber bisa menerima pesan dari antrean yang sama melalui broker tersebut.
