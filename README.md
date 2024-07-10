# Langkah 1: Persiapan Direktori dan File.
1.	Buat dua direktori: website-utama dan website-profil.
   <img width="426" alt="image" src="https://github.com/HanifDika/Responsi/assets/94159054/758410b2-691d-490a-8b23-bceb63703668">

Pembahasan :
Perintah ini digunakan untuk membuat direktori baru bernama website-utama dan pindah ke direktori tersebut.

2. Buat file index.html di dalam direktori website-utama.
 <img width="426" alt="image" src="https://github.com/HanifDika/Responsi/assets/94159054/26f32f81-fe24-4b9c-85c7-ff2eb93d6fbe">

Pembahasan :
Perintah ini membuka editor teks nano untuk membuat dan mengedit file index.html di dalam direktori website-utama.

Isi file index.html dengan konten berikut:

 <img width="426" alt="image" src="https://github.com/HanifDika/Responsi/assets/94159054/38c46175-9901-473e-92bc-224002934d6d">

Pembahasan :
Ini adalah isi dari file index.html yang mencakup informasi pribadi dan tautan ke halaman profil.

3.	Letakkan file gambar profil (misalnya foto.jpg) di dalam direktori website-profil.
 <img width="426" alt="image" src="https://github.com/HanifDika/Responsi/assets/94159054/b18c6418-1d35-4104-9de5-eed48a427efc">

Pembahasan :
Perintah ini mengunduh gambar profil dan menyimpannya sebagai foto.jpg di direktori website-profil.

4.	Buat file index.html di dalam direktori website-profil.
 <img width="429" alt="image" src="https://github.com/HanifDika/Responsi/assets/94159054/00775ac9-2ff1-42aa-b743-6d89b9e2b4da">

Pembahasan :
Perintah ini membuka editor teks nano untuk membuat dan mengedit file index.html di dalam direktori website-profil.

5.	Isi file index.html dengan konten berikut:
 <img width="430" alt="image" src="https://github.com/HanifDika/Responsi/assets/94159054/184a28eb-fcb4-421a-b8fd-be17d32cf68a">

Pembahasan :
Ini adalah isi dari file index.html yang mencakup informasi pribadi dan gambar profil.

# Langkah 2: Docker Network
1.	Buat jaringan Docker dengan nama my-ajeng-pratiwi-network.
 <img width="430" alt="image" src="https://github.com/HanifDika/Responsi/assets/94159054/62b27ca0-4ea7-4618-ba3f-f8a1aae72678">

Pembahasan :
Perintah ini membuat jaringan Docker baru dengan nama my-hanif-farhandika-network.

# Langkah 3: Dockerfile dan Image
Dockerfile untuk Website Utama
1.	Buat file Dockerfile di dalam direktori website-utama.
   
 <img width="429" alt="image" src="https://github.com/HanifDika/Responsi/assets/94159054/d6bcfd2c-2441-4865-b9e1-27513a42574e">

Pembahasan :
Perintah ini membuka editor teks nano untuk membuat dan mengedit file Dockerfile di dalam direktori website-utama.

2.	Isi dengan konten berikut:
 <img width="253" alt="image" src="https://github.com/HanifDika/Responsi/assets/94159054/e38099be-4f51-45f2-89ab-f004f0690556">

Pembahasan :
Ini adalah Dockerfile untuk website utama yang menggunakan image dasar Nginx dan menyalin file index.html ke direktori yang sesuai di dalam container Nginx.


# Dockerfile untuk Website Profil
1.	Buat file Dockerfile di dalam direktori website-profil.
 
 
 ![image](https://github.com/HanifDika/Responsi/assets/94159054/a7c456b2-ce08-4dfb-a7bf-9cf411cc2ac0)


Pembahasan :
Perintah ini membuka editor teks nano untuk membuat dan mengedit file Dockerfile di dalam direktori website-profil.

2.	Isi dengan konten berikut:
 <img width="270" alt="image" src="https://github.com/HanifDika/Responsi/assets/94159054/a343493c-a360-461c-b2cb-1cb2cd94a9ea">

Pembahasan :
ni adalah Dockerfile untuk website profil yang menggunakan image dasar Nginx dan menyalin file foto.jpg ke direktori yang sesuai di dalam container Nginx.

# Langkah 4: Build Image
Bangun dua image Docker dari Dockerfile yang sudah dibuat.
1.	Build image untuk website utama:
 <img width="422" alt="image" src="https://github.com/HanifDika/Responsi/assets/94159054/9c9be420-6261-4e7d-b26f-90d6f4a01d16">

Pembahasan :
Perintah ini membangun image Docker untuk website utama dengan tag website-utama.

2.	Build image untuk website profil:
 <img width="422" alt="image" src="https://github.com/HanifDika/Responsi/assets/94159054/6bdff079-66c1-4e1f-91d6-ed22468638ea">

Pembahasan :
Perintah ini membangun image Docker untuk website profil dengan tag website-profil.	

# Langkah 5: Docker Volume (Opsional)
1.	Buat volume bernama profile-images.
   
  ![image](https://github.com/HanifDika/Responsi/assets/94159054/5527d80f-26c6-4798-8888-39af21539c39)

Pembahasan :
Perintah ini membuat volume Docker baru dengan nama profile-images.

# Langkah 6: Menjalankan Container
1.	Jalankan container untuk website utama:
 <img width="422" alt="image" src="https://github.com/HanifDika/Responsi/assets/94159054/47e684c9-c059-43b1-9155-dddb47ff3beb">

Pembahasan :
Perintah ini menjalankan container Docker untuk website utama dalam mode detached (-d), dengan nama website-utama, menggunakan jaringan Docker my-hanif-farhandika-network, dan memetakan port 8080 di host ke port 80 di container.

2.	Jalankan container untuk website profil:
 <img width="422" alt="image" src="https://github.com/HanifDika/Responsi/assets/94159054/5c35b005-6e2e-4872-9b73-644f29cbe52f">

Pembahasan :
Perintah ini menjalankan container Docker untuk website profil dalam mode detached (-d), dengan nama website-profil, menggunakan jaringan Docker my-hanif-farhandika-network, dan memetakan port 8081 di host ke port 80 di container.
<img width="451" alt="image" src="https://github.com/HanifDika/Responsi/assets/94159054/c8c01c70-181e-46cc-85b4-cca31ba105d0">


 <img width="451" alt="image" src="https://github.com/HanifDika/Responsi/assets/94159054/97daa60e-238a-4876-9df7-100b1bc58820">




 

# Kesimpulan :
Laporan ini menjelaskan langkah-langkah mendetail untuk membuat dan menjalankan dua situs web sederhana menggunakan Docker. Dimulai dengan persiapan direktori dan file, kemudian pembuatan jaringan Docker, dan dilanjutkan dengan pembuatan Dockerfile untuk setiap situs. Setelah membangun image Docker dari Dockerfile tersebut, kedua kontainer dijalankan menggunakan jaringan yang sama dengan pemetaan port yang berbeda. Hasil akhirnya adalah dua situs web yang dapat diakses secara terpisah melalui port 8080 dan 8081, menunjukkan kemampuan Docker dalam mengisolasi dan mengelola aplikasi web secara efisien.
