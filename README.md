# HuiTekno — Dashboard Ceramah Ramadan 2027

Aplikasi pengelolaan jadwal ceramah Ramadan berbasis HTML, JavaScript, Firebase Hosting, dan Cloud Firestore.

## 🌐 Tautan Proyek

- **Website aktif:** https://fir-penceramah-ramadhan.web.app
- **Repositori GitHub:** https://github.com/risukadigital/HuiTekno-Dashboard-Ceramah-Ramadan-2027

## Status Proyek

- Website telah berhasil di-deploy ke Firebase Hosting.
- Formulir penyimpanan jadwal publik telah diuji melalui HP dan berhasil menyimpan jadwal.
- Kode sumber telah disimpan di GitHub pada cabang `main`.
- Pengujian fitur lain tetap perlu dilakukan secara bertahap.

## Struktur File

| File atau folder | Fungsi |
|---|---|
| `index.html` | Antarmuka dan logika utama aplikasi |
| `firebase.json` | Konfigurasi Firebase Hosting dan Firestore Rules |
| `firestore.rules` | Aturan akses Cloud Firestore |
| `.firebaserc` | Referensi proyek Firebase |
| `manifest.json` | Metadata aplikasi PWA |
| `service-worker.js` | Dukungan cache dan PWA |
| `icons/` | Ikon aplikasi |
| `PWA1.png` | Gambar pendukung aplikasi |
| `FIREBASE_PENCERAMAH_RAMADHAN_27.html` | File HTML tambahan proyek |

## Teknologi

- HTML, CSS, dan JavaScript
- Firebase Hosting
- Cloud Firestore
- Firebase Authentication
- Progressive Web App (PWA)

## Alur Pengembangan

Pastikan Firebase CLI sudah terpasang dan akun yang digunakan memiliki akses ke proyek.

Login Firebase:

```powershell
firebase login
```

Periksa perubahan lokal:

```powershell
git status
```

Simpan perubahan ke Git:

```powershell
git add .
git commit -m "Deskripsi perubahan"
git push origin main
```

Deploy perubahan aplikasi ke Firebase Hosting:

```powershell
firebase deploy --only hosting --project fir-penceramah-ramadhan
```

Perintah Git menyimpan dan mengirim kode ke GitHub. Perintah deploy memperbarui aplikasi di Firebase Hosting. Keduanya merupakan proses yang berbeda.

## Keamanan

- Jangan memasukkan kata sandi, token akses, private key, atau service-account key ke repositori publik.
- Aturan Firestore harus membatasi operasi baca, tambah, edit, dan hapus sesuai kebutuhan aplikasi.
- Periksa aturan akses publik dan admin sebelum menambahkan fitur baru.
- Hindari memasukkan nomor HP atau data pribadi nyata ke dokumentasi publik.

## Pengujian Berikutnya

- Memastikan jadwal yang disimpan dari HP tampil di laptop.
- Menguji login admin.
- Menguji tambah, edit, dan hapus jadwal sesuai hak akses.
- Memastikan pembaruan data konsisten di berbagai perangkat.
- Memeriksa perilaku cache dan pembaruan PWA.

## Riwayat Versi

- `e729184` — Versi awal HuiTekno Dashboard Ceramah Ramadan 2027.
