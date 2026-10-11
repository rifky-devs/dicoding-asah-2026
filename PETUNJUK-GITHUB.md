# Cara mengunggah ke GitHub

1. Ekstrak ZIP ini.
2. Buat repository baru di GitHub, misalnya `dicoding-asah-2026`. Pilih repository kosong agar tidak bentrok dengan file yang sudah ada.
3. Buka folder hasil ekstrak di VS Code.
4. Buka terminal di folder itu, lalu jalankan:

```bash
git init
git branch -M main
git add .
git commit -m "docs: add Dicoding Asah learning notes"
git remote add origin https://github.com/USERNAME/dicoding-asah-2026.git
git push -u origin main
```

Ganti `USERNAME` dengan username GitHub sendiri. Perintah tersebut untuk repository baru. Kalau repository sudah berisi file, jangan langsung menjalankan langkah ini; cek isi repository dulu.

Setelah berhasil diunggah, setiap kali ada catatan baru:

```bash
git add .
git commit -m "docs: add notes for [nama materi]"
git push
```

Sebelum commit, jalankan `git status` dan pastikan tidak ada password, token, API key, atau file `.env` yang ikut masuk.
