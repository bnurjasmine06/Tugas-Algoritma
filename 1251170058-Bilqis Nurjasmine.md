# TUGAS MANDIRI PERTEMUAN 1
**Nama:** Bilqis Nurjasmine  
**NIM:** 1251170058  
**Kelas:** 3 B 

---
### BAGIAN A RANCANGAN ALGORITMA DENGAN KARAKTERISTIK LENGKAP

#### CASE KELAS B (Pendaftaran & Otentikasi Pengguna Baru)
> **Langkah-langkah (Instruksi Terstruktur):**
1.	Mulai
2.	Pengguna membuka aplikasi mobile banking dan menekan menu “Daftar” atau “Buat Akun”.
3.	Pengguna memasukkan data yang diperlukan seperti, nomer rekening, nomer handphone yang sudah terdaftar di bank, dan identitas diri sesuai ketentuan yang berlaku di bank
4.	Sistem memeriksa kecocokan data yang dimasukkan dengan data yang sudah terdaftar pada sistem bank
5.	Jika data tidak cocok sistem memunculkan pesan kesalahan dan meminta pengguna mengecek kembali serta memasukkan kembali data
6.	Jika data sudah sesuai, sistem meminta pengguna untuk membuat username dan password untuk akun mobile banking.
7.	Sistem memverifikasi username dan kekuatan password sesuai dengan ketentuan keamanan yang berlaku.
8.	Jika password tidak memenuhi ketentuan tersebut, sistem akan memunculkan pesan kesalahan dan meminta pengguna membuat ulang password
9.	Jika data akun sesuai, sistem mengirimkan pesan berupa  kode OTP ke nomer handphone yang terdaftar.
10.	Pengguna mengetik kode OTP yang diterima
11.	Sistem memeriksa kode OTP yang dimasukkan
12.	Jika kode OTP salah atau kadaluwarsa, sistem menampilkan pesan kesalahan dan meminta pengguna melakukan verifikasi kembali.
13.	Jika kode OTP yang dimasukkan benar, sistem akan meminta pengguna untuk membuat PIN mobile banking.
14.	Pengguna memasukan PIN dan mengkonfirmasinya.
15.	Sistem memeriksa kesesuaian PIN yang dimasukkan
16.	Jika PIN sudah sesuai, seluruh data dan verifikasi telah berhasil, sistem akan memulai membuat akun mobile banking pengguna
17.	Sistem menyimpan data akun dan informasi autentifikasi secara aman ke dalam sistem bank
18.	Sistem menampilkan notifikasi “Pembuatan akun Anda telah berhasil”.
19.	Selesai

**Karakteristik Algoritma:**    
1. **Input:** Nomer rekening, nomer handphone yang terdaftar, data identitas yang dimasukkan, username, password, kode OTP, dan PIN mobile banking
   
2. **Output:** Akun mobile banking berhasil dibuat, data akun tersimpan denga naman di sistem bank, dan sistem menampilkan notifikasi “Pembuatan akun Anda telah berhasil. Jika terjadi kesalahan dalam proses sistem akan menampilkan pesan kesalahan dan meminta pengguna untuk melakukan perbaikan atau verifikasi kembali
   
3. **Definiteness:** Setiap Langkah dalam algoritma memiliki instruksi yang jelas dan kondisi validasi format dan pencocokan bernilai pasti (bener/salah) tanpa ada makna ganda
  
4. **Finiteness:** Memiliki titik akhir yang jelas dengan dua kemungkinan yang pertama setelah sitem berhasil membuat akun, menyimpan data akun dan menampilkan notifikasi “Pembuatan akun Anda telah berhasil. Yang kedua proses dapat berhenti apabila data atau proses yang dilakukan tidak memenuhi dan proses dihentikan oleh pengguna
   
5. **Effectiveness:** Langkahnya sangat berurutan mulai dari pengumpulan data hingga verifikasi dua langkah

### BAGIAN B: ANALISIS PEMILIHAN STRUKTUR DATA
1. **Skenario 1 (Fitur Undo / Redo):**  
   Sebuah aplikasi pengolah kata (*Text Editor*) membutuhkan fitur untuk membatalkan ketikan terakhir pengguna (*Undo*) dan mengembalikannya lagi (*Redo*).  
   * **Struktur Data Terpilih:** Stack   
   * **Alasan:** Stack cocok digunakan untuk fitur undo dan redo karna memiliki prinsip Last In First Out, yang artinya tindakan yang dilakukan terakhir akan menjadi tindakan yang dikeluarkan pertama. Contohnya saat lagi mengedit di canva langkah terakhir itu memisahkan elemen-elemen yang sebelumnya jadi satu, jadi ketika memencet tombol undo, tindakan terakhir tersebut yang memisakan elemen-elemen dibatalkan jadi, elemen-elemen yang tadinya kepisah jadi satu lagi  

2. **Skenario 2 (Peta Navigasi Rute Perjalanan):**  
   Sebuah aplikasi GPS membutuhkan cara untuk memodelkan lokasi-lokasi kota beserta jalan penghubungnya guna mencari rute tercepat.  
   * **Struktur Data Terpilih:** Graph  
   * **Alasan:** Graph cocok digunakan karena dalam pembahasan graph itu seperti peta navigasi yang bisa menggambarkan antara tempat satu dengan tempat yang lainnya. contoh pergi ke kampus menggunakan Google maps rumah dan kampus sebagai titik dan jalan yang menghubungkan sebagai penghubung. Dengan menggunakan graph orang akan tau rute mana yang paling cepat 

3. **Skenario 3 (Sistem Login Pengguna Berbasis Username):**  
   Sistem butuh mencari data akun dari jutaan *user* secara instan berdasarkan *Username* saat proses *login*.  
   * **Struktur Data Terpilih:** Hash Table  
   * **Alasan:** Hash Table cocok digunakan untuk sistem login karena dapat mencari data pengguna menggunakan username dengan cepat. contoh mau login mobile banking trus masukin username dan password yang sudah dibuat. Sistem akan mencari username tersebut untuk menemukan data akun dan mencocokkan password yang dimasukkan. jadi sistem bisa mecari dengan cepat tanpa harus mengecek satu-satu

