# Infrastruktur Global AWS

![Infrastruktur Global AWS](https://github.com/putrafa/linuxsysadmin/assets/121589476/5efe8598-bb16-4beb-802e-14b1b14658c2)

![Infrastruktur Global AWS](https://github.com/putrafa/linuxsysadmin/assets/121589476/3aff2c5a-8ea5-4b04-9c07-4117b0a45201)

Infrastruktur AWS Cloud dibangun di sekitar Wilayah. AWS memiliki 22 Wilayah di seluruh dunia. Satu Wilayah AWSadalah lokasi geografis fisik dengan satu atau beberapa Availability Zone. Availability Zone terdiri dari satu atau beberapa pusat data.

Untuk mencapai toleransi kesalahan dan stabilitas, Wilayah diisolasi dari satu sama lain. Sumber daya di satu Wilayah tidak secara otomatis direplikasi ke Wilayah lain. Saat Anda menyimpan data di Wilayah tertentu, data Anda tidak direplikasi di luar Wilayah tersebut.

Merupakan tanggung jawab Anda untuk mereplikasi data lintas Wilayah, jika bisnis Anda memerlukannya.

Wilayah AWS yang diperkenalkan sebelum 20 Maret 2019diaktifkansecara default. Wilayah yang diperkenalkan setelah 20 Maret 2019—seperti Asia Pasifik (Hong Kong) dan Timur Tengah (Bahrain)—dinonaktifkansecara default. Anda harus mengaktifkan Wilayah ini sebelum Anda dapat menggunakannya. Anda dapat menggunakan AWS Management Console untuk mengaktifkan atau menonaktifkan Wilayah.

Beberapa Wilayah memiliki akses terbatas. Akun Amazon AWS (Tiongkok) hanya menyediakan akses ke Wilayah Beijing dan Ningxia. Untuk mempelajari lebih lanjut entang AWS di Tiongkok.

## Memilih Wilayah

![Memilih Wilayah](https://github.com/putrafa/linuxsysadmin/assets/121589476/c30ac943-4dfc-4743-a03b-798950e8905f)

Terdapat beberapa faktor yang perlu dipertimbangkan saat memilih satu atau beberapa Wilayah optimal, tempat Anda menyimpan data dan menggunakan layanan AWS.

Salah satu pertimbangan penting adalah tata kelola data dan persyaratan hukum. Undang-undang setempatmungkin mengharuskan informasi tertentu disimpan di dalam batas geografis. Undang-undang tersebut dapat membatasi Wilayah tempat Anda dapat menawarkan konten atau layanan. Misalnya, pertimbangkan European Union (EU) Data Protection Directive.

Biasanya, menjalankan aplikasi dan menyimpan data di Wilayah yang sedekat mungkin dengan pengguna dan sistem yang akan mengaksesnya merupakan hal yang diinginkan. Ini akan membantu Anda mengurangi latensi. CloudPing adalah salah satu situs web yang dapat digunakan untuk menguji latesi antara lokasi Anda dan semua Wilayah AWS.

## Availability Zone

![Availability Zone](https://github.com/putrafa/linuxsysadmin/assets/121589476/a711d8f9-fe9b-49db-a92b-2f212e3523d7)

Setiap Wilayah AWS memiliki banyak lokasi terisolasi yang dikenal sebagaiAvailability Zone.

Setiap Availability Zone menyediakan kemampuan untuk mengoperasikan aplikasi dan basis data yang tersedia dengan sangat baik, toleran terhadap kesalahan, dan dapat diskalakan daripada yang mungkin dilakukan dengan satu pusat data. Setiap Availability Zone dapat mencakup beberapa pusat data (biasanya tiga), dan pada skala penuh, dapat mencakup ratusan ribu server. Availability Zone merupakan partisi Infrastruktur Global AWS yang terisolasi penuh. Availability Zone memiliki infrastruktur daya tersendiri, dan secara fisik berjarak sangat jauh dari Availability Zone lainnya—tetapi semua Availability Zone berjarak 100 km satu sama lain.

Semua Availability Zone saling berhubungan dengan jaringan bandwidth tinggi yang berlatensi rendah melalui fiber khusus yang sepenuhnya redundan, yang menyediakan throughput tinggi di antara Availability Zone. Jaringan tersebut mencapai replikasi sinkronis di antara Availability Zone.

Availability Zone membantu membangun aplikasi yang tersedia dengan sangat baik. Saat aplikasi dipartisi di seluruh aplikasi Availability Zone, perusahaan diisolasi dan dilindungi dengan lebih baik dari masalah seperti petir, tornado, gempa bumi, dan lainnya.

## Pusat data AWS

![Pusat Data AWS](https://github.com/putrafa/linuxsysadmin/assets/121589476/a5b7efd8-bf3c-47d6-a539-c9daa1adc009)

Dasar untuk infrastruktur AWS adalah pusat data. Pelanggan tidak menentukan pusat data untuk deployment sumber daya. Sebaliknya, Availability Zone adalah tingkat spesifikasi paling granular yang dapat dibuat pelanggan. Namun, pusat data adalah lokasi tempat data aktual berada. Amazon mengoperasikan pusat data mutakhir yang tersedia dengan sangat baik. Meskipun jarang, kegagalan yang memengaruhi ketersediaan instans di lokasi yang sama dapat terjadi. Jika Anda meng-host semua instans Anda di satu lokasi yang terpengaruh oleh kegagalan tersebut, tidak ada instans Anda yang akan tersedia.

Pusat data AWS dirancang dengan aman dengan mempertimbangkan beberapa faktor:

- Setiap lokasi dievaluasi dengan saksama untuk mengurangi risiko lingkungan.
- Pusat data memiliki desain redundanyang mengantisipasi dan menoleransi kegagalan sekaligus menjaga tingkat layanan.
- Untuk memastikan ketersediaan, komponensistem penting dicadangkandi beberapa Availability Zone.
- Untuk memastikan kapasitas, AWS terus memantau penggunaan layanan untuk men-deploy infrastruktur guna mendukung komitmen dan persyaratan ketersediaan.Lokasi Pusat data tidak diungkapkandan semua akses ke sana dibatasi.
- Jika terjadi kegagalan, proses otomatis memindahkan lalu lintas data dari area yang terdampak.

AWS menggunakanperalatan jaringan khususyang bersumber dari beberapa Produsen Perangkat Asli yang juga dikenal sebagai ODM. ODM merancang dan membuat produk berdasarkan spesifikasi dari perusahaan kedua. Perusahaan kedua kemudian mengubah merek produk untuk dijual.

## Point of Presence

![Point of Presence](https://github.com/putrafa/linuxsysadmin/assets/121589476/5de4c86f-d871-4bc4-8e77-51112093be24)

Amazon CloudFrontadalah jaringan penyampaian konten(CDN) yang digunakan untuk mendistribusikan konten ke pengguna akhir untuk mengurangi latensi. Amazon Route 53 adalah layanan Domain Name System (DNS). Permintaan ke salah satu layanan ini akan dialihkan ke edge locationterdekat secara otomatis untuk menurunkan latensi.

Points of PresenceAWS terletakdi sebagianbesarkotabesardi (total 69 kota) di 30 negaradi seluruhdunia. Denganterus mengukur konektivitas internet, kinerja, dan komputasi untuk menemukan cara terbaik untuk merutekan permintaan, Points of Presence memberikanpengalamanpenggunayang lebihbaikhampirsecarareal-time. TitikkehadiraninidigunakanolehbanyaklayananAWS, termasuklayananAmazon CloudFront, Amazon Route 53, AWS Shield, danAWS Web Application Firewall (AWS WAF).

Cache Edge Wilayahldigunakan secara default dengan Amazon CloudFront. Cache edge regional digunakan saat Anda memiliki konten yang tidak cukup sering diakses untuk tetap berada di edge location. Cache edge Regional menyerap konten ini dan memberikan alternatif terhadap konten yang harus diambil dari server asal.

## Fitur Infrastruktur AWS

![Fitur Infrastruktur AWS](https://github.com/putrafa/linuxsysadmin/assets/121589476/1d5ef6f3-5419-41e9-9a6d-832f9a921933)

AWS Global Infrastructure memiliki beberapa fitur berharga:

- Pertama, elastisdan dapat diskalakan. Ini berarti sumber daya dapat menyesuaikan dengan peningkatan atau penurunan kebutuhan kapasitas secara dinamis. Ini juga dapat dengan cepat menyesuaikan untuk mengakomodasi pertumbuhan.
- Kedua, infrastruktur initoleran terhadap kesalahan, yang berarti memiliki redundansi komponen bawaan yang memungkinkannya melanjutkan operasi meskipun komponen gagal.
- Terakhir, diperlukan sedikit atau tanpa intervensi manusia, sekaligus memberikan ketersediaan tinggidengan sedikit waktu henti.


# Kategori Layanan AWS
