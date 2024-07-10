Langkah 1: Persiapan Direktori dan File.
1.	Buat dua direktori: website-utama dan website-profil.
   
Pembahasan :
Perintah ini digunakan untuk membuat direktori baru bernama website-utama dan pindah ke direktori tersebut.

3.	Buat file index.html di dalam direktori website-utama.
 
Pembahasan :
Perintah ini membuka editor teks nano untuk membuat dan mengedit file index.html di dalam direktori website-utama.

Isi file index.html dengan konten berikut:
 
Pembahasan :
Ini adalah isi dari file index.html yang mencakup informasi pribadi dan tautan ke halaman profil.

3.	Letakkan file gambar profil (misalnya foto.jpg) di dalam direktori website-profil.
 
Pembahasan :
Perintah ini mengunduh gambar profil dan menyimpannya sebagai foto.jpg di direktori website-profil.

4.	Buat file index.html di dalam direktori website-profil.
 
Pembahasan :
Perintah ini membuka editor teks nano untuk membuat dan mengedit file index.html di dalam direktori website-profil.

5.	Isi file index.html dengan konten berikut:
 
Pembahasan :
Ini adalah isi dari file index.html yang mencakup informasi pribadi dan gambar profil.

Langkah 2: Docker Network
1.	Buat jaringan Docker dengan nama my-ajeng-pratiwi-network.
 
Pembahasan :
Perintah ini membuat jaringan Docker baru dengan nama my-hanif-farhandika-network.

Langkah 3: Dockerfile dan Image
Dockerfile untuk Website Utama
1.	Buat file Dockerfile di dalam direktori website-utama.
 
Pembahasan :
Perintah ini membuka editor teks nano untuk membuat dan mengedit file Dockerfile di dalam direktori website-utama.

2.	Isi dengan konten berikut:
 
Pembahasan :
Ini adalah Dockerfile untuk website utama yang menggunakan image dasar Nginx dan menyalin file index.html ke direktori yang sesuai di dalam container Nginx.


Dockerfile untuk Website Profil
1.	Buat file Dockerfile di dalam direktori website-profil.
 
Pembahasan :
Perintah ini membuka editor teks nano untuk membuat dan mengedit file Dockerfile di dalam direktori website-profil.

2.	Isi dengan konten berikut:
 
Pembahasan :
ni adalah Dockerfile untuk website profil yang menggunakan image dasar Nginx dan menyalin file foto.jpg ke direktori yang sesuai di dalam container Nginx.

Langkah 4: Build Image
Bangun dua image Docker dari Dockerfile yang sudah dibuat.
1.	Build image untuk website utama:
 
Pembahasan :
Perintah ini membangun image Docker untuk website utama dengan tag website-utama.

2.	Build image untuk website profil:
 
Pembahasan :
Perintah ini membangun image Docker untuk website profil dengan tag website-profil.	

Langkah 5: Docker Volume (Opsional)
1.	Buat volume bernama profile-images.
 
Pembahasan :
Perintah ini membuat volume Docker baru dengan nama profile-images.

Langkah 6: Menjalankan Container
1.	Jalankan container untuk website utama:
 
Pembahasan :
Perintah ini menjalankan container Docker untuk website utama dalam mode detached (-d), dengan nama website-utama, menggunakan jaringan Docker my-hanif-farhandika-network, dan memetakan port 8080 di host ke port 80 di container.

2.	Jalankan container untuk website profil:
 
Pembahasan :
Perintah ini menjalankan container Docker untuk website profil dalam mode detached (-d), dengan nama website-profil, menggunakan jaringan Docker my-hanif-farhandika-network, dan memetakan port 8081 di host ke port 80 di container.


 



 

Kesimpulan :
Laporan ini menjelaskan langkah-langkah mendetail untuk membuat dan menjalankan dua situs web sederhana menggunakan Docker. Dimulai dengan persiapan direktori dan file, kemudian pembuatan jaringan Docker, dan dilanjutkan dengan pembuatan Dockerfile untuk setiap situs. Setelah membangun image Docker dari Dockerfile tersebut, kedua kontainer dijalankan menggunakan jaringan yang sama dengan pemetaan port yang berbeda. Hasil akhirnya adalah dua situs web yang dapat diakses secara terpisah melalui port 8080 dan 8081, menunjukkan kemampuan Docker dalam mengisolasi dan mengelola aplikasi web secara efisien.






















<img width="429" alt="image" src="https://github.com/HanifDika/Responsi/assets/94159054/6375012e-95cd-4907-8a36-b96649f9ecc9">
