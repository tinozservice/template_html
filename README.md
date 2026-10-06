# Template HTML — VibeCode Template

Koleksi **template HTML single-file** siap pakai: dashboard laporan, halaman booking hotel, portofolio personal, dan aplikasi baca novel. Setiap template berdiri sendiri dalam satu file (HTML + CSS + JavaScript inline) tanpa proses build dan tanpa framework.

> Dokumentasi internal projek (log progres, memory, style guide) tersimpan di vault [`obsidian/`](obsidian/).

## 📄 Daftar Template

| # | Template | Kategori | Tema Warna | Versi | Fitur Utama |
|---|----------|----------|------------|-------|-------------|
| 1 | [`marketing-report-deep-ocean.html`](templates/marketing-report-deep-ocean.html) | Marketing Report / Dashboard | Deep Ocean + Light Blue Sky | v1.1.0 | 8 jenis chart SVG murni, KPI count-up, tabel performa kampanye — sepenuhnya offline tanpa dependensi eksternal |
| 2 | [`hotel-booking-golden-hour.html`](templates/hotel-booking-golden-hour.html) | Hotel / Booking | Golden Hour (oranye–kuning) | v1.0.0 | Filter fungsional (fasilitas, tipe kamar, bintang, dual price slider), estimasi harga dinamis dari tanggal & tamu, sort, empty state |
| 3 | [`portfolio-slate-cyan.html`](templates/portfolio-slate-cyan.html) | Portfolio | Slate Cyan (gray–cyan) | v1.0.2 | 6 section (Hero–Contact), scrollspy, skill bar animasi, form kontak demo mailto, sosial media |
| 4 | [`e-novel-maroon-gray.html`](templates/e-novel-maroon-gray.html) | E-Novel / Reading App | Maroon Gray | v1.0.0 | Dark mode, search filter buku, reading progress, daftar penulis trending & novel terbaru |

## ✨ Karakter Umum

- **Single-file** — HTML + CSS + JS inline, tanpa build step, tanpa framework; cukup buka di browser
- **Responsif** — pendekatan mobile-first dengan CSS Grid/Flexbox
- **Anti AI-slop** — flat color, palet warna terbatas, garis 1px, radius kecil, tanpa gradien berlebih/glassmorphism
- **Vanilla JavaScript** — dibungkus IIFE, kompatibel dengan browser modern
- **Animasi seperlunya** — halus dan menghormati `prefers-reduced-motion`
- **Ikon hemat** — Font Awesome 6 free (seperlunya); ikon brand yang tidak tersedia di FA free (mis. Fiverr) memakai inline SVG dari Simple Icons (CC0)
- **Konten sample** — gambar dari Unsplash (free license), semua URL terverifikasi; data (hotel, novel, klien) bersifat fiktif

## 📁 Struktur Projek

```
template_html/
├── AGENTS.md                  # Aturan kerja untuk AI agents
├── README.md                  # File ini
├── obsidian/                  # Vault dokumentasi
│   ├── HUB.md                 # Pusat informasi projek
│   ├── 01 - Log/              # Log progres harian
│   ├── 02 - Templates List/   # Indeks & dokumentasi tiap template
│   ├── 03 - Memory/           # Keputusan penting & pembelajaran
│   └── 04 - Documentation/    # Style guide
└── templates/                 # SEMUA output template HTML
    ├── e-novel-maroon-gray.html
    ├── hotel-booking-golden-hour.html
    ├── marketing-report-deep-ocean.html
    └── portfolio-slate-cyan.html
```

## 🚀 Cara Menggunakan

1. Clone repository:

   ```bash
   git clone https://github.com/tinozservice/template_html.git
   ```

2. Buka template langsung — klik dua kali file di folder `templates/`, atau:

   ```bash
   python -m http.server 8000
   # lalu buka http://localhost:8000/templates/portfolio-slate-cyan.html
   ```

3. Sesuaikan konten — semua warna memakai CSS Custom Properties di `:root`, jadi tema mudah diganti dari satu tempat.

## 📐 Konvensi

- Nama file: `purpose-theme.html` — tema warna selalu di kata akhir (contoh: `hotel-booking-golden-hour.html`)
- **Dilarang** memakai nama `index.html`
- Semua output template disimpan di `templates/`, bukan di root projek
- Template baru diprioritaskan single-file; aset pendukung (opsional) di subfolder template
- Setiap penambahan/perubahan template wajib dicatat di vault `obsidian/` — aturan lengkap ada di [`AGENTS.md`](AGENTS.md)

## 🗂 Dokumentasi (Vault Obsidian)

| Dokumen | Isi |
|---------|-----|
| [`HUB.md`](obsidian/HUB.md) | Pusat informasi & status projek |
| [`Progress Log.md`](obsidian/01%20-%20Log/Progress%20Log.md) | Log progres dan revisi |
| [`Templates Index.md`](obsidian/02%20-%20Templates%20List/Templates%20Index.md) | Indeks lengkap + dokumentasi per template |
| [`Project Memory.md`](obsidian/03%20-%20Memory/Project%20Memory.md) | Keputusan penting, konvensi, dan pelajaran |
| [`Style Guide.md`](obsidian/04%20-%20Documentation/Style%20Guide.md) | Panduan gaya penulisan & referensi palet warna |

## 📜 Kredit & Lisensi

- **Template** — bebas dipakai dan dimodifikasi
- **Gambar** — [Unsplash](https://unsplash.com/license) (free license)
- **Ikon** — [Font Awesome 6 Free](https://fontawesome.com) dan [Simple Icons](https://simpleicons.org) (CC0)
- **Font** — [Google Fonts](https://fonts.google.com) sesuai tema masing-masing template
