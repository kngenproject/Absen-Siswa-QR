# Panduan Kontribusi

Terima kasih sudah tertarik untuk berkontribusi pada **Absensi Siswa QR**! 🎉

---

## 🐛 Melaporkan Bug

1. Pastikan bug belum dilaporkan di [Issues](../../issues)
2. Buka Issue baru dengan judul yang jelas
3. Sertakan:
   - Langkah-langkah untuk mereproduksi bug
   - Perilaku yang diharapkan vs yang terjadi
   - Browser dan versi yang digunakan
   - Screenshot jika memungkinkan

---

## 💡 Mengusulkan Fitur

1. Buka Issue baru dengan label `enhancement`
2. Jelaskan fitur yang diusulkan dan alasan manfaatnya
3. Jika bisa, sertakan mockup atau contoh referensi

---

## 🔧 Mengajukan Pull Request

1. **Fork** repo ini
2. Buat branch baru dari `main`:
   ```bash
   git checkout -b fitur/nama-fitur
   # atau
   git checkout -b fix/nama-bug
   ```
3. Lakukan perubahan pada file `index.html`
4. Test di browser sebelum commit
5. Commit dengan pesan yang deskriptif:
   ```bash
   git commit -m "Tambah: fitur export PDF rekap absensi"
   git commit -m "Fix: scan QR gagal di Safari iOS"
   ```
6. Push ke branch kamu:
   ```bash
   git push origin fitur/nama-fitur
   ```
7. Buka Pull Request ke branch `main`

---

## 📐 Panduan Kode

Karena ini adalah aplikasi single-file HTML, harap perhatikan:

- **Jangan tambahkan dependensi baru** tanpa diskusi terlebih dahulu
- Semua library dimuat dari CDN — pastikan ada fallback untuk mode offline
- Pertahankan kompatibilitas dengan Chrome, Firefox, dan Edge versi terbaru
- Pastikan tampilan tetap responsif di layar mobile
- Data harus tetap tersimpan dan terbaca dari `localStorage` yang sudah ada

---

## 📋 Konvensi Pesan Commit

| Prefix | Digunakan untuk |
|---|---|
| `Tambah:` | Fitur baru |
| `Fix:` | Perbaikan bug |
| `Update:` | Perubahan pada fitur yang sudah ada |
| `Hapus:` | Menghapus kode atau fitur |
| `Docs:` | Perubahan dokumentasi |
| `Style:` | Perubahan tampilan/CSS |

---

Dengan berkontribusi, kamu setuju bahwa kontribusimu akan dilisensikan di bawah lisensi **MIT** yang sama dengan proyek ini.
