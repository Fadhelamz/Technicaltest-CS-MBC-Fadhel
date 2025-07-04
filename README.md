# Technical Test Cyber Security MBC Laboratory - Landing Page Project

Website ini dibuat oleh **Fadhel Ahmad Mudzakky** sebagai bagian dari technical test untuk Divisi Cyber Security di MBC Laboratory, Telkom University.
Project ini terdiri dari frontend berbasis HTML dan CSS, serta backend sederhana menggunakan PHP untuk mengelola form kontak.
Website telah dideploy secara online menggunakan GitHub Pages dan Vercel (frontend only).

## 🌐 Live Website (Frontend only)
https://technicaltest-cs-mbc-fadhel.vercel.app/

## 🗂️ Struktur Proyek
MBC-LAB/

├── frontend/

│   ├── index.html          # Halaman Home

│   ├── css/

│   │   └── style.css       # Semua styling digabung di satu file


│   └── assets/

│       └── images/         # Gambar

├── backend/

│   ├── contact.php 

└── README.md

## ⚙️ Instruksi Instalasi Lokal
Berikut adalah langkah-langkah untuk menjalankan proyek secara lokal di komputer Anda:

### 1. Clone Repository atau Salin Folder ke htdocs (XAMPP)
Jika menggunakan GitHub:
bash
git clone https:https://github.com/Fadhelamz/Technicaltest-CS-MBC-Fadhel.git
cd Technicaltest-CS-MBC-Fadhel
Atau cukup salin folder ke htdocs/ pada XAMPP Anda

2. Jalankan Backend PHP
Aktifkan Apache dari XAMPP Control Panel
Buka browser dan akses:
http://localhost//Technicaltest-CS-MBC-Fadhel/index.html

3. Form Kontak
Form kontak berada di bagian bawah halaman utama
Saat dikirim, akan mengarah ke file contact.php

🚀 Deployment
🔸 GitHub Pages (Frontend Only)
Upload repository ke GitHub (public)

Masuk ke Settings > Pages > pilih branch main dan folder / (root)

Website otomatis akan muncul di:
https://fadhelamz.github.io/Technicaltest-CS-MBC-Fadhel/

🔸 Vercel (Alternatif Frontend)
Masuk ke https://vercel.com dan login dengan GitHub
Klik "New Project" → pilih repo Technicaltest-CS-MBC-Fadhel
Deploy dan akses via domain dari Vercel

🔗 Live: https://technicaltest-cs-mbc-fadhel.vercel.app/

⚠️ Vercel dan GitHub Pages tidak mendukung file .php, sehingga backend hanya berjalan secara lokal atau di hosting seperti InfinityFree.

🔐 Konfigurasi SSL & Backend
Frontend (GitHub Pages & Vercel) sudah otomatis menggunakan HTTPS (aman).
Backend (PHP) saat ini hanya bisa berjalan di server lokal (XAMPP) atau hosting PHP seperti InfinityFree / 000webhost.
Belum digunakan database atau autentikasi lanjutan.

## ⚠️ Keterbatasan Backend (contact.php)

Form kontak pada proyek ini menggunakan `contact.php` sebagai backend sederhana untuk menerima dan menampilkan data yang dikirim dari form HTML.

Namun, file PHP tidak dapat dijalankan di GitHub Pages maupun Vercel karena kedua platform ini tidak menyediakan dukungan untuk server-side script seperti PHP. Akibatnya:

- Form tetap bisa diisi oleh pengguna, **tapi tidak akan diproses** saat diklik "Send".
- File `contact.php` hanya bisa dijalankan secara lokal (di XAMPP/Laragon) atau di hosting yang mendukung PHP seperti **InfinityFree** atau **000webhost**.

### Solusi Sementara
Untuk mencoba form kontak agar benar-benar bekerja:
1. Jalankan proyek secara lokal menggunakan XAMPP atau Laragon.
2. Atau, upload file `contact.php` ke hosting gratis yang support PHP.

## ❗ Error: "This site can’t be reached" Saat Submit Form

Saat pengguna menekan tombol **"Send"** pada form kontak, browser akan mencoba mengakses file `contact.php` menggunakan metode POST.

Namun, jika proyek ini dijalankan
maka backend (`contact.php`) **tidak dapat dijalankan**, karena:
- GitHub Pages dan Vercel **tidak memiliki server PHP**
- Saat browser mencoba mengakses `contact.php`, responsnya akan **404 Not Found** atau **"This site can’t be reached"**

### 💡 Contoh Error:
   This site can’t be reached
   contact.php refused to connect.
   
📁 Dokumentasi Tambahan
File PDF dokumentasi tersedia, mencakup:
Alur kerja form
Diagram arsitektur
Screenshot tampilan semua halaman

📝 Penutup
Website ini dibuat sebagai bagian dari tes rekrutasi Divisi Cyber Security MBC Lab.
Saya menyadari adanya keterbatasan pada bagian backend (PHP belum di-hosting), namun struktur proyek ini sudah mendukung pengembangan lebih lanjut jika dibutuhkan.
Terima kasih atas kesempatan dan semoga hasil project ini menunjukkan komitmen dan potensi saya.

— Fadhel Ahmad Mudzakky
