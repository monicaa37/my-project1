Nama    : Monica Gloria Damanik

NPM     : 2206082442

Kelas   : PBP B

Tautan Adaptable : https://inventory-monica.adaptable.app
Tautan Github    : https://github.com/monicaa37/my-project1.git

------------------------------------- TUGAS 2 -------------------------------------
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

      - Pastikan Anda sudah berada dalam direktori proyek Django Anda.

      - Jalankan perintah berikut untuk membuat aplikasi "main": python manage.py startapp main .

      - Setelah membuat aplikasi "main," Anda perlu mendaftarkannya ke dalam proyek Anda.

      - Buka file nama_proyek/settings.py dan temukan variabel INSTALLED_APPS. Tambahkan nama aplikasi "main" ke dalam daftar aplikasi yang terdaftar.

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
   

-------------------------------------- TUGAS 3 ------------------------------------
1. Apa perbedaan antara form POST dan form GET dalam Django?
ans : 
- Method GET

a. Jangan gunakan GET bila kita ingin membuat form untuk data yang sensitif/ mempunyai privasi, misalnya username,password (karena akan tampil di URL)
b. Sebaliknya gunakan GET untuk data dengan informasi yang umum, seperti nama,email atau lainnya
c. Gunakan method GET untuk data yang relatif kecil

- Method POST

a. Gunakan method POST untuk jenis informasi data pribadi misalnya username dan password ,karena lebih aman dibandingkan method GET dan data tidak akan tampil di URL
b. Gunakan method POST untuk data yang relatif besar.

2. Apa perbedaan utama antara XML, JSON, dan HTML dalam konteks pengiriman data?
ans : 
- XML (eXtensible Markup Language): Digunakan untuk menyimpan dan mengirim data terstruktur dengan menggunakan tag pembuka dan penutup. Fleksibel dan kuat, cocok untuk data yang sangat terstruktur.

- JSON (JavaScript Object Notation): Digunakan untuk pertukaran data yang ringan, menggunakan sintaks objek dan array mirip JavaScript. Sederhana dan mudah dibaca, cocok untuk data sederhana.

- HTML (HyperText Markup Language): Bahasa markup untuk membuat tampilan halaman web. Digunakan untuk mendefinisikan struktur dan konten halaman web, bukan untuk pertukaran data.

3. Mengapa JSON sering digunakan dalam pertukaran data antara aplikasi web modern?

ans : 
JSON sering digunakan dalam aplikasi web modern karena ringan, mudah dibaca, mendukung berbagai struktur data, independen dari bahasa, efisien dalam penggunaan bandwidth, mendukung RESTful APIs, dan memiliki dukungan luas.

4. Jelaskan bagaimana cara kamu mengimplementasikan checklist di atas secara step-by-step

ans : 
- Membuat Input Form:

   a. Buat model objek yang ingin Anda tambahkan.
   b. Buat form Django untuk model tersebut di forms.py.

- Migrasi Database:

   a. Buat dan terapkan migrasi untuk mengaktifkan model di database dengan perintah makemigrations dan migrate.

- Membuat 5 Fungsi Views:

Buat views untuk:
   a. Menambahkan objek dengan form input.
   b. Melihat objek dalam format HTML.
   c. Melihat objek dalam format XML.
   d. Melihat objek dalam format JSON.
   e. Melihat objek berdasarkan ID dalam format XML dan JSON.

- Membuat Template HTML:

   a. Buat file HTML untuk tampilan objek dan form input.

- Mengatur URL Routing:

   a. Tentukan URL untuk setiap view di file urls.py aplikasi Anda.

Dengan langkah-langkah ini, Anda akan memiliki aplikasi Django yang memungkinkan pengguna untuk menambahkan objek dan melihatnya dalam berbagai format. Pastikan untuk menyesuaikan model, form, dan template sesuai kebutuhan aplikasi Anda.

hasil screenshot postman : 
1. json 
![screenshot json](images/json.png)

2. json id
![screenshot json id](images/json_id.png)

3. xml 
![screenshot xml](images/xml.png)

4. xml id 
![screenshot xml id](images/xml_id.png)

5. html 
![screenshot html](images/html.png)