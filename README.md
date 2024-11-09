# Rent_Car-Laravel

Berikut adalah penjelasan tentang aplikasi Rent_Car :
Teknologi Backend:
	1	PHP (>= 7.4): Aplikasi ini dibangun menggunakan PHP dengan versi minimal 7.4. Ini diperlukan untuk menjalankan Laravel 8.4.
	2	Laravel 8.4: Laravel adalah framework PHP yang kuat untuk pengembangan aplikasi web secara cepat. Laravel mempermudah tugas-tugas web umum seperti routing, autentikasi, sesi, caching, dan migrasi basis data.
	3	Livewire: Livewire adalah framework full-stack yang memungkinkan Anda membangun antarmuka dinamis di Laravel tanpa meninggalkan kenyamanan Laravel. Ini digunakan untuk menangani pembaruan UI real-time tanpa menulis banyak JavaScript.
Teknologi Frontend:
	1	Jetstream: Jetstream adalah paket Laravel yang menyediakan titik awal yang kuat untuk membangun aplikasi berbasis Laravel dengan fitur autentikasi, manajemen sesi, dan lainnya. Jetstream mencakup fitur-fitur seperti registrasi, login, verifikasi email, autentikasi dua faktor, dll. Jetstream menggunakan Livewire atau Inertia.js untuk interaksi frontend.
	2	Tailwind CSS: Framework CSS utility-first yang digunakan untuk membuat desain kustom dengan cepat. Tailwind CSS digunakan di frontend untuk menata komponen dan membangun layout responsif.
	3	Alpine.js (mungkin digunakan): Jika digunakan bersama Livewire, Alpine.js adalah framework JavaScript minimalis yang membantu membuat komponen UI interaktif.
Basis Data:
	1	MySQL: MySQL digunakan sebagai basis data relasional untuk menyimpan data aplikasi, termasuk profil pengguna, tawaran, umpan balik, dan ulasan.
Alat Tambahan:
	1	Composer: Composer adalah manajer ketergantungan untuk PHP. Ini digunakan untuk menginstal Laravel dan ketergantungannya.
	2	npm (Node Package Manager): npm digunakan untuk menginstal ketergantungan frontend seperti pustaka JavaScript atau framework CSS (misalnya Tailwind CSS).
	3	Artisan (CLI Laravel): Antarmuka baris perintah Laravel yang digunakan untuk menjalankan tugas seperti migrasi, menjalankan aplikasi, dan mengelola cron job.
	4	Mailtrap (Layanan SMTP): Digunakan untuk menangkap email selama pengembangan, memastikan bahwa fungsi email bekerja tanpa mengirim email nyata.
Fungsi Utama:
	•	Menerbitkan Tawaran Lokasi: Pemilik mobil dapat menerbitkan ketersediaan mobil mereka untuk hari/jam tertentu.
	•	Tawaran Premium: Pemilik mobil dapat membuat tawaran mereka menjadi premium agar lebih terlihat.
	•	Penyaringan dan Pencarian Tawaran: Pengguna dapat memfilter dan mencari mobil yang tersedia berdasarkan kebutuhan mereka.
	•	Notifikasi Email: Pengguna diberitahu melalui email ketika tawaran mereka diterima.
	•	Profil Pengguna: Setiap pengguna memiliki profil yang berisi informasi dan ulasan dari pengguna lain.
	•	Sistem Umpan Balik: Setelah setiap penyewaan mobil selesai, formulir umpan balik dikirim kepada pemilik mobil dan pengguna (manfaatnya).
Cara Mengatur Aplikasi:
	1	Kloning repositori: git clone ...
	2	Install ketergantungan:
	◦	composer install untuk ketergantungan PHP.
	◦	npm install untuk ketergantungan frontend.
	3	Setup Basis Data:
	◦	Buat file .env dan masukkan kredensial basis data yang valid.
	◦	Jalankan php artisan migrate untuk membuat tabel yang diperlukan.
	◦	Hasilkan kunci aplikasi: php artisan key:generate.
	4	Setup Email: Konfigurasi pengaturan SMTP Mailtrap di file .env untuk pengelolaan email.
	5	Jalankan aplikasi:
	◦	php artisan serve untuk menjalankan server pengembangan.
	◦	php artisan schedule:work untuk mengaktifkan cron job yang menjalankan tugas harian.
Penggunaan:
Setelah menyelesaikan pengaturan, pengguna dapat mendaftar akun dengan dua peran: satu sebagai "Partner" (pemilik mobil) dan satu lagi sebagai "User" (manfaat). Fitur untuk menerbitkan, menerima, dan mengelola tawaran dapat diuji di antara kedua akun ini.

