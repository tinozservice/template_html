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
**Referensi**: [[marketing-report-deep-ocean]], [[Style Guide]]

---

### # 2026-10-06 - Tema warna Deep Ocean + Light Blue Sky
**Konteks**: Pembuatan template dashboard Marketing Report memerlukan identitas warna yang konsisten dan profesional.
**Keputusan**: Menggunakan palet dua tema — Deep Ocean sebagai tinta (`#0b2b3f`, `#0f4c75`, `#1f6f9e`) dan Light Blue Sky sebagai tint (`#3f8fba`, `#6fb3d6`, `#a8d0e8`, `#eef4f8`), dengan aksen hemat teal/amber/coral.
**Dampak**: Semua template bertema serupa memakai variabel CSS yang sama agar konsisten; mudah diubah via `:root`.
**Referensi**: [[marketing-report-deep-ocean]]

---

### # 2026-10-06 - Chart tanpa dependensi eksternal
**Konteks**: Template harus portabel dan bisa dibuka langsung tanpa internet.
**Keputusan**: Semua chart (line, area, bar, horizontal bar, donut, funnel, gauge, sparkline) dibangun dengan SVG + vanilla JS, bukan library eksternal seperti Chart.js.
**Dampak**: File tunggal, ringan, tanpa CDN; animasi & tooltip dikontrol sendiri.
**Referensi**: [[marketing-report-deep-ocean]]

---

### # 2026-10-06 - Tema warna Golden Hour (oranye–kuning) & dependensi eksternal
**Konteks**: Pembuatan template hotel booking memerlukan identitas warna hangat (orange, yellow, dan turunannya).
**Keputusan**: Palet Golden Hour — oranye `#A84A0F`/`#C25A14`/`#7C350B`, kuning-amber `#E2A23C`/`#F0C87E`/`#F5E3C2`, netral krem `#FAF6EE`/`#FDF4E3`/`#FFFDF8`, tinta hangat `#31241A`. Tipografi: Fraunces (display), Inter (body), IBM Plex Mono (angka/harga). Template ini memakai dependensi eksternal (Google Fonts, Font Awesome 6 seperlunya, foto kamar Unsplash) — berbeda dari marketing-report-deep-ocean yang sepenuhnya offline.
**Dampak**: Template bertema hangat berikutnya memakai variabel CSS yang sama; prinsip anti AI-slop tetap dipertahankan (tanpa gradien, tanpa glow, radius ≤ 6px).
**Referensi**: [[hotel-booking-golden-hour]], [[Style Guide]]

---

### # 2026-10-06 - Tema warna Slate Cyan (gray–cyan) & pola animasi ringan
**Konteks**: Pembuatan template portfolio memerlukan identitas warna dingin (gray, cyan, dan turunannya).
**Keputusan**: Palet Slate Cyan — slate netral `#16202B`/`#4C5A6A`/`#6B7887`, garis `#DEE5EA`/`#EBF0F3`, background `#F7F9FA`, cyan `#0F7387`/`#12879D`/`#1FA0B5` dengan tint `#DFF2F6`/`#F0F9FB`. Tipografi: Space Grotesk (display), Inter (body), IBM Plex Mono (label/angka). Pola interaksi ringan: scrollspy navbar (IntersectionObserver), reveal-on-scroll, progress bar skill yang terisi saat terlihat — semuanya dinonaktifkan dengan `prefers-reduced-motion`.
**Dampak**: Template portfolio berikutnya memakai variabel CSS yang sama; trik `html.js` dipakai agar konten tetap terlihat bila JavaScript mati.
**Referensi**: [[portfolio-slate-cyan]], [[Style Guide]]

---

### # 2026-10-06 - Konvensi penamaan template: akhiri dengan tema warna
**Konteks**: User ingin nama file template mencantumkan tema warna di kata akhir agar konsisten, seperti `hotel-booking-golden-hour` dan `portfolio-slate-cyan`.
**Keputusan**: Format nama template: `purpose-theme.html` (tema di kata akhir). `marketing-report.html` di-rename menjadi `marketing-report-deep-ocean.html` (tema Deep Ocean + Light Blue Sky) dengan `git mv` agar riwayat terjaga.
**Dampak**: Semua template baru wajib mengikuti format ini; referensi lama di vault (AGENTS.md, HUB, Log, Templates Index, Style Guide) diperbarui.
**Referensi**: [[marketing-report-deep-ocean]], [[Templates Index]]

---

### # 2026-10-06 - Tema warna Maroon Gray (maroon–gray) + dark mode
**Konteks**: Pembuatan template E-Novel memerlukan identitas warna maroon + gray dan dukungan tampilan gelap seperti pada referensi screenshot.
**Keputusan**: Palet Maroon Gray — maroon `#4C1119`/`#6B1620`/`#8A1F2D`/`#A62B3C` dengan tint `#F3DDE1`/`#FBF0F2`; netral `#2A272E`/`#6B6770`/`#8A8691`, garis `#E4E1E6`/`#EFEDF1`, background `#F5F4F6`. Tipografi: Outfit (display), Inter (body), IBM Plex Mono (angka). Dark mode via override CSS variables pada `body.dark` + tombol toggle (tanpa localStorage).
**Dampak**: Pola dark mode ini bisa dipakai ulang untuk template app-like berikutnya; pill radius hanya untuk tab & tombol follow, sisanya radius kecil (anti AI-slop).
**Referensi**: [[e-novel-maroon-gray]], [[Style Guide]]

