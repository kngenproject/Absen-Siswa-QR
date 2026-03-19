<div align="center">

<img src="https://img.shields.io/badge/versi-2.3.0-0077c8?style=for-the-badge&logo=html5&logoColor=white" />
<img src="https://img.shields.io/badge/PWA-Offline%20Ready-16a34a?style=for-the-badge&logo=googlechrome&logoColor=white" />
<img src="https://img.shields.io/badge/No%20Backend-localStorage-f59e0b?style=for-the-badge&logo=databricks&logoColor=white" />
<img src="https://img.shields.io/badge/Bahasa-Indonesia-dc2626?style=for-the-badge" />

# 📋 Absensi Siswa QR

**Aplikasi absensi siswa berbasis QR Code — satu file HTML, tanpa server, offline ready.**

Dirancang untuk guru dan staf sekolah yang ingin sistem absensi digital yang cepat, ringan, dan bisa berjalan penuh tanpa koneksi internet.

[⬅️ Kembali ke repo utama](../README.md) · [🐛 Laporkan Bug](../../issues) · [💡 Request Fitur](../../issues)

</div>

---

## ✨ Fitur Utama

| Fitur | Keterangan |
|---|---|
| 📷 **Scan QR via Kamera** | Absen otomatis hanya dengan kamera HP atau laptop |
| 🪪 **Generate Kartu QR** | Buat kartu QR individual per siswa, lengkap dengan nama & kelas |
| 📊 **Import Excel Massal** | Upload file `.xlsx`, `.xls`, atau `.csv` untuk input banyak siswa sekaligus |
| 🗂️ **Export QR Semua Kelas** | Ekspor QR seluruh siswa ke Excel (per sheet kelas) atau ZIP (PNG per siswa) |
| 📅 **Rekap Absensi** | Rekap harian dengan filter tanggal, kelas, dan status kehadiran |
| 📤 **Export ke Excel & CSV** | Unduh data rekap absensi untuk arsip atau laporan |
| 🔔 **Notifikasi Suara** | Bunyi konfirmasi saat absen berhasil tercatat |
| 📶 **PWA — Bisa Diinstall** | Install ke layar utama HP/laptop, bisa dipakai penuh tanpa internet |

---

## 🖥️ Tampilan Aplikasi

Aplikasi memiliki 6 tab utama yang bisa diakses dari navigasi atas:

```
📊 Dashboard   🪪 Buat Kartu   📥 Import Excel   🗂️ QR Semua Kelas   👥 Daftar Siswa   📅 Rekap Absensi
```

**Dashboard** — Ringkasan statistik hari ini: jumlah hadir, terlambat, izin/sakit, dan total siswa.

**Buat Kartu** — Input data siswa (Nama, NIS, Kelas, No. Absen), generate QR, lalu download PNG atau cetak langsung.

**Import Excel** — Upload file Excel, preview data, lalu simpan massal ke sistem. Template siap unduh tersedia.

**QR Semua Kelas** — Generate QR seluruh siswa sekaligus, lalu ekspor ke Excel (per sheet) atau ZIP (PNG per siswa).

**Daftar Siswa** — Kelola data siswa dengan pencarian dan filter per kelas.

**Rekap Absensi** — Tampilkan, filter, dan ekspor rekap berdasarkan tanggal, kelas, dan status kehadiran.

---

## ⚡ Instalasi & Penggunaan

### Cara 1 — Buka Langsung
1. Download file `index.html`
2. Buka dengan browser (Chrome / Edge / Firefox)
3. Langsung bisa digunakan ✅

### Cara 2 — Install sebagai PWA *(Direkomendasikan)*
1. Buka aplikasi di browser Chrome
2. Klik ikon **"Install"** di address bar (atau *Add to Home Screen*)
3. Aplikasi tersimpan di layar utama dan bisa dibuka offline

> Saat pertama dibuka dalam kondisi online, Service Worker akan otomatis meng-cache semua library. Setelah itu semua fitur berjalan offline penuh.

---

## 📋 Format Template Excel (Import)

| Nama | NIS *(opsional)* | Kelas | No Absen *(opsional)* |
|---|---|---|---|
| Budi Santoso | 2024001 | 10A | 1 |
| Siti Rahayu | 2024002 | 10A | 2 |

- Baris pertama boleh berupa header atau langsung data
- Template siap pakai: tab **Import Excel** → *Download Template Excel*

---

## 🔒 Privasi & Penyimpanan Data

Semua data tersimpan di **localStorage** browser — tidak ada data yang dikirim ke server manapun.

> ⚠️ Disarankan melakukan ekspor Excel secara berkala sebagai cadangan.

---

## 📦 Library yang Digunakan

| Library | Versi | Fungsi |
|---|---|---|
| [html5-qrcode](https://github.com/mebjas/html5-qrcode) | latest | Scan QR via kamera |
| [qrcodejs](https://github.com/davidshimjs/qrcodejs) | 1.0.0 | Generate QR code |
| [SheetJS (xlsx)](https://sheetjs.com/) | 0.18.5 | Import & export Excel |
| [JSZip](https://stuk.github.io/jszip/) | 3.10.1 | Export QR ke ZIP |
| [Google Fonts](https://fonts.google.com/) | — | Nunito & Poppins |
| [Material Icons](https://fonts.google.com/icons) | — | Ikon antarmuka |

---

## 📝 Riwayat Versi

### v2.3.0 — Maret 2026 *(Terbaru)*
- ✨ PWA Offline penuh — bisa diinstall & dipakai tanpa internet
- ✨ Service Worker otomatis cache semua library CDN saat online
- ✨ Banner offline & toast notifikasi saat koneksi kembali
- ✨ Web App Manifest + ikon app dari SVG inline
- ✨ Auto-update notifikasi saat versi baru tersedia

### v2.2.0 — Maret 2026
- ✨ Kelas dinamis — terisi otomatis sesuai data siswa
- ✨ Notifikasi suara saat absen berhasil
- 🔧 Tampilan tab Scan dioptimalkan untuk HP

### v2.1.0 — Juni 2025
- ✨ Import data siswa massal dari Excel / CSV
- ✨ Generate QR semua siswa sekaligus per kelas
- ✨ Export QR ke Excel dan ZIP
- 🔧 Drag & drop upload, preview sebelum import

### v2.0.0 — Mei 2025
- ✨ Scan QR otomatis via kamera
- ✨ Rekap absensi harian dengan filter
- ✨ Export rekap ke Excel & CSV

### v1.0.0 — Rilis Awal
- ✨ Buat kartu QR siswa satu per satu
- ✨ Download & cetak QR PNG
