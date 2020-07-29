Remarks
=======

1. Monitoring Dionaea
-------------------------

Dalam melakukan pratikum crawling malware ini terdapat hal yang perlu diperhatikan ketika sudah menjalankan dionaea yaitu selalu memonitoring log yang dilakukan dionaea. Hal tersebut dikarenakan ketika dionaea dijalankan maka akan banyak malware yang akan menyerang setiap saatnya. Oleh karena itu perlu dicontrol supaya jumlah storage / kapasitas dari server dionaea tidak habis terpenuhi. Hal tersebut dapat terjadi seperti kasus berikut dimana menjalankan dionaea selama 6 hari berturut turut tanpa termonitoring dan tercontrol. Oleh karena itu untuk mengantisipasi hal ini penulis menyarankan untuk selalu memonitoring setiap harinya dan menghentikan layanan dionaea jika penyimpanan hampir penuh. 

.. image :: 50.jpg

2. Monitoring Cowrie
----------------------------

Hal yang sama juga perlu diperhatikan ketika sudah menjalankan cowrie. Cowrie merupakan honeypot yang bersifat high-interaction sehingga terdapat kemungkinan adanya serangan yang berhasil mengakses sistem operasi pemilik cowrie. Oleh karena itu perlu selalu dimonitoring setiap saatnya. Selain itu juga perlu dimonitoring jumlah malware atau serangan yang tertampung sehingga cowrie kehabisan storage / penyimpanan data data malware atau serangan. Untuk mengatasi tersebut, penulis menyarankan untuk memonitoring setiap saat dan ketika hampir penuh dapat dihentikan layanan cowrienya. 

.. image :: 51.jpg
