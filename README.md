# Reflection

## Publisher
a. How much data your publisher program will send to the message broker in one run? \
Program publisher akan mengirim 5 data ke message broker dalam satu kali dijalankan.

b. The url of: “amqp://guest:guest@localhost:5672” is the same as in the subscriber program, what does it mean? \
URL amqp://guest:guest@localhost:5672 yang digunakan di program publisher dan subscriber menunjukkan bahwa keduanya terhubung ke server RabbitMQ yang sama di komputer lokal. guest:guest adalah username dan password default untuk autentikasi, localhost berarti broker berjalan di komputer sendiri, dan 5672 adalah port standar RabbitMQ. Karena menggunakan alamat yang sama, publisher bisa mengirim pesan dan subscriber bisa menerima pesan dari antrean yang sama melalui broker tersebut.

### Running RabbitMQ
![Running RabbitMQ as message broker](image/RunningRabbitMQ.png)

### Sending and Processing Event
![Sending and processing event](image/SendingAndProcessingEvent.png)
Ketika subscriber terkoneksi dengan RabbitMQ dan publisher mengirimkan data, maka subscriber akan menerima data yang dikirimkan publisher.

### Monitoring Chart Based on Publisher
![Monitoring chart based on publisher](image/MonitoringChartBasedOnPublisher.png)
Grafik ungu pada message rate merupakan Consumer ACK (acknowledgement), yakni konfirmasi dari subscriber ke message broker bahwa pesan telah berhasil diterima dan diproses.

## Bonus

### Sending and Processing Event (Cloud)
![Sending and processing event cloud](image/SendingAndProcessingEventCloud.png)

### Monitoring Chart Based on Publisher (Cloud)
![Monitoring chart based on publisher](image/MonitoringChartBasedOnPublisherCloud.png)
Terdapat grafik kuning, yakni publisher membuat pesan dan mempublikasikannya.
