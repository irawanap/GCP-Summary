### GCP-Summary

Pengantar ke Layanan Komputasi GCP
Layanan komputasi merupakan komponen terpenting dalam menjalankan sebuah aplikasi. Setiap aplikasi memerlukan mesin yang memproses dan menjalankan programnya. Google Cloud menyediakan beberapa opsi layanan komputasi yang bisa digunakan sesuai dengan kebutuhan. Pada modul ini kita akan mempelajari layanan-layanan komputasi dari Google Cloud tersebut, antara lain:

*Compute Engine*
*Google Kubernetes Engine*
*Cloud Run*
*App Engine*
*Cloud Functions*


# Compute Engine
Layanan ini menyediakan virtual machine (VM) yang aman dan customizable (dapat dikustomisasi). VM instance yang Anda buat akan berjalan di data center Google yang terhubung dengan jaringan fiber di seluruh dunia. 

Compute Engine menawarkan beberapa fitur seperti berikut.

Virtual machine dengan kinerja pemrosesan dan penyimpanan yang tinggi.
Auto scaling (penyesuaian kapasitas otomatis) dan load balancer (pembagian beban) untuk VM yang bersifat homogen/identik.
Akses langsung ke GPU yang bisa digunakan untuk mempercepat kinerja.
Dukungan berbagai versi dari sistem operasi seperti Linux dan Windows.
Preemptible VM (instance yang dapat terhenti kapan saja tergantung pada system event) yang dapat dibuat dan dijalankan dengan harga yang lebih rendah daripada VM normal.
Compute Engine cocok digunakan bagi Anda yang memerlukan kontrol penuh atas infrastruktur dan akses langsung ke hardware seperti GPU dan SSD. Anda juga dapat memindahkan data pada data center atau colocation menuju cloud dengan menggunakan layanan ini.



# Google Kubernetes Engine
Google Kubernetes Engine menyediakan environment yang terkelola untuk deploy, manage, dan scale containerized application menggunakan infrastruktur Google. Google Kubernetes Engine environment terdiri dari beberapa mesin (khususnya, Compute Engine instance) yang dikelompokkan bersama untuk membentuk sebuah Kubernetes cluster.

Sebagaimana namanya, Google Kubernetes Engine cluster ditenagai oleh sistem manajemen cluster open source yang disebut Kubernetes. Kubernetes menyediakan mekanisme untuk berinteraksi dengan sejumlah mesin yang disebut cluster. Anda dapat menggunakan baris perintah untuk berinteraksi dengan Kubernetes, seperti men-deploy dan mengelola aplikasi, melakukan tugas administrasi, menetapkan kebijakan, dan memantau kesehatan pod. 



# Cloud Run
Cloud Run adalah layanan komputasi terkelola dari Google yang memungkinkan Anda untuk menjalankan container dengan mudah di infrastrukturnya Google yang terkenal sangat scalable. 

Berbeda dengan layanan Google Kubernetes Engine (yang kita bahas di materi sebelumnya) di mana kita harus meluncurkan cluster, membuat deployment, mengelola pod, dan komponen Kubernetes lainnnya untuk menjalankan aplikasi dalam container (containerized application), Cloud Run menghilangkan semua kerumitan tersebut sehingga memudahkan Anda sebagai Developer untuk men-deploy aplikasi di Google Cloud.



# App Engine
App Engine pertama kali diluncurkan pada tanggal 7 April 2008. Ini adalah sebuah Platform-as-a-Service (PaaS) dari Google yang menyediakan layanan untuk meng-hosting aplikasi dengan mudah. 

Dengan App Engine, kita hanya perlu fokus dalam mengembangkan aplikasi dan mengunggahnya ke App Engine. Infrastruktur yang digunakan untuk menjalankan aplikasi sepenuhnya menjadi tanggung jawab Google. App Engine juga akan secara otomatis menaikkan sumber daya (scale up) jika terjadi lonjakan jumlah pengguna dan mengurangi sumber daya (scale down) sesuai dengan jumlah pengguna.

 

# Cloud Functions
Cloud Functions adalah sebuah execution environment (lingkungan pengeksekusian kode) bermodel serverless (nirserver alias pengguna tak perlu membuat dan mengelola server) yang digunakan untuk membangun aplikasi atau menghubungkan antar layanan Google Cloud.

Sama seperti App Engine atau Cloud Run, Cloud Functions memiliki model komputasi serverless. Namun, Cloud Functions memiliki ukuran lebih kecil karena yang kita deploy adalah kode logika yang berada di dalam function (fungsi), bukan aplikasi besar seperti App Engine atau Cloud Run. Karena Cloud Functions bersifat serverless, kita tidak perlu melakukan pengaturan terhadap infrastruktur atau server di baliknya. Layanan semacam ini juga biasa disebut sebagai Function as a Service (FaaS).

