# Database Vendor CV LENTRA MICE - Vercel Ready

## Penyebab umum 404: NOT_FOUND di Vercel
404 biasanya muncul karena `index.html` tidak berada di root repository GitHub.

Struktur GitHub yang benar:

```
index.html
function.js
vercel.json
README.md
.gitignore
```

Jangan upload folder `lentra_mice_vercel_fix_404` ke dalam repository sehingga menjadi:

```
lentra_mice_vercel_fix_404/index.html
```

Jika struktur seperti itu, Vercel tidak menemukan halaman utama dan bisa muncul 404.

## Cara upload ke GitHub
1. Ekstrak ZIP ini.
2. Buka folder hasil ekstrak.
3. Upload isi foldernya saja ke GitHub, bukan foldernya.
4. Pastikan `index.html` terlihat langsung di halaman utama repository.
5. Deploy ulang di Vercel.

## Setting Vercel yang disarankan
- Framework Preset: Other
- Build Command: kosongkan
- Output Directory: kosongkan atau isi `.`
- Root Directory: `/` jika file ada langsung di root repository

## Catatan
Aplikasi ini berjalan sebagai static website dan menyimpan data di browser menggunakan localStorage.
