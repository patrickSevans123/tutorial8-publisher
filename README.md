7. Try to answer the following questions, and write the answer in the and new file readme.md in
   you repository.  
   a. How many data your publlsher program will send to the message broker in one
   run?</br>
   Data yang akan dikirim oleh publisher kepada message broker dalam satu kali run adalah lima data karena publish_event dipanggil sebanyak lima kali. </br>
   b. The url of: “amqp://guest:guest@localhost:5672” is the same as in the subscriber program, what does it mean? </br>
   Hal ini dapat diartikan bahwa kedua program baik subsriber dan publisher terhubung pada message broker yang sama untuk memungkinkan penerimaan message oleh subscriber dari publisher.</br>

Picture of Running RabbitMQ:
![rabbit](img/rabbitmq-first-screenshot.png)

Picture of Subscriber's Console Output:
![console](img/console-subscriber.png)
Gambar diatas menunjukkan bahwa subscriber menerima message dari publisher pada saat program publisher dijalankan berupa lima baris output pada console. Subscriber yang terhubung pada message broker akan menerima data yang dikirimkan oleh publisher ke message broker.

Picture of Running RabbitMQ while sending and processing event:
![rabbit](img/rabbitmq-second-screenshot.png)
Gambar diatas menunjukkan adanya subscriber yang ditandai dengan "Connections: 1 dan Consumers: 1". Pada gambar juga terlihat bahwa message rates meningkat yang menunjukkan bahwa rata-rata message meningkat saat message dikirim oleh publisher.
