# Aset karakter ADRIY (privat)

Gambar karakter ADRIY untuk video Adriy.project. Repo ini sengaja privat: berisi wajah ADRIY.

- `santai/` — outfit santai (sweater abu-abu ADRIY, celana hitam, sneaker)
  - `00-penuh-berdiri.webp`, `lembar-01..09.png` — lembar asli badan penuh (4 pose per lembar)
  - `dekat/` — lembar asli close-up dan setengah badan, termasuk 5 bentuk mulut (`dekat-09.png`)
  - `aset.json` — daftar pose per lembar
  - `pose/` — hasil potong: satu PNG transparan per pose (dibuat `scripts/adri_aset.py` di repo Aidriy)
  - `peta.json` — peta pose ADRI -> gambar, dibaca video

## Dipakai di repo Aidriy

```bash
bash video/scripts/ambil_aset.sh        # salin repo ini ke video/public/adri/ (tidak masuk git Aidriy)
```

Menambah aset baru: taruh lembar di folder outfit, tambah tata letaknya di `scripts/adri_aset.py` (repo Aidriy),
jalankan skrip itu, lalu commit hasilnya di sini.
