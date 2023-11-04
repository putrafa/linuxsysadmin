# Pengantar Komputasi Cloud

## Introduction

![Apa Itu Komputasi Cloud](https://github.com/putrafa/linuxsysadmin/assets/121589476/516b440b-3218-4974-9a43-53f6cb9b3e67)

Apa arti Komputasi Cloud?

Komputasi Cloud adalah pengiriman sesuai permintaan untuk daya komputasi, basis data, penyimpanan, aplikasi, dan sumber daya IT lain melalui internet dengan harga sesuai pemakaian. Sumber daya ini berjalan pada server komputer yang terletak di pusat data yang besar di lokasi yang berbeda di seluruh dunia. Saat Anda menggunakan penyedia layanan cloud seperti AWS, penyedia layanan itu memiliki komputer yang Anda gunakan. Sumber daya ini dapat digunakan bersama seperti blok bangunan untuk membangun solusi yang membantu memenuhi tujuan bisnis dan memenuhi persyaratan teknologi.

## Infrastruktur Sebagai Perangkat Lunak

Komputasi cloud memungkinkan Anda berhenti menganggap infrastruktur Anda sebagai perangkat keras, dan sebaliknya menganggapnya (dan menggunakannya) sebagai perangkat lunak. Jadi apa artinya?

![Model Komputasi Tradisional](https://github.com/putrafa/linuxsysadmin/assets/121589476/ddbefaec-1446-4411-b4cc-7d4278d8351c)

Dalam model komputasi tradisional, infrastruktur dianggap sebagai perangkat keras. Solusi perangkat keras itu bersifat fisik, yang berarti mereka memerlukan ruang, staf, keamanan fisik, perencanaan, dan biaya modal.

![Model Komputasi Tradisional](https://github.com/putrafa/linuxsysadmin/assets/121589476/b0f750f4-8a72-4320-a1a5-6156773dd5ee)

Sebaliknya, komputasi cloud memungkinkan Anda menganggap infrastruktur Anda sebagai perangkat lunak. Solusi perangkat lunak bersifat fleksibel. Anda dapat memilih layanan cloud yang paling sesuai dengan kebutuhan, menyediakan dan membatalkan sumber daya tersebut sesuai permintaan, dan membayar apa yang Anda gunakan. Anda dapat menaikkan atau menurunkan skala sumber daya secara elastis dan otomatis. Dengan model komputasi cloud, Anda dapat memperlakukan sumber daya sebagai sementara dan sekali pakai. Fleksibilitas yang ditawarkan komputasi cloud memungkinkan bisnis mengimplementasikan solusi baru dengan cepat dan dengan biaya di muka yang rendah.

## Model Layanan Cloud

![Model Layanan Cloud](https://github.com/putrafa/linuxsysadmin/assets/121589476/69dd84da-eff6-406e-87ca-8d0205340abe)

Ada tiga model layanan cloud utama. Setiap model mewakili bagian yang berbeda dari tumpukan komputasi cloud dan memberikan Anda tingkat kontrol yang berbeda atas sumber daya IT Anda:

- Infrastructure as a service (IaaS)

Layanan dalam kategori ini adalah blok bangunan dasar untuk IT cloud dan biasanya menyediakan akses ke fitur jaringan, komputer (virtual atau pada perangkat keras khusus), dan ruang penyimpanan data. IaaS memberikan tingkat fleksibilitas dan kontrol pengelolaan tertinggi atas sumber daya IT Anda. Ini adalah hal yang paling mirip dengan sumber daya IT yang banyak dikenal oleh departemen dan developer IT saat ini.

- Platform as a Service (PaaS)

Layanan dalam kategori ini menghilangkan kebutuhan organisasi untuk mengelola infrastruktur dasarnya (biasanya perangkat keras dan sistem operasi), serta memungkinkan Anda untuk fokus pada deployment dan pengelolaan aplikasi Anda.

- Software as a Service (SaaS)

Layanan dalam kategori ini memberikan Anda produk lengkap yang dijalankan dan dikelola oleh penyedia layanan. Dalam kebanyakan kasus, software as a servicemengacu pada aplikasi pengguna akhir. Dengan penawaran SaaS, Anda tidak perlu lagi memikirkan cara memelihara layanan atau cara mengelola infrastruktur dasar. Anda hanyaperlu memikirkan cara bagaimana Anda berencana untuk menggunakan perangkat lunak tertentu. Contoh umum aplikasi SaaS adalah email berbasis web yang dapat Anda gunakan untuk mengirim dan menerima email tanpa mengelola penambahan fitur ke produk email, atau memeliharaserver dan sistem operasi tempat program email dijalankan.

## Model Deployment 

![Model Layanan Cloud](https://github.com/putrafa/linuxsysadmin/assets/121589476/cb93b08a-ef27-4d58-ac21-c364b9630cd8)

Ada tiga model deployment komputasi cloud utama, yang mewakili lingkungan cloud tempat aplikasi Anda dapat di-deploy:

- Cloud

Aplikasi berbasis cloud sepenuhnya diterapkan di cloud dan semua bagian aplikasi yang berjalan di cloud. Aplikasi di cloud telah dibuat di cloud atau telah dimigrasikan dari infrastruktur yang ada untuk mengambil manfaat komputasi cloud. Aplikasi berbasis cloud dapat dibangun pada bagian infrastruktur tingkat rendah atau dapat menggunakan layanan tingkat yang lebih tinggi yang menyediakan pemisahan dari persyaratan manajemen, arsitektur, dan penskalaan infrastruktur inti.

- Hybird

Deployment hybrid adalah cara untuk menghubungkan infrastruktur dan aplikasi antara sumber daya berbasis cloud dan sumber daya yang ada yang tidak terletak di cloud. Metode deployment hybrid yang paling umum adalah antara cloud dan infrastruktur on-premise yang ada. Model ini memungkinkan organisasi untuk memperluas dan menumbuhkan infrastruktur mereka ke cloud sambil menghubungkan sumber daya cloud ke sistem internal.

- On premise

Men-deploy sumber daya on-premise, dengan menggunakan alat manajemen sumber daya dan virtualisasi, kadang-kadang disebut cloud privat. Deployment on-premise tidak memberikan banyak manfaat komputasi cloud, deployment ini terkadang dicari karena kemampuannya untuk menyediakan sumber daya khusus. Dalam banyak kasus, model deployment ini sama seperti infrastruktur IT lama, tapi itu juga menggunakan manajemen aplikasi dan teknologi virtualisasi untukmeningkatkan pemanfaatan sumber daya.

## Kesamaan Antara AWS dan IT Tradisional

- Grup keamanan AWS, access control list jaringan (ACL jaringan), dan AWS Identity and Access Management (IAM) mirip dengan firewall, access control list (ACL), dan administrator.

- Elastic Load Balancing dan Amazon Virtual Private Cloud (Amazon VPC) mirip dengan perute, pipeline jaringan, dan switch.

- Amazon Machine Image (AMI) dan instans Amazon Elastic Compute Cloud (Amazon EC2) mirip dengan server on-premise.

- Amazon Elastic Block Store (Amazon EBS), Amazon Elastic File System (Amazon EFS), Amazon Simple Storage Service (Amazon S3), dan Amazon Relational Database Service (Amazon RDS) mirip dengan penyimpanan terpasang langsung (DAS), jaringan area penyimpanan (SAN), penyimpanan terpasang jaringan (NAS), dan layanan manajemen basis data relasional (RDBMS).

  