---

### # 2026-10-07 - Tema warna Go Green (hijau) & pola landing page konversi
**Konteks**: Pembuatan template landing page ISP fiber fiktif "FiberIndo" memerlukan identitas hijau (go green) sekaligus pola konversi lengkap (harga, perbandingan, Q&A, cek ketersediaan).
**Keputusan**: Palet Go Green — hijau aksi `#176B40` (hover `#115230`), hijau grafik `#2E9E67` (+ sekunder `#8CCBA6`), band gelap `#0E3F26`, tint `#D9EFE1`/`#E9F5EE`; netral page `#F6FAF7`, panel `#FFFFFF`/`#EFF6F1`, garis `#DCE8DF`; tinta `#11251B`, sekunder `#3E5949`, muted `#5C7367` (digelapkan dari `#6E8377` setelah audit kontras Lighthouse). Tipografi: Sora (display), Inter (body), IBM Plex Mono (angka/harga). Toggle harga bulanan/tahunan via atribut `data-monthly`/`data-annual` pada kartu paket.
**Dampak**: Ramp hijau siap dipakai untuk template bertema hijau berikutnya; prinsip anti AI-slop dipertahankan (tanpa gradien, radius ≤ 6px, chart SVG murni). Muted `#5C7367` menjadi batas aman teks kecil 12–13px di latar terang.
**Referensi**: [[landing-fiber-optik-go-green]], [[Style Guide]]

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

### Pelajaran 2
- **Masalah**: (1) Saat mengunduh gambar stok via loop PowerShell, URL `"photo-$id?auto=..."` rusak — PowerShell membaca `$id?auto` sebagai satu nama variabel sehingga hasilnya 404. (2) ID foto Unsplash yang dipilih dari ingatan bisa salah konten (mis. foto uang atau orang di depan komputer, bukan buku).
- **Solusi**: (1) Selalu bungkus nama variabel dengan `${}` sebelum karakter `?` pada URL: `photo-${id}?auto=...`. (2) Verifikasi visual gambar sebelum dipakai: unduh versi kecil (`w=160&q=40`), inspeksi satu per satu, baru tulis URL ke template. (3) Cek massal semua URL gambar template dengan curl (`-sL`, harus 200) sebelum review.
- **Referensi**: [[e-novel-maroon-gray]]

### Pelajaran 3
- **Masalah**: Gambar dengan atribut `width`/`height` dirender sangat vertikal (mis. cover buku 174×600) karena atribut `height` berlaku sebagai tinggi tetap dan mengalahkan `aspect-ratio` CSS bila CSS tidak menetapkan `height`. Terbukti di browser user: `aspect-ratio: 2/3` terabaikan, tinggi mengikuti atribut (600px).
- **Solusi**: Selalu tulis `height: auto` pada selector gambar yang rasionya dikontrol CSS (`width: 100%; height: auto; aspect-ratio: ...; object-fit: cover;`). Hasil audit: hotel aman (tinggi eksplisit), marketing-report tanpa gambar, portfolio & e-novel diperbaiki dan diverifikasi via browser (hero 398×498, projek 357×238, cover 174×232).
- **Referensi**: [[portfolio-slate-cyan]], [[e-novel-maroon-gray]]

### Pelajaran 4
- **Masalah**: Ikon `fa-fiverr` tidak dirender (kotak kosong) karena brand Fiverr tidak tersedia di Font Awesome 6 free — dikonfirmasi tidak ada di 6.5.2 maupun 6.7.2.
- **Solusi**: Untuk brand yang tidak ada di FA free, gunakan inline SVG resmi dari Simple Icons (CC0) dengan `fill="currentColor"` agar mengikuti warna tema. Biasakan audit kelas `fa-*` template terhadap file CSS FA (cek keberadaan `.<kelas>:before`) untuk mendeteksi ikon hilang sebelum review.
- **Referensi**: [[portfolio-slate-cyan]]

### Pelajaran 5
- **Masalah**: Saat verifikasi visual lewat browser otomasi, jendela browser kadang tidak terlihat/terfokus — rendering dijeda sehingga `requestAnimationFrame` dan callback `IntersectionObserver` tidak berjalan; elemen reveal & chart tampak "tidak muncul" padahal logikanya benar (false alarm).
- **Solusi**: Pastikan jendela browser terlihat/fokus untuk verifikasi visual (reveal, chart, animated). Verifikasi interaksi DOM murni (toggle harga, accordion, toast form) tetap valid tanpa rendering. Lighthouse tetap bisa dipakai karena ia melakukan render sendiri. Untuk test scroll terjadwal, matikan dulu `scroll-behavior: smooth` agar `scrollTo` instan.
- **Referensi**: [[landing-fiber-optik-go-green]]

### Pelajaran 6
- **Masalah**: Bar cakupan kota (`.cov-fill`) tidak terlihat sama sekali; semua track tampak identik. Root cause: elemen `<span>` bersifat `display: inline`, sehingga `width`/`height` diabaikan. Track lolos karena sebagai grid item otomatis di-blockify, tetapi fill di dalamnya tetap inline.
- **Solusi**: Beri `display: block` (atau `inline-block`) pada elemen inline yang diberi dimensi. Verifikasi memakai `getBoundingClientRect()` (geometri terkomputasi) — mengecek atribut `style`/`cssText` saja bisa memberi false positive (nilai benar, layout tidak menerapkan).
- **Referensi**: [[landing-fiber-optik-go-green]]

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