Nama    : Monica Gloria Damanik

NPM     : 2206082442

Kelas   : PBP B

Tautan Adaptable : https://inventory-monica.adaptable.app
Tautan Github    : https://github.com/monicaa37/my-project1.git

1. Jelaskan bagaimana cara kamu mengimplementasikan checklist di atas secara step-by-step.
   jawab : 

   **TAHAP 1 : MEMBUAT SEBUAT PROYEK DJANGO BARU**

      a. Membuat Direktori dan Mengaktifkan Virtual Environment
      - Pertama, buat direktori baru di lokasi yang Anda inginkan untuk proyek Anda. Anda dapat melakukannya melalui terminal atau dengan menggunakan file explorer. Setelah membuat direktori, masuk ke dalamnya dengan perintah cd.
      - Sekarang, Anda perlu membuat virtual environment di dalam direktori proyek Anda.
      - Gunakan perintah berikut untuk membuat venv. Perlu mengaktifkannya dengan perintah venv\Scripts\activate.
     
     b. Menyiapkan Dependencies dan Membuat Proyek Django
      - Di dalam direktori yang sama, buat berkas requirements.txt dan tambahkan beberapa dependencies.
      - Lalu, Pasang dependencies dengan perintah berikut. Jangan lupa jalankan virtual environment terlebih dahulu sebelum menjalankan perintah berikut: pip install -r requirements.txt
      - Kemudian, buat proyek Django sesuai yang diinginkan dengan perintah berikut: django-admin startproject (nama proyek) 
     
     c. Konfigurasi Proyek dan Menjalankan Server
      - Tambahkan tanda (*) pada ALLOWED_HOSTS di settings.py untuk keperluan deployment.
      - Jalankan server Django dengan perintah: python manage.py runserver.
      - Kemudian, nonaktifkan virtual environment dengan perintah: deactivate 

    **TAHAP 2 : MEMBUAT APLIKASI DENGAN NAMA MAIN PADA PROYEK TERSEBUT**

       a. Pastikan Anda sudah berada dalam direktori proyek Django Anda.

       b. Jalankan perintah berikut untuk membuat aplikasi "main": python manage.py startapp main .

       c. Setelah membuat aplikasi "main," Anda perlu mendaftarkannya ke dalam proyek Anda.
       
       d. Buka file nama_proyek/settings.py dan temukan variabel INSTALLED_APPS. Tambahkan nama aplikasi "main" ke dalam daftar aplikasi yang terdaftar.

2. Buatlah bagan yang berisi request client ke web aplikasi berbasis Django beserta responnya dan jelaskan pada bagan tersebut kaitan antara urls.py, views.py, models.py, dan berkas html.
jawab : ![Bagan Request Monica](Request_Bagan.png)

3. Jelaskan mengapa kita menggunakan virtual environment? Apakah kita tetap dapat membuat aplikasi web berbasis Django tanpa menggunakan virtual environment?
jawab : Virtual environment ini berguna untuk mengisolasi package serta dependencies dari aplikasi sehingga tidak bertabrakan dengan versi lain yang ada pada komputermu. Untuk membuat aplikasi web, anda masih dapat membuat aplikasi web berbasis Django tanpa menggunakan virtual environment, tetapi tidak disarankan. 
   
4. Jelaskan apakah itu MVC, MVT, MVVM dan perbedaan dari ketiganya.
jawab : 
    a. Model View Controller atau yang dapat disingkat MVC adalah sebuah pola arsitektur dalam membuat sebuah aplikasi dengan cara memisahkan kode menjadi tiga bagian yang terdiri dari:
      * Model --> Bagian yang bertugas untuk menyiapkan, mengatur, memanipulasi, dan mengorganisasikan data yang ada di database.
      * View --> Bagian yang bertugas untuk menampilkan informasi dalam bentuk Graphical User Interface (GUI).
      * Controller --> Bagian yang bertugas untuk menghubungkan serta mengatur model dan view agar dapat saling terhubung.
        
   b. Model View Template
      * Model: Sama seperti dalam MVC, model mengurus data dan logika bisnis.
      * View: Bertanggung jawab untuk tampilan dan presentasi data, mirip dengan View dalam MVC.
      * Template: Template dalam MVT adalah elemen yang berbeda. Ini adalah bagian yang merender tampilan dalam aplikasi web         Django. Template menggantikan peran Controller dalam MVC, karena sebagian besar logika pengendalian berada dalam             framework Django itu sendiri.

   c. Model View - View Model adalah arsitektur yang digunakan dalam pengembangan aplikasi berbasis klien, khususnya dalam pengembangan aplikasi web menggunakan kerangka kerja JavaScript. 
    * Model: Ini adalah representasi data dan logika bisnis, sama seperti dalam MVC dan MVT.
    * View: Bertanggung jawab untuk tampilan dan presentasi data, mirip dengan View dalam MVC dan MVT.
    * ViewModel: Ini adalah komponen yang memisahkan Model dari View. ViewModel mengambil data dari Model dan mempersiapkannya untuk ditampilkan di View. ViewModel juga mengelola tindakan pengguna dan berfungsi sebagai penghubung antara Model dan View. 
    
      Perbedaan ketiganya adalah dalam bagaimana komponen-komponen ini berinteraksi dan siapa yang bertanggung jawab untuk apa. MVC dan MVT adalah konsep yang lebih tua dan sering digunakan dalam pengembangan aplikasi web dengan back-end yang kuat, sedangkan MVVM adalah pendekatan yang lebih modern untuk pengembangan aplikasi berbasis klien dengan fokus pada pemisahan antara tampilan dan logika bisnis.
   