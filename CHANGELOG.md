# Changelog

Semua perubahan penting pada proyek ini didokumentasikan di file ini.

Format mengikuti [Keep a Changelog](https://keepachangelog.com/id/1.0.0/).

---

## [2.3.0] — Maret 2026

### Ditambahkan
- PWA Offline penuh — bisa diinstall & dipakai tanpa internet
- Service Worker otomatis cache semua library CDN saat pertama online
- Banner notifikasi saat aplikasi berjalan offline
- Toast notifikasi saat koneksi internet kembali
- Web App Manifest dengan ikon app dari SVG inline
- Auto-update notifikasi saat versi baru tersedia

### Diperbaiki
- Semua data tetap tersimpan dan terbaca dari localStorage saat offline

---

## [2.2.0] — Maret 2026

### Ditambahkan
- Kelas dinamis — dropdown kelas terisi otomatis sesuai data siswa yang diinput
- Notifikasi suara saat absen berhasil tercatat

### Diperbaiki
- Tampilan tab Scan dioptimalkan dan dipadatkan untuk layar HP

---

## [2.1.0] — Juni 2025

### Ditambahkan
- Import data siswa massal dari file Excel (.xlsx, .xls) dan CSV
- Generate QR untuk semua siswa sekaligus, dikelompokkan per kelas
- Export QR ke Excel (per sheet kelas dalam satu file)
- Export QR ke ZIP (PNG individual per siswa, folder per kelas)
- Download template Excel siap pakai untuk import
- Drag & drop upload file Excel
- Preview data sebelum disimpan ke sistem

---

## [2.0.0] — Mei 2025

### Ditambahkan
- Scan QR otomatis via kamera HP atau laptop
- Generate QR per siswa secara manual
- Absensi manual dari dropdown pilihan siswa
- Rekap absensi harian dengan filter tanggal, kelas, dan status
- Export rekap absensi ke Excel (.xlsx) dan CSV
- Statistik kehadiran hari ini (hadir, terlambat, izin, sakit)
- Mode offline dasar (PWA)

---

## [1.0.0] — Rilis Awal

### Ditambahkan
- Versi awal aplikasi absensi QR
- Buat kartu QR siswa satu per satu
- Download QR sebagai PNG
- Cetak QR langsung dari browser
