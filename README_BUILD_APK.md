# Pijar Sekolah — Android WebView Bersih (Tanpa Header Browser)

Proyek ini dibuat khusus untuk menjalankan **https://siswa.pijarsekolah.id** sebagai aplikasi Android native tanpa bilah alamat/judul Chrome (`Beranda - Pijar Sekolah | siswa.pijarsekolah.id`) dan menggunakan ikon APK kustom Anda.

## Fitur yang Sudah Terpasang
- **Tanpa Header Website/Browser**: Menggunakan `Theme.Material3.Light.NoActionBar` dengan Status Bar berwarna `#0E87E6`.
- **Ikon APK Kustom**: Sudah dikonversi otomatis menjadi format PNG resmi Android di semua folder `mipmap-*` serta Adaptive Icon (`ic_launcher_foreground.png`).
- **Sesi Login Tersimpan**: `CookieManager` & `domStorageEnabled` aktif agar tidak perlu login ulang terus-menerus.
- **Upload Tugas & Download PDF**: Mendukung `onShowFileChooser` dan `DownloadManager`.
- **Tombol Kembali (Back)**: Menavigasi riwayat halaman WebView sebelum menutup aplikasi.

## Cara Build Menjadi File `.apk`

### Cara 1: Tanpa PC / Laptop (Lewat GitHub Actions — Gratis)
1. Buat repository baru di GitHub lalu unggah semua isi folder ZIP ini (termasuk folder `.github/workflows/build-apk.yml`).
2. Buka tab **Actions** di repository GitHub Anda, lalu jalankan workflow **Build Pijar Sekolah APK**.
3. Setelah selesai (~2 menit), unduh file **PijarSekolah-APK** (`app-debug.apk`) dan langsung instal di HP Android Anda!

### Cara 2: Menggunakan Android Studio di PC / Laptop
1. Ekstrak folder ZIP ini, lalu buka di **Android Studio** (*File > Open*).
2. Tunggu proses Gradle Sync selesai.
3. Klik menu **Build > Build Bundle(s) / APK(s) > Build APK(s)**.
4. Ambil file APK di `app/build/outputs/apk/debug/app-debug.apk`.
