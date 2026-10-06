# 🧠 Project Memory

> **Memory jangka panjang projek template HTML**
> - Simpan keputusan penting, pola kerja, dan pembelajaran
> - Baca ini sebelum memulai pekerjaan baru

## 💡 Keputusan Penting

### # 2026-10-06 - Direktori output `templates/`
**Konteks**: File template yang diletakkan langsung di root membuat struktur projek terlihat berantakan.
**Keputusan**: Semua output template HTML disimpan di direktori khusus `templates/` (aturan ditambahkan ke `AGENTS.md`).
**Dampak**: Root projek hanya berisi `AGENTS.md`, `obsidian/`, dan `templates/`. Semua template lama dipindahkan ke `templates/`.
**Referensi**: [[Templates Index]], [[Style Guide]]

---

### # 2026-10-06 - Gaya desain anti AI-slop (editorial report)
**Konteks**: Desain awal memakai banyak gradien, glow, glassmorphism, dan radius besar yang tampak generic/AI-generated.
**Keputusan**: Beralih ke gaya *editorial report*: flat color, palet monokromatik Deep Ocean → Light Blue Sky, garis tipis 1px, radius 2–4px, tipografi tegas dengan aksen monospace, menerima `prefers-reduced-motion`.
**Dampak**: Template tampak lebih natural, profesional, dan punya karakter; jadi acuan desain template berikutnya.
**Referensi**: [[marketing-report]], [[Style Guide]]

---

### # 2026-10-06 - Tema warna Deep Ocean + Light Blue Sky
**Konteks**: Pembuatan template dashboard Marketing Report memerlukan identitas warna yang konsisten dan profesional.
**Keputusan**: Menggunakan palet dua tema — Deep Ocean sebagai tinta (`#0b2b3f`, `#0f4c75`, `#1f6f9e`) dan Light Blue Sky sebagai tint (`#3f8fba`, `#6fb3d6`, `#a8d0e8`, `#eef4f8`), dengan aksen hemat teal/amber/coral.
**Dampak**: Semua template bertema serupa memakai variabel CSS yang sama agar konsisten; mudah diubah via `:root`.
**Referensi**: [[marketing-report]]

---

### # 2026-10-06 - Chart tanpa dependensi eksternal
**Konteks**: Template harus portabel dan bisa dibuka langsung tanpa internet.
**Keputusan**: Semua chart (line, area, bar, horizontal bar, donut, funnel, gauge, sparkline) dibangun dengan SVG + vanilla JS, bukan library eksternal seperti Chart.js.
**Dampak**: File tunggal, ringan, tanpa CDN; animasi & tooltip dikontrol sendiri.
**Referensi**: [[marketing-report]]

---

### # 2026-10-06 - Tema warna Golden Hour (oranye–kuning) & dependensi eksternal
**Konteks**: Pembuatan template hotel booking memerlukan identitas warna hangat (orange, yellow, dan turunannya).
**Keputusan**: Palet Golden Hour — oranye `#A84A0F`/`#C25A14`/`#7C350B`, kuning-amber `#E2A23C`/`#F0C87E`/`#F5E3C2`, netral krem `#FAF6EE`/`#FDF4E3`/`#FFFDF8`, tinta hangat `#31241A`. Tipografi: Fraunces (display), Inter (body), IBM Plex Mono (angka/harga). Template ini memakai dependensi eksternal (Google Fonts, Font Awesome 6 seperlunya, foto kamar Unsplash) — berbeda dari marketing-report yang sepenuhnya offline.
**Dampak**: Template bertema hangat berikutnya memakai variabel CSS yang sama; prinsip anti AI-slop tetap dipertahankan (tanpa gradien, tanpa glow, radius ≤ 6px).
**Referensi**: [[hotel-booking-golden-hour]], [[Style Guide]]

---

### # 2026-10-06 - Tema warna Slate Cyan (gray–cyan) & pola animasi ringan
**Konteks**: Pembuatan template portfolio memerlukan identitas warna dingin (gray, cyan, dan turunannya).
**Keputusan**: Palet Slate Cyan — slate netral `#16202B`/`#4C5A6A`/`#6B7887`, garis `#DEE5EA`/`#EBF0F3`, background `#F7F9FA`, cyan `#0F7387`/`#12879D`/`#1FA0B5` dengan tint `#DFF2F6`/`#F0F9FB`. Tipografi: Space Grotesk (display), Inter (body), IBM Plex Mono (label/angka). Pola interaksi ringan: scrollspy navbar (IntersectionObserver), reveal-on-scroll, progress bar skill yang terisi saat terlihat — semuanya dinonaktifkan dengan `prefers-reduced-motion`.
**Dampak**: Template portfolio berikutnya memakai variabel CSS yang sama; trik `html.js` dipakai agar konten tetap terlihat bila JavaScript mati.
**Referensi**: [[portfolio-slate-cyan]], [[Style Guide]]

---

### # YYYY-MM-DD - Deskripsi keputusan
**Konteks**: 
**Keputusan**: 
**Dampak**: 
**Referensi**: 

---

## 🔄 Pola Kerja yang Terbukti

### Penamaan Template
- Gunakan format: `style-theme-purpose.html` (contoh: `minimal-blog.html`)
- Hindari nama generik seperti `index.html` atau `template.html`

### Struktur HTML
- Gunakan semantic HTML5
- Sertakan meta tags untuk SEO
- Responsive dengan CSS Grid/Flexbox

---

## 📚 Pembelajaran

### Pelajaran 1
- **Masalah**: Blok aksen foto yang diposisikan absolut terhadap seluruh `figure` (termasuk area figcaption) membuat caption tampak "terpleset" keluar dari foto dan mengambang di atas blok aksen.
- **Solusi**: Batasi elemen dekoratif (offset accent block) di dalam wrapper khusus yang hanya membungkus foto (`photo-wrap`), lalu beri jarak caption dari tepi aksen agar duduk bersih di atas background halaman. Terapkan pada [[portfolio-slate-cyan]].
- **Referensi**: [[portfolio-slate-cyan]]

---

## ⚠️ Hal yang Perlu Dihindari

- Scanning folder secara massal tanpa kebutuan
- Membuat file `index.html`
- Duplikasi kode antar template
- Mengabaulkan update vault Obsidian

---

## 🔧 Konvensi Kode

### CSS
- Gunakan CSS reset modern
- Prefer CSS variables untuk tema
- Responsive mobile-first

### JavaScript
- Vanilla JS bila memungkinkan
- Gunakan IIFE untuk scoping
- Kompatibel dengan browser modern

### HTML
- Validasi W3C
- Accessibility (ARIA)
- Semantic tags