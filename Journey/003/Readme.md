# Dasar-Dasar Harga

## Model Harga AWS

![Model Harga AWS](https://github.com/putrafa/linuxsysadmin/assets/121589476/ace83eca-0a4f-4873-b45b-9bb1e27aa23f)

Cara Membayar AWS:

- Bayar sesuai yang Anda gunakan
- Bayar lebih sedikit ketika Anda melakukan pemesanan
- Bayar lebih sedikit saat Anda menggunakan lebih banyak
- Bayar jauh lebih sedikit sering berkembangnya AWS

# Total Biaya Kepemilikan

![On Promise Cloud](https://github.com/putrafa/linuxsysadmin/assets/121589476/38b93e3b-823a-49fb-a0ba-9e2e80c811ce)

On-premise versus cloud adalah pertanyaan yang diajukan banyak bisnis. Perbedaan antara kedua opsi ini adalah bagaimana mereka di-deploy.

Infrastruktur on-premise diinstal secara on-premise pada komputer dan server milik perusahaan. Ada beberapa biaya tetap yang juga dikenal sebagai biaya modal, yang berkaitan dengan infrastruktur tradisional. Biaya modal meliputi fasilitas, perangkat keras, lisensi, dan staf pemeliharaan. Meningkatkan skala mahal dan menyita waktu. Menurunkan skala tidak mengurangi biaya tetap.

Infrastruktur cloud dibeli dari penyedia layanan yang membangun dan memelihara fasilitas, perangkat keras, serta staf pemeliharaan. Pelanggan membayar sesuai yang digunakan. Menaikkan atau menurunkan skala itu sederhana. Biaya mudah diperkirakan karena tergantung penggunaan layanan.

Sulit untuk membandingkan model pengiriman IT on-premise dengan AWS Cloud. Keduanya berbeda karena mereka menggunakan konsep dan istilah yang berbeda.Menggunakan IT on-premise melibatkan diskusi yang didasarkan pada biaya modal, siklus perencanaan yang panjang, dan beberapa komponen untuk membeli, membangun, mengelola, dan menyegarkan sumber daya dari waktu ke waktu.

Menggunakan AWS Cloud melibatkan diskusi tentang fleksibilitas, ketangkasan, dan biaya berbasis konsumsi.

![TCO](https://github.com/putrafa/linuxsysadmin/assets/121589476/3ed39ada-8609-496a-ab8d-56a20bf95ff9)

Anda dapat mengidentifikasi pilihan terbaik dengan membandingkan solusi on-premise dengan solusi cloud. Total Biaya Kepemilikan (atau TCO) adalah alat yang dapat digunakan untuk perbandingan ini. TCO adalah perkiraan keuangan yang ditujukan untuk membantu pembeli dan pemilik dalam menentukan biaya langsung dan tidak langsung dari suatu produk atau sistem. TCO meliputi biaya layanan, ditambah semua biaya terkait kepemilikan layanan.

![Pertimbangan TCO](https://github.com/putrafa/linuxsysadmin/assets/121589476/9ea7325f-3547-4b93-a9af-397227684a47)

![On Promise vs Semua yg di Cloud](https://github.com/putrafa/linuxsysadmin/assets/121589476/5483c0fd-74b0-4fc0-907f-4568eb1b36c4)

![On Promise vs Semua yg di Cloud](https://github.com/putrafa/linuxsysadmin/assets/121589476/b54f4d72-a70e-425a-8c3d-9fad4057df37)

![Kalkulator Simpel Bulanan AWS](https://github.com/putrafa/linuxsysadmin/assets/121589476/9149a67f-0885-4e40-806b-bec66dc7dda5)

![Kalkulator TCO AWS](https://github.com/putrafa/linuxsysadmin/assets/121589476/6001a410-1fc7-4e8d-bba3-8f2d74db499f)

![Pertimbangan Manfaat Tambahan](https://github.com/putrafa/linuxsysadmin/assets/121589476/216e8b92-fd8e-481c-9e37-b8baec6c09d0)

# AWS Organizations

## Introduction

![Logo AWS Organizations](https://github.com/putrafa/linuxsysadmin/assets/121589476/96600ce3-13c0-4894-8fc4-f0b794f89e5a)

AWS Organizations adalah layanan manajemen akun yang memungkinkan Anda menggabungkan beberapa akun AWS ke sebuahorganisasiyang Anda buat dan kelola secara terpusat. AWS Organizations meliputi tagihan terkonsolidasi dan kemampuan manajemen akun yang membantu Anda memenuhi anggaran, keamanan, dan kebutuhan kepatuhan bisnis Anda dengan lebih baik.

Manfaat utama AWS Organizations:
- Mengelola kebijakan akses secara terpusat di beberapa akun AWS
- Mengontrol akses ke layanan AWS
- Mengautomasi perbuatan dan pengelolaan akun AWS
- Tagihan terkonsolidasi di beberapa akun AWS

## Terminologi AWS Organizations

![Tirmonologi AWS Organizations](https://github.com/putrafa/linuxsysadmin/assets/121589476/bcfa59e1-c24e-4be9-bb0b-4e82f23a5a46)

Diagram menunjukkan organisasidasar atau rootyang terdiri dari tujuh akun yang disusun menjadi empat unit organisasi (atau OU). OU adalah kontainer untuk akun dalam root. OU juga dapat berisi OU lainnya. Struktur ini memungkinkan Anda membuat hierarki yang terlihat seperti pohon terbalik dengan root di bagian atasnya. Cabangnya terdiri dari OU turunan dan bergerak ke bawah sampai berakhir di akun yang terlihat seperti daun di pohon.

Ketika Anda melampirkan kebijakan ke salah satu node dalam hierarki, kebijakan tersebut akan turun dan memengaruhi semua cabang dan daun di bawahnya. Organisasi contoh ini memiliki beberapa kebijakan yang dilampirkan ke beberapa OU atau dilampirkan langsung ke akun. 

OU hanya dapat memiliki satu induk, dan untuk saat ini masing-masing akun juga hanya dapat menjadi anggota satu OU saja. Akun adalah akun AWS standar yang berisi sumber daya AWS Anda. Anda dapat melampirkan kebijakan ke akun untuk menerapkan kontrol hanya untuk satu akun tersebut.

## Fitur Utama dan Manfaat AWS Organizations


![Fitur Utama dan Manfaat AWS Organizations](https://github.com/putrafa/linuxsysadmin/assets/121589476/0547632c-e405-4e91-829c-d0b2e330e590)

AWS Organizations memungkinkan Anda untuk:

- Membuat service control policies (SCP) yang secara terpusat mengontrol penggunaan layanan AWS di beberapa akun AWS.

- Membuat grup akun dan kemudian melampirkan kebijakan ke dalam grup untuk memastikan kebijakan yang benar diterapkan di seluruh akun tersebut.

- Menyederhanakan pengelolaan akun menggunakan antarmuka pemrograman aplikasi (API)untuk mengautomasi pembuatan dan pengelolaan akun AWS baru.

- Menyederhanakan proses penagihan dengan menyiapkan metode pembayaran tunggal untuk semua akun AWS di organisasi Anda. Dengan tagihan terkonsolidasi, Anda dapat melihat tampilan tagihan terkonsolidasi yang dikeluarkan oleh semua akun Anda, dan Anda dapat memanfaatkan keuntungan harga dari penggunaan gabungan. Tagihan terkonsolidasi menyediakan lokasi pusat untuk mengelola penagihan di semua akun AWS Anda, dan kemampuan untuk mendapatkan keuntungan dari diskon volume.

## Keamanan dengan AWS Organizations

![Keamanan AWS Organizations](https://github.com/putrafa/linuxsysadmin/assets/121589476/6b755866-5d59-450d-83fa-8c77e34fb975)

## Penyiapan Organisasi

![Penyiapan Organisasi](https://github.com/putrafa/linuxsysadmin/assets/121589476/8295dbcf-50bd-41d9-8988-09b3b440663a)

- Langkah 1 adalah membuat organisasi Anda dengan akun AWS Anda saat ini sebagai akun master. Anda juga mengundang satu akun AWS untuk bergabung dengan organisasi Anda dan membuat akun lain sebagai akun anggota.

- Langkah 2 adalah membuat dua unit organisasi dalam organisasi baru Anda dan menempatkan akun anggota di OU tersebut.

- Langkah 3 adalah membuat service control policies yang memungkinkan Anda menerapkan batasan tindakan apa yang dapat didelegasikan kepada pengguna dan peran dalam akun anggota. Kebijakan kontrol layanan adalah jenis kebijakan kontrol organisasi.

- Langkah 4 adalah menguji kebijakan organisasi Anda. Masuk sebagai pengguna untuk masing-masing peran (seperti OU1 atau OU2) dan lihat bagaimana service control policies ini memengaruhi akses akun. Atau, Anda dapat menggunakan simulator kebijakan IAM untuk menguji dan memecahkan masalah IAM dan kebijakan berbasis sumber daya yang melekat pada pengguna, grup, atau IAM role di akun AWS Anda.

Batas AWS Organizations

![Batas AWS Organizations](https://github.com/putrafa/linuxsysadmin/assets/121589476/7bbb6a8f-e1f6-4cbd-96ce-1d01133449a1)

## Mengakses AWS Organizations

![Mengakses AWS Organizations](https://github.com/putrafa/linuxsysadmin/assets/121589476/48cb2987-0b90-4725-8916-63b1ce950e3e)

AWS Organizations dapat dikelola melalui antarmuka yang berbeda.

AWS Management Consoleadalah antarmuka berbasis browser yang dapat Anda gunakan untuk mengelola organisasi dan sumber daya AWS Anda. Anda dapat melakukan tugas apa pun di organisasi Anda dengan menggunakan konsol.

Alat AWS Command Line Interface (AWS CLI)memungkinkan Anda mengeluarkan perintah yang dikaitkan oleh perintah sistem Anda untuk menjalankan tugas AWS Organizations dan tugas AWS. Cara ini bisa lebih cepat dan lebih mudah daripada menggunakan konsol.

Anda juga dapat menggunakan kit pengembangan perangkat lunak (SDK) AWS untuk menangani tugas seperti menandatangani permintaan secara kriptografis, mengelola kesalahan, dan mencoba kembali permintaan secara otomatis.

AWS SDK terdiri dari beberapa library dan kode sampel untuk berbagai bahasa pemrograman dan platform seperti Java, Python, Ruby, NET, iOS, dan Android. 

API Kueri HTTPS AWS Organizationsakan memberi Anda akses terprogram ke AWS Organizations dan AWS. Anda dapat menggunakan API untuk mengeluarkan permintaan HTTPS secara langsung ke layanan. Ketika Anda menggunakan API HTTPS, Anda harus menyertakan kode untuk menandatangani permintaan secara digital dengan menggunakan kredensial Anda.

## Manajemen Penagihan dan Biaya AWS

![Manajemen Penagihan dan Biaya AWS](https://github.com/putrafa/linuxsysadmin/assets/121589476/9c487410-d794-45aa-b365-5952122797e5)

Manajemen Penagihan dan Biaya AWSadalah layanan yang Anda gunakan untuk membayar tagihan AWS, memantau penggunaan, dan membuat anggaran untuk biaya Anda. Manajemen Penagihan dan Biaya memungkinkan Anda memprakirakan dan mendapatkan gambaran yang lebih baik mengenai besarnya biaya dan penggunaan Anda di masa depan sehingga Anda dapat membuat rencana untuk ke depannya.

![Dasbor Penagihan AWS](https://github.com/putrafa/linuxsysadmin/assets/121589476/90ebf8d0-6685-4c92-a5f2-96cf8993491c)

Dasbor Penagihan AWS memungkinkan Anda melihat status pengeluaran AWS bulan ini sampai saat ini, dan mengidentifikasi layanan yang berkontribusi terhadap sebagian besar pengeluaran keseluruhan Anda, dan memahami tren biaya dengan baik.

Salah satu grafik yang terletak di dasbor adalah Ringkasan Pembelanjaan. Ringkasan Pembelanjaan menunjukkan jumlah pembelanjaan Anda bulan lalu, perkiraan biaya penggunaan AWS Anda untuk bulan ini sampai saat ini, dan prakiraan untuk kemungkinan pembelanjaan Anda bulan ini.

Grafik lain adalah Pembelanjaan Bulan Ini Sampai Saat ini berdasarkan Layanan, yang menunjukkan layanan teratas yang paling sering Anda gunakan dan proporsi biaya yang dikaitkan dengan layanan tersebut.

![Dasbor Penagihan AWS](https://github.com/putrafa/linuxsysadmin/assets/121589476/14941fa4-e1f5-456c-adf0-9377551978db)

![Alat Dasbor Penagihan](https://github.com/putrafa/linuxsysadmin/assets/121589476/285a7c10-d44c-49ad-b96b-c3c57cb44ad4)

Dari dasbor penagihan, Anda dapat mengakses beberapa alat manajemen biaya lainnya yang dapat Anda gunakan untuk memperkirakan dan merencanakan pengeluaran AWS Anda. Alat ini meliputi Tagihan AWS, AWS Cost Explorer, AWS Budgets, dan Laporan Penggunaan dan Biaya AWS.

![Tagihan Bulanan](https://github.com/putrafa/linuxsysadmin/assets/121589476/2308d865-be71-4164-bcd1-a7cbc6bf1bb2)

Halaman Tagihan AWSakan mencantumkan biaya yang dikenakan kepada Anda selama bulan lalu untuk setiap layanan AWS, dengan detail lebih lanjut berdasarkan Wilayah AWS dan akun terkait.

![Cost Explorer](https://github.com/putrafa/linuxsysadmin/assets/121589476/feeca938-85a5-40fb-8c9e-6b3866323f54)

Cost Explorer mencakup laporan default yang memvisualisasikan biaya dan penggunaan untuk layanan AWS Anda yang paling banyak memakan biaya. Laporan biaya operasional bulanan memberi Anda gambaran umum semua biaya Anda selama 3 bulan terakhir. Laporan ini juga menyediakan prakiraan untuk bulan mendatang dengan interval kepercayaan yang sesuai.

Cost Explorer adalah alat gratis yang memungkinkan Anda:

- Melihat grafik biaya Anda.
- Melihat data biaya selama 13 bulan terakhir.
- Memprakirakan banyaknya biaya yang mungkin Anda habiskan selama 3 bulan ke depan.
- Menemukan pola banyaknya biaya yang Anda habiskan untuk sumber daya AWS dari waktu ke waktu dan mengidentifikasi area masalah biaya.
- Mengidentifikasi layanan yang paling sering Anda gunakan.
- Melihat metrik, seperti Availability Zone yang memiliki lalu lintas paling banyak atau akun AWS tertaut yang paling banyak digunakan.

![AWS Budget](https://github.com/putrafa/linuxsysadmin/assets/121589476/c21232f5-6ac5-49b9-b40f-1cd4249c4102)

AWS Budgets menggunakan visualisasi biaya yang disediakan oleh Cost Explorer untuk menunjukkan status anggaran Anda dan untuk memprakirakan biaya Anda.

Anda juga dapat menggunakan AWS Budgets untuk membuat pemberitahuan saat Anda melampaui anggaran untuk bulan tersebut atau ketika perkiraan biaya melebihi anggaran Anda. Anggaran dapat dilacak pada tingkat bulanan, triwulanan, atau tahunan, dan Anda dapat menyesuaikan tanggal mulai dan akhir. Peringatan anggaran dapat dikirim melalui email atau melalui Amazon Simple Notification Service (Amazon SNS).

![Laporan Biaya AWS](https://github.com/putrafa/linuxsysadmin/assets/121589476/867fb0b1-4d17-4316-9977-0cc2fbe0935d)

Laporan Biaya dan Penggunaan AWSadalah lokasi tunggal untuk mengakses informasi yang komprehensif mengenai biaya dan penggunaan AWS Anda. Alat ini mencantumkan penggunaan untuk setiap kategori layanan yang digunakan oleh akun dan penggunanya dalam item baris per jam atau harian, dan setiap pajak yang Anda aktifkan untuk tujuan alokasi pajak.

# Dukungan Teknis

## AWS Suppport

![AWS Support](https://github.com/putrafa/linuxsysadmin/assets/121589476/8e6dbe79-b9bf-4dc9-a09e-4267009b19fe)

AWS Support dikembangkan untuk memberikan dukungan lengkap dan sumber daya yang tepat untuk membantu kesuksesan Anda. Kami ingin mendukung semua pelanggan kami, termasuk pelanggan yang mungkin bereksperimen dengan AWS, yaitu mereka yang mencari penggunaan produksi AWS, dan juga pelanggan yang menggunakan AWS sebagai sumber daya bisnis yang penting. AWS Support bervariasi berdasarkan jenis dukungan yang disediakan, tergantung pada kebutuhan dan tujuan pelanggan.

![AWS Support MAT](https://github.com/putrafa/linuxsysadmin/assets/121589476/fb0e3b22-b9b8-4495-a99b-a79399811361)

Dengan AWS, pelanggan dapat merencanakan, men-deploy, dan mengoptimalkan dengan percaya diri.

Jika Anda ingin bimbingan proaktif, AWS Support memiliki Manajer Akun Teknis (MAT)yang ditunjuk sebagai kontak utama pengguna. MAT dapat memberikan panduan, tinjauan arsitektur, dan komunikasi berkelanjutan yang terus menerus untuk memberi Anda informasi dan persiapan saat Anda merencanakan, men-deploy, dan mengoptimalkan solusi Anda.

Jika Anda ingin memastikan bahwa Anda mengikuti praktik terbaik untuk meningkatkan performa dan toleransi kesalahan di lingkungan AWS, AWS Support memiliki AWS Trusted Advisor. AWS Trusted Advisor seperti ahli cloud yang disesuaikan. Ini adalah sumber daya online yang memeriksa peluang untuk mengurangi pengeluaran bulanan dan meningkatkan produktivitas. 

Untuk bantuan akun, Support Conciergeadalah ahli penagihan dan akun yang akan memberikan analisis cepat dan efisien mengenai masalah penagihan dan akun. Concierge menangani semua pertanyaan tingkat penagihan dan akun nonteknis.

## Paket Support

![Paket Support](https://github.com/putrafa/linuxsysadmin/assets/121589476/220a9f90-19ef-486b-ac64-7e2dda9ded94)

AWS ingin Anda dapat merencanakan, men-deploy, dan mengoptimalkan dengan percaya diri. Kami telah mengembangkan rencana khusus untuk mendukung Anda, termasuk paket dukungan Basic, Developer, Business, dan Enterprise:

- Paket Basic Support, menawarkan:
  - Akses 7x24 jam ke layanan pelanggan, dokumentasi, whitepaper, dan forum dukungan.
  - Akses ke enam pemeriksaan Trusted Advisor inti.
  - Akses ke Personal Health Dashboard

- Paket Developer Support, menawarkan sumber daya bagi pelanggan yang menguji atau melakukan pengembangan awal di AWS, serta semua pelanggan yang:
  - Menginginkan akses ke panduan dan dukungan teknis.
  - Menjelajahi cara cepat untuk menggunakan AWS.
  - Menggunakan AWS untuk beban kerja atau aplikasi nonproduksi

- Paket Business Support, menawarkan sumber daya untuk pelanggan yang menjalankan beban kerja produksi di AWS dan semua pelanggan yang:
  - Menjalankan satu atau beberapa aplikasi di lingkungan produksi.
  - Mengaktifkan beberapa layanan, atau menggunakan layanan utama secara ekstensif.
  - Bergantung pada solusi bisnis mereka agar tersedia, dapat diskalakan, dan aman.
 
- Paket Enterprise Support, menawarkansumber daya untuk pelanggan yang menjalankan bisnis dan beban kerja yang sangat penting di AWS dan semua pelanggan yang ingin:
  - Berfokus pada manajemen proaktif untuk meningkatkan efisiensi dan ketersediaan.
  - Membangun dan mengoperasikan beban kerja yang mengikuti praktik terbaik AWS.
  - Menggunakan keahlian AWS untuk mendukung peluncuran dan migrasi.
  - Menggunakan Manajer Akun Teknis (MAT), yang menyediakan keahlian teknis untuk berbagai layanan AWS, serta memperoleh pemahaman detail tentang kasus penggunaan dan arsitektur teknologi Anda. Manajer Akun Teknis adalah kontak utama untuk kebutuhan dukungan yang sedang berjalan.

## Keparahan Kasus dan Waktu Respon

![Keparahan Kasus dan Waktu Respon](https://github.com/putrafa/linuxsysadmin/assets/121589476/8de4e9ac-31cc-40bf-980c-d99bf1c781ef)

Ada lima tingkat keparahanyang berbeda:

- Kritis Bisnis Anda berisiko. Fungsi aplikasi Anda yang sangat penting tidak tersedia.
- Mendesak Bisnis Anda terdampak secara signifikan. Fungsi penting aplikasi Anda tidak tersedia.
- Tinggi Fungsi penting aplikasi Anda terganggu atau terdegradasi.
- Normal Fungsi nonkritis aplikasi Anda berperilaku tidak normal atau Anda memiliki pertanyaan tentang pengembangan yang sensitif terhadap waktu.
- Rendah Anda memiliki pertanyaan tentang pengembangan umum atau Anda ingin meminta fitur.
