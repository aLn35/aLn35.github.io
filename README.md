# Portfolio - Deployment (GitHub Pages)

Panduan singkat untuk men-deploy website ini secara gratis menggunakan GitHub Pages (user/organization site).

File penting:
- `index.html`
- `assets/` (folder berisi gambar, PDF CV, dll.)

Langkah cepat (web akan tersedia di `https://<username>.github.io`):

1) Buat repository baru di GitHub
- Buka https://github.com/new
- Di kolom "Repository name" ketik persis: `aLn35.github.io` (harus sama persis dengan username GitHub)
- Pilih Public
- Jangan centang "Add a README file"
- Klik Create repository

2) Upload file lewat web (cara mudah)
- Di halaman repo baru klik "uploading an existing file"
- Drag & drop seluruh isi workspace (`index.html` + folder `assets/`)
- Klik "Commit changes"

3) Atau pakai terminal (lebih cepat jika nyaman):

```bash
# di root folder project (tempat index.html berada)
git init
git add .
git commit -m "Initial portfolio"
git branch -M main
# ganti <username> jika diperlukan, contoh: aLn35
git remote add origin https://github.com/aLn35/aLn35.github.io.git
git push -u origin main
```

4) Aktifkan GitHub Pages
- Masuk ke tab `Settings` pada repo
- Pilih `Pages` di sidebar kiri
- Pada bagian `Source` pilih `Deploy from a branch`
- `Branch` pilih `main`, folder pilih `/ (root)`
- Klik `Save`
- Tunggu 1-2 menit lalu refresh halaman `Settings > Pages` sampai muncul notifikasi "Your site is live at https://aLn35.github.io"

5) Verifikasi & caching
- Setelah live, buka link `https://aLn35.github.io` di HP/tablet/desktop
- Jika tidak terlihat, tekan Ctrl+F5 (hard refresh) atau bersihkan cache browser

Tips tambahan & perbaikan yang saya terapkan:
- Sudah menambahkan aturan CSS responsif di akhir `index.html` untuk meningkatkan tampilan di HP, tablet, desktop.
- Periksa `assets/` agar path relatif di `index.html` tidak rusak.

Butuh bantuan saya untuk:
- Menyusun commit dan melakukan `git push` dari komputer ini (kamu perlu memberikan akses atau jalankan perintah di terminal lokal).
- Saya bisa buat PR, menyiapkan branch, atau menulis file tambahan jika mau.

Katakan apa yang mau saya lakukan selanjutnya: saya bisa kirim perintah `git` yang perlu kamu jalankan, atau bantu langkah upload lewat web.