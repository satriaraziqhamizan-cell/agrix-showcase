# AGRIX — Showcase Gallery

Folder ini adalah galeri yang menampilkan **semua tools** AGRIX per role (Petani, Penyuluh, Pemerintah, Peneliti), berdampingan versi Web dan versi App — termasuk sub-level di dalam tools bertingkat (Peta Digital Twin, Detail Lahan, Profil).

⚠️ **Showcase ini HARUS dipublish PALING TERAKHIR**, setelah `agrix-web` dan `agrix-app` sudah live di GitHub Pages — karena showcase menampilkan kedua situs itu lewat iframe.

## Langkah-langkah
1. Publish dulu folder **agrix-web** → catat URL-nya (mis. `https://USERNAME.github.io/agrix-web`)
2. Publish folder **agrix-app** → catat URL-nya (mis. `https://USERNAME.github.io/agrix-app`)
3. Buka file `index.html` di folder ini dengan text editor apa saja, cari bagian paling atas `<script>` (sekitar baris ke-100), lalu edit 2 baris ini:
   ```javascript
   const WEB_BASE = "https://USERNAME.github.io/agrix-web";   // <-- ganti USERNAME & nama repo sesuai punyamu
   const APP_BASE = "https://USERNAME.github.io/agrix-app";   // <-- ganti USERNAME & nama repo sesuai punyamu
   ```
   Ganti `USERNAME` dan nama repo dengan punya kamu sendiri. **Jangan pakai garis miring `/` di akhir URL.**
4. Simpan file, lalu buat repository baru di GitHub (mis. `agrix-showcase`), push isi folder ini (`index.html`, `assets/`).
5. Aktifkan GitHub Pages seperti biasa (Settings → Pages → branch `main` → root).
6. Selesai! Kalau lupa mengedit langkah 3, showcase akan menampilkan kotak peringatan kuning di halaman.

## Isi folder
```
index.html   ← halaman showcase (berasal dari showcase.html, jangan diganti nama)
assets/      ← logo AGRIX (untuk header showcase saja)
```
