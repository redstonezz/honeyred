Introduction
============

1. Honeypot and Honeynet
---------------------------

Honeynet merupakan sekumpulan honeypot yang didesain untuk menarik perhatian seorang attacker dengan kerawanan yang sengaja dibuat pada suatu sistem dan jaringan. Hooneynet akan menyediakan layanan yang dibutuhkan oleh attacker sehingga dapat melancarkan serangan tersebut. Setelah itu dari aktivitas serangan dan metode serangan yang tertangkap pada honeynet akan dapat dipelajari atau dianalisis sehingga dapat meningkatkan keamanan jaringan. Selain itu tujuan dibuatnya honeynet juga supaya menjadi umpan sehingga jaringan yang terdapat aset organisasi tidak diserang.

Honeypot adalah security resource yang sengaja dibuat untuk diselidiki, diserang, atau dikompromikan. Pada umumnya Honeypot berupa komputer, data, atau situs jaringan yang terlihat seperti bagian dari jaringan, tapi sebenarnya itu hanyalah umpan yang terisolasi dan termonitor. Jika dilhat dari sisi penyerang, maka honeypot tampak seperti suatu server atau komputer biasa saja yang dapat menjadi serangan. Oleh karena itu seoarang attacker tidak menyadari bahwa itu hanyalah umpan. Konsep tujuan yang digunakan oleh honeypot yaitu untuk “know yout enemy”. Dengan mengimplementasikan suatu honeypot maka dapat memperoleh pengetahuan seperti apa yang dicari oleh attacker dan tools yang digunakan. Pengetahuan itulah yang nantinya digunakan unuk meningkatkan keamanan dan melindungi sistem.

Honeypot dapat diklasifikasikan berdasarkan pada tingkat interaksi yang dimilikinya, yang dimaksud tingkat interaksi adalah  tingkat aktivitas penyerang didalam sistem yang diperbolehkan maka semakin tinggi pula tingkat interaksi honeypot. Berikut merupaka beberapa jenis interaksi pada honeypot:

1.1 High-interaction Honeypot
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

High-interaction honeypot menawarkan suatu kerentanan dari sistem operasi nyata yang mengizinkan seorang attacker dapat berinteraksi langsung dengan sistem operasi tersebut. Pada honeypot ini desediakan sistem operasi dimana penyerang dapat berinteraksi langsung dan tidak ada batasan yang membatasi interaksi tersebut. Menghilangkan batasan-batasan tersebut menyebabkan tingkat risiko yang dihadapi semakin tinggi karena penyerang dapat memiliki akses root dan dapat digunakan untuk mendeteksi zero-day attaks. Pada saat yang sama, kemungkinan pengumpulan informasi semakin meningkat dikarenakan kemungkinan serangan yang tinggi. Dikarenakan penyerang dapat berinteraksi secara penuh dengan sistem operasi, maka apabila si penyerang telah mendapat akses root. Berikut merupakan kelebihan dan kekurangan dari high-interaction honeypot.
	
1.1.1 Kelebihan High-interaction honeypot

	- Penyerang berinteraksi langsung dengan sistem yang nyata termasuk diantaranya sistem operasi, network, hingga layanan yang diberikan ( web service, ssh service, mail service, dll ).

	- Umumnya dibangun suatu sistem khusus dengan topologi yang telah dipersiapkan.

	- Sistem tersebut biasanya terdiri dari berbagai macam implementasi dari teknologi keamanan yang banyak digunakan untuk melindungi suatu sistem, seperti firewall, IDS/IPS, router, dll.

	- Target serangan berupa sistem operasi sebenarnya yang siap untuk berinteraksi secara langsung dengan penyerang.

1.1.2 Kekurangan High-interaction honeypot

	- Perencanaan dan implementasi sistem jauh lebih rumit dan dibutuhkan banyak pertimbangan.

	- High-interaction honeypot bersifat tidak efisien karena membutuhkan pengawasan berkala.

	- Apabila telah diambil alih oleh penyerang maka honeypot tersebut dapat menjadi ancaman bagi jaringan yang ada.

1.2 Low-interaction Honeypot
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
       
Low-interaction honeypot menawarkan kerentanan yang tampak seperti emulasi dari layanan yang diperlukan oleh attacker. Pada sistem ini sangat mudah untuk dibuat dan memerlukan sedikit code untuk membuat honeypot tersebut. Akan tetapi juga dapat memudahkan seorang attacker untuk mengetahui bahwa sistem yang dibuat tersebut hanyalah umpan. Low-interaction honeypot menyediakan tingkat interaksi yang dibatasi. Akan tetapi honeypot yang didesain untuk mengemulasikan service (layanan) seperti pada server yang asli. Berikut merupakan kelebihan dan kekurangan low-interaction honeypot.

1.2.1 Kelebihan Low-interaction honeypot

	- Mudah di install, dikonfigurasi, deployed, dan dimaintain.

	- Mampu mengemulasi suatu layanan seperti http, ftp, telnet, dsb.

	- Difungsikan untuk deteksi serangan, khususnya pada proses scanning atau percobaan.

1.2.2 Kekurangan Low-interaction honeypot

	- Layanan yang di berikan hanya berupa emulasi, sehingga penyerang tidak dapat berinteraksi secara penuh dengan layanan yang diberikan atau sistem operasinya secara langsung.

	- Informasi yang bisa kita dapatkan dari penyerang sangat minim.

	- Apabila serangan dilakukan oleh real person bukan automated tools mungkin akan segera menyadari bahwa yang sedang dihadapi merupakan mesin honeypot, karena keterbatasan layanan yang bisa diakses.

2. Dionaea
----------

Dionaea adalah honeypot interaksi rendah yang menangkap muatan serangan dan malware. Prinsip dari cara kerja dionea yaitu dengan membuat perangkap yang memiliki sistem deteksi. Setelah itu dionea akan membuka layanan yang dibutuhkan malware sehingga malware tersebut masuk ke dionea dan terperangkap. Dionaea dimaksudkan untuk menggunakan bahasa script python kemudian implementasikan penggunakan libemu untuk mendeteksi kode-kode shell, serta mendukung ipv6 dan tls.

3. Cowrie
-----------

Cowrie adalah SSH dan Telnet honeypot interaksi sedang hingga tinggi yang dirancang untuk mencatat serangan brute force dan interaksi shell yang dilakukan oleh penyerang. Dalam mode interaksi sedang (shell) ia mengemulasi sistem UNIX dengan Python, dalam mode interaksi tinggi (proxy) berfungsi sebagai SSH dan proxy telnet untuk mengamati perilaku penyerang ke sistem lain.



	 
