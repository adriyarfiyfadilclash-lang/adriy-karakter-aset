# Aset karakter ADRIY (privat)

Gambar karakter ADRIY untuk video Adriy.project. Repo ini sengaja privat: berisi wajah ADRIY.

- `santai/` — outfit santai (sweater abu-abu ADRIY, celana hitam, sneaker)
  - `00-penuh-berdiri.webp`, `lembar-01..09.png` — lembar asli badan penuh (4 pose per lembar)
  - `dekat/` — lembar asli close-up dan setengah badan, termasuk 5 bentuk mulut (`dekat-09.png`)
  - `aset.json` — daftar pose per lembar
  - `pose/` — hasil potong: satu PNG transparan per pose (dibuat `scripts/adri_aset.py` di repo Aidriy)
  - `peta.json` — peta pose ADRI -> gambar, dibaca video

- `travel/` — outfit travel (jaket abu-abu, ransel, tas pinggang ADRIY, headphone, botol, bantal leher, celana kargo)
  - `lembar-01..09.png` badan penuh, `dekat/` close-up, setengah badan, dan lembar bentuk mulut
  - `tata.json` — tata letak lembar dan peta pose khusus outfit ini

- `arkeolog/` — outfit arkeolog/petualang lapangan (topi rimba, kemeja khaki ADRIY, rompi, ransel), 85 pose
  siap pakai di `pose/`; dipakai otomatis untuk video bertopik sejarah/arkeologi

- `formal/` (69 pose) jas formal — investasi, ekonomi, bisnis, berita; juga style bisnis
- `angkasa/` (69 pose) astronot — luar angkasa, planet, atmosfer
- `penyelam/` (41 pose + 4 rusak di `rusak/`) penyelam — laut, hewan laut; ada siklus jalan dan bentuk mulut badan penuh
- `lab/` (78 pose) jas lab — sains, kimia, biologi, kedokteran; juga style sains

Outfit dipilih otomatis per video dari topik (lihat `art_direct` di pipeline.py repo Aidriy).

## Dipakai di repo Aidriy

```bash
bash video/scripts/ambil_aset.sh        # salin repo ini ke video/public/adri/ (tidak masuk git Aidriy)
```

Menambah aset baru: taruh lembar di folder outfit, tambah tata letaknya di `scripts/adri_aset.py` (repo Aidriy),
jalankan skrip itu, lalu commit hasilnya di sini.
