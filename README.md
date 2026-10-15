# Radio Files

Hosting mp3 untuk radio FiveM lewat GitHub Pages.

## Struktur
```
.
├── index.html     halaman tes + generator link otomatis
├── songs.json     daftar lagu
├── .nojekyll      biar Pages cepat deploy
└── lagu/          taruh mp3 di sini
```

## Cara tambah lagu
1. Ganti nama mp3 tanpa spasi, huruf kecil, pakai `-` (contoh: `lagu-4.mp3`).
2. Upload ke folder `lagu/` (Add file > Upload files, atau lewat Git/GitHub Desktop).
3. Tambah baris di `songs.json`:
   ```json
   { "label": "Lagu 4", "file": "lagu/lagu-4.mp3" }
   ```
   Hati-hati koma: semua baris pakai koma kecuali yang terakhir.
4. Commit, tunggu 1-3 menit.
5. Buka `https://USERNAME.github.io/NAMAREPO/`, tes play, lalu Copy link / Copy Lua.

## Aktifkan Pages
Settings > Pages > Source: Deploy from a branch > Branch: main, folder / (root) > Save.
