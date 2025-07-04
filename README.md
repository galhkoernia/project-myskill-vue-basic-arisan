Aplikasi Arisan Berbasis Vue.js
================================

Deskripsi:
----------
Proyek ini merupakan aplikasi web sederhana untuk mencatat peserta arisan secara interaktif
menggunakan framework Vue.js. Aplikasi ini dibuat sebagai bagian dari penyelesaian project 
kelas online di MySkill.

Fitur Utama:
------------
- Input nama peserta arisan
- Validasi nama (tidak boleh kosong atau duplikat)
- Menampilkan daftar peserta secara dinamis
- Transisi animasi saat menambahkan/menghapus peserta
- Tampilan antarmuka yang rapi dan modern

Teknologi yang Digunakan:
--------------------------
- Vue 3 (melalui Vue CLI)
- HTML5 & CSS3
- JavaScript (ES6)
- Built-in Vue transition system

Struktur Proyek:
----------------
src/
├── assets/
│   └── style.css               # Styling terpisah
├── components/
│   ├── ParticipantForm.vue     # Form input peserta
│   └── ParticipantList.vue     # Daftar peserta dengan transisi
├── App.vue                     # Root component
└── main.js                     # Entry point aplikasi

Cara Menjalankan:
-----------------
1. Clone repo atau download project ini
2. Buka terminal dan masuk ke direktori project
3. Jalankan perintah:
   npm install
   npm run serve
4. Buka browser dan akses:
   http://localhost:8080

Catatan:
--------
Project ini disusun untuk menyelesaikan kelas online:
"MySkill Bootcamp - Frontend Development"
dan sebagai latihan implementasi dasar Vue.js (komponen, props, event, dan transisi).

---

Galuh Kurnia Pratama
Bootcamp Frontend @ MySkill
