# Color Detector

**Color Detector** adalah aplikasi Android untuk mendeteksi warna secara real-time melalui kamera, mode manual, dan galeri. Aplikasi dapat diunduh dan dicoba melalui APK yang tersedia di [GitHub Releases](https://github.com/Valearaafi/Color-Detector/releases).

---

## Latar Belakang & Tujuan

Menentukan kode warna dari objek di sekitar biasanya membutuhkan alat khusus atau perkiraan manual. Color Detector dikembangkan untuk memberikan **pembacaan warna instan** langsung dari kamera ponsel: nama warna terdekat, kode HEX, RGB, dan HSV, tanpa aplikasi berbayar atau koneksi internet.

## Fitur yang Tersedia

- **Deteksi real-time** dari titik tengah kamera, diperbarui frame demi frame.
- **Mode manual** dengan crosshair yang dapat digeser ke titik mana pun pada layar.
- **Mode galeri** untuk memilih gambar dari perangkat dan mendeteksi warna dengan sentuhan.
- **Detail warna lengkap**: pratinjau warna, kode HEX, RGB, dan HSV dalam panel detail.
- **Perkiraan nama warna** berdasarkan jarak Euclidean terhadap 22 warna referensi.
- **Salin kode HEX** ke clipboard dengan satu ketukan.

## Teknologi yang Digunakan

- **Android native (Java)** — antarmuka dan logika aplikasi.
- **CameraX** — pipeline kamera untuk pratinjau dan analisis frame (konversi YUV ke RGB).
- **Material Design** — komponen FAB, kartu, bottom sheet, dan snackbar.
- **Gradle** — sistem build.

Spesifikasi aplikasi: Android 5.0 (API 21) ke atas.

## Mengunduh & Memasang

1. Buka halaman [Releases](https://github.com/Valearaafi/Color-Detector/releases) di repositori ini.
2. Unduh APK pada rilis terbaru (misalnya `ColorDetector-v1.0.0.apk`).
3. Pada ponsel Android, buka berkas APK yang sudah diunduh.
4. Jika diminta, izinkan pemasangan dari sumber tidak dikenal (*Settings → Install unknown apps*).
5. Ikuti proses pemasangan hingga selesai, lalu buka aplikasi dan berikan izin kamera.

> **Catatan**: APK yang tersedia ditandatangani dengan kunci *debug* untuk keperluan uji coba.

## Keterbatasan

- Nama warna merupakan perkiraan dari 22 warna referensi, bukan standar penamaan resmi.
- Pembacaan warna kamera dapat dipengaruhi oleh pencahayaan dan kondisi sensor perangkat.
