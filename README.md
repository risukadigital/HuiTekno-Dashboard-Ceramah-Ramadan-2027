# HuiTekno — Dashboard Ceramah Firebase

Proyek salinan berbasis template HTML yang diberikan, dipisahkan dari proyek nomor 1 (Supabase).

## Yang perlu dilakukan
1. Buat project Firebase baru untuk proyek nomor 14.
2. Aktifkan **Authentication → Email/Password** dan buat akun admin.
3. Buat **Cloud Firestore database**.
4. Buka `index.html`, lalu isi `firebaseConfig` dengan konfigurasi aplikasi web dari Firebase Console. Jangan memasukkan private key/service-account key ke frontend.
5. Deploy ke Hosting setelah uji coba. Instal Firebase CLI (`npm install -g firebase-tools`), login (`firebase login`), lalu dari folder ini jalankan `firebase deploy`.

## Struktur
- `index.html` — UI template dan adapter Firebase Auth/Firestore.
- `firebase.json` — konfigurasi Hosting dan Firestore rules.
- `firestore.rules` — aturan awal: baca jadwal publik, tulis hanya setelah login.
- `manifest.json`, `service-worker.js` — dukungan PWA dasar.

## Penting sebelum produksi
- Aturan Firestore ini mengizinkan semua akun terautentikasi menulis. Untuk produksi, ubah menjadi custom claims admin atau aturan role khusus sebelum deploy publik.
- Template memiliki agenda Khatib Idul Fitri/Idul Adha yang belum disimpan ke database oleh kode sumber; bagian itu belum ditambahkan pada migrasi ini.
- Realtime menggunakan `onSnapshot` Firestore. Lakukan pengujian login, baca, tambah, edit, hapus, dan akses lintas perangkat setelah konfigurasi Firebase diisi.
- Tidak ada konfigurasi Firebase nyata yang disertakan; aplikasi belum terhubung atau dipublikasikan.
