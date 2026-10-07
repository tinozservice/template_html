# 📄 Templates Index

> **Daftar semua template HTML yang tersedia di projek ini**
> - Update setiap kali ada template baru
> - Gunakan nama file template (tanpa ekstensi .html)
> - Link ke dokumentasi tiap template

## 📋 Daftar Template

### 🎨 Portfolio
| Nama Template | Status | Tanggal Dibuat | Versi | Link |
|---------------|--------|----------------|-------|------|
| portfolio-slate-cyan | ✅ Selesai | 2026-10-06 | v1.0.2 | [[portfolio-slate-cyan]] |

### 💼 Landing Page
| Nama Template | Status | Tanggal Dibuat | Versi | Link |
|---------------|--------|----------------|-------|------|
| landing-fiber-optik-go-green | ✅ Selesai | 2026-10-07 | v1.0.1 | [[landing-fiber-optik-go-green]] |

### 📝 Blog
| Nama Template | Status | Tanggal Dibuat | Versi | Link |
|---------------|--------|----------------|-------|------|
| news-blog-noir-maroon | ✅ Selesai | 2026-10-07 | v1.0.0 | [[news-blog-noir-maroon]] |

### 🛍 E-commerce
| Nama Template | Status | Tanggal Dibuat | Versi | Link |
|---------------|--------|----------------|-------|------|
| ecommerce-ez-fresh-orange-yellow | ✅ Selesai | 2026-10-07 | v1.0.0 | [[ecommerce-ez-fresh-orange-yellow]] |

### 📚 E-Novel
| Nama Template | Status | Tanggal Dibuat | Versi | Link |
|---------------|--------|----------------|-------|------|
| e-novel-maroon-gray | ✅ Selesai | 2026-10-06 | v1.0.0 | [[e-novel-maroon-gray]] |

### 🏨 Hotel / Booking
| Nama Template | Status | Tanggal Dibuat | Versi | Link |
|---------------|--------|----------------|-------|------|
| hotel-booking-golden-hour | ✅ Selesai | 2026-10-06 | v1.0.0 | [[hotel-booking-golden-hour]] |

### 📊 Marketing Report
| Nama Template | Status | Tanggal Dibuat | Versi | Link |
|---------------|--------|----------------|-------|------|
| marketing-report-deep-ocean | ✅ Selesai | 2026-10-06 | v1.1.0 | [[marketing-report-deep-ocean]] |

## ➕ Cara Menambahkan Template Baru

1. Buat file template di dalam direktori `templates/` (bukan root projek)
2. Beri nama sesuai dengan style tema (contoh: `portfolio-modern.html`)
3. Buat dokumentasi template di folder ini
4. Update status di tabel di atas

## 📝 Template Dokumentasi Per Template

```
## Nama Template
- **File**: `nama-template.html`
- **Kategori**: Portfolio/Landing Page/Blog/E-commerce
- **Tanggal**: YYYY-MM-DD
- **Versi**: v1.0.0
- **Status**: ✅ Selesai / 🔄 Dalam pengerjaan / ❌ Dibatalkan

### Deskripsi
Deskripsi singkat template ini

### Fitur
- Fitur 1
- Fitur 2

### Teknologi
- HTML
- CSS
- (JavaScript jika ada)

### Preview
![[preview-screenshot.png]]

### Link Terkait
- [[Log/YYYY-MM-DD]]
```

---

## 📊 Marketing Report — Deep Ocean

- **File**: `templates/marketing-report-deep-ocean.html`
- **Kategori**: Marketing Report / Dashboard
- **Tanggal**: 2026-10-06
- **Versi**: v1.1.0
- **Status**: ✅ Selesai

### Deskripsi
Laporan pemasaran satu halaman bergaya **editorial report** dengan tema warna **Deep Ocean** (tinta) dan **Light Blue Sky** (tint). Desain flat dan minimalis: tanpa gradien berlebih, tanpa glassmorphism/glow, border-radius kecil, dan tipografi tegas dengan aksen monospace. Menampilkan performa kampanye, kanal, dan audiens melalui berbagai jenis chart.

### Fitur
- Masthead dokumen dengan periode, penyusun, dan tanggal
- 4 KPI (Revenue, Leads, Conversion Rate, ROAS) dengan animasi count-up + sparkline
- Line/Area chart: Tren Revenue vs Ad Spend
- Donut chart: Sumber Trafik dengan legend monokromatik
- Bar chart: Penjualan per Kanal
- Horizontal bar chart: Top Campaigns
- Area chart: Engagement Rate Harian
- Conversion Funnel
- Radial gauge: Skor Kesehatan Kampanye (Reach, Engagement, Efficiency)
- Tabel detail performa 9 kampanye dengan progress bar & status
- Tooltip interaktif, responsif (mobile-first), dukungan `prefers-reduced-motion`

### Catatan Desain
- Palet dibatasi pada ramp Deep Ocean → Light Blue Sky; warna aksen (teal/amber) dipakai hemat
- Semua chart memakai warna flat (bukan gradient), garis tipis 1px, radius 4px/2px

### Teknologi
- HTML5 semantic
- CSS3 (Custom Properties, Grid, Flexbox, animasi)
- Vanilla JavaScript (IIFE, tanpa dependensi eksternal)
- Chart digambar dengan SVG murni

### Preview
![[preview-marketing-report-deep-ocean.png]]

### Link Terkait
- [[Progress Log]]

---

## 🏨 Hotel Booking — Golden Hour

- **File**: `templates/hotel-booking-golden-hour.html`
- **Kategori**: Hotel / Booking
- **Tanggal**: 2026-10-06
- **Versi**: v1.0.0
- **Status**: ✅ Selesai

### Deskripsi
Halaman pencarian & booking hotel satu file bertema **Golden Hour** — ramp warna oranye → kuning di atas netral krem. Gaya flat: garis 1px, radius kecil (3–6px), tanpa gradien, penggunaan ikon hemat, tipografi Fraunces (display) + Inter (body) + IBM Plex Mono (angka/harga).

### Fitur
- Header: brand "Senja Stays", navigasi Popular / Near Me / Surprise Me, Sign up, Log in
- Sidebar: form Search (Location, Check in, Check out, Guests), Popular Filters, Room Type, Price Range (input min/max + dual slider), Star Rating, Reset
- Kartu hotel: nama, rating (bintang + skor), total review, jarak dari posisi user, chip fasilitas, tipe kamar, kelas kamar, harga per malam, estimasi total dinamis (malam × tamu)
- Filter berfungsi: fasilitas (AND), tipe kamar, bintang, rentang harga + empty state
- Estimasi harga & meta hasil dihitung ulang dari tanggal check-in/check-out dan jumlah tamu
- Sort: Recommended / harga / rating / jarak
- Tombol "Booking Now" hanya sample (menampilkan toast, tidak terhubung ke mana pun)
- Responsif mobile-first, mendukung `prefers-reduced-motion`

### Catatan Desain
- Palet: oranye `#A84A0F`/`#C25A14`, kuning-amber `#E2A23C`/`#F0C87E`, krem `#FAF6EE`/`#FDF4E3`, tinta `#31241A`
- Anti AI-slop: tanpa gradien, tanpa glow/glassmorphism, radius maksimal 6px

### Teknologi
- HTML5 semantic
- CSS3 (Custom Properties, Grid, Flexbox)
- Vanilla JavaScript (IIFE)
- Google Fonts (Fraunces, Inter, IBM Plex Mono), Font Awesome 6 (hemat), foto kamar dari Unsplash

### Preview
![[preview-hotel-booking-golden-hour.png]]

### Link Terkait
- [[Progress Log]]

---

## 🎨 Portfolio — Slate Cyan

- **File**: `templates/portfolio-slate-cyan.html`
- **Kategori**: Portfolio
- **Tanggal**: 2026-10-06
- **Versi**: v1.0.2
- **Status**: ✅ Selesai

### Deskripsi
Portofolio personal satu file bertema **Slate Cyan** — slate netral dingin dipadukan ramp cyan. Gaya flat: garis 1px, radius kecil (3–6px), tanpa gradien/glow, ikon hemat, tipografi Space Grotesk (display) + Inter (body) + IBM Plex Mono (label/angka). Persona sample: "Raka Pratama — Web Designer & Front-end Developer".

### Fitur
- Header: brand/monogram kiri, navbar section kanan (About, Skills, Projects, Services, Contact) dengan **scrollspy**
- **Hero**: badge ketersediaan, nama, role, lead, CTA, stats mono (pengalaman/proyek/klien), foto profil dengan aksen blok flat
- **About**: narasi 2 paragraf + facts grid (lokasi, pengalaman, fokus, mode kerja)
- **Skills**: 6 progress bar yang terisi saat terlihat di viewport
- **Projects**: 3 kartu (gambar, jenis, deskripsi, tag, link "Open case study")
- **Services**: 3 kartu layanan (Web Design, Front-end Development, SEO & Performance) dengan daftar deliverable
- **Contact**: daftar Email / WhatsApp / Telegram + form demo (membuka mailto dengan pesan terisi) + toast
- Footer: kiri brand © 2026 | slogan, kanan 5 sosial media (LinkedIn, Fiverr, Facebook, Instagram, GitHub)
- Reveal-on-scroll halus, responsif mobile-first, mendukung `prefers-reduced-motion`, konten tetap terlihat tanpa JavaScript (`html.js`)

### Catatan Desain
- Palet: slate `#16202B`/`#4C5A6A`, garis `#DEE5EA`, page `#F7F9FA`, cyan `#0F7387`/`#12879D`, tint `#DFF2F6`/`#F0F9FB`
- Anti AI-slop: tanpa gradien, tanpa glow/glassmorphism, radius maksimal 6px
- Semua gambar memakai `height: auto` bersama `aspect-ratio` agar rasio CSS konsisten (fix v1.0.1, hero 4/5 & projek 3/2)
- Ikon Fiverr memakai inline SVG dari Simple Icons (CC0) karena `fa-fiverr` tidak tersedia di Font Awesome free (fix v1.0.2)

### Teknologi
- HTML5 semantic
- CSS3 (Custom Properties, Grid, Flexbox, animasi ringan)
- Vanilla JavaScript (IIFE, IntersectionObserver)
- Google Fonts (Space Grotesk, Inter, IBM Plex Mono), Font Awesome 6 (hemat; ikon Fiverr via inline SVG Simple Icons), foto profil & projek dari Unsplash

### Preview
![[preview-portfolio-slate-cyan.png]]

### Link Terkait
- [[Progress Log]]

---

## 📚 E-Novel — Maroon Gray

- **File**: `templates/e-novel-maroon-gray.html`
- **Kategori**: E-Novel / Reading App
- **Tanggal**: 2026-10-06
- **Versi**: v1.0.0
- **Status**: ✅ Selesai

### Deskripsi
Halaman aplikasi baca novel satu file berdasarkan screenshot referensi, bertema **Maroon Gray** — ramp maroon dipadukan netral abu dingin. Layout app-like: sidebar navigasi, topbar dengan search, grid buku, daftar reading progress, dan rail kanan berisi penulis trending + daftar novel terbaru. Gaya flat: garis 1px, radius kecil (4–9px; pill hanya untuk tab & tombol follow), ikon hemat.

### Fitur
- Sidebar: brand "E-Novel", nav Home (aktif) / Discover / Bookmark / Settings / Help
- Topbar: search **fungsional** (filter buku per judul/penulis), toggle **dark mode**, notifikasi + dot, avatar
- Tab kategori: Popular (aktif) / Top Selling / Following / New + link "Next"
- Grid 10 buku dengan cover rasio 3/4 (judul, penulis) responsif (auto-fill)
- Daftar reading progress: thumbnail, judul, jumlah halaman, progress bar, % (mono)
- Rail kanan: **Trending Author** (5 penulis, tombol Follow/Unfollow berfungsi) dan **Newest Novel** — menggantikan "Popular Blogs" sesuai permintaan, berisi judul, "Published by", jumlah likes/komentar, badge "New"
- Dark mode penuh via `body.dark` (override CSS variables), ikon bulan/matahari
- Responsif mobile-first: sidebar jadi drawer + backdrop, layout rail menurun ke bawah

### Catatan Desain
- Palet: maroon `#4C1119`/`#6B1620`/`#8A1F2D`, gray `#2A272E`/`#6B6770`, background `#F5F4F6`; dark mode `#17151A`
- Anti AI-slop: tanpa gradien/glow, radius maks 9px kecuali pill kontekstual

### Teknologi
- HTML5 semantic
- CSS3 (Custom Properties, Grid, Flexbox, dark mode)
- Vanilla JavaScript (IIFE)
- Google Fonts (Outfit, Inter, IBM Plex Mono), Font Awesome 6 (hemat), gambar dari Unsplash — 22 URL diverifikasi HTTP 200 dan diinspeksi visual sebelum dipakai

### Preview
![[preview-e-novel-maroon-gray.png]]

### Link Terkait
- [[Progress Log]]

---

## 🚀 Landing Page — Fiber Optik Go Green

- **File**: `templates/landing-fiber-optik-go-green.html`
- **Kategori**: Landing Page / ISP Fiber
- **Tanggal**: 2026-10-07
- **Versi**: v1.0.1
- **Status**: ✅ Selesai

### Deskripsi
Landing page satu file untuk ISP fiber fiktif **FiberIndo** bertema **Go Green** — ramp hijau di atas netral mint. Gaya flat anti AI-slop: garis 1px, radius 3–6px, tanpa gradien/glow, ikon hemat, tipografi Sora (display) + Inter (body) + IBM Plex Mono (angka/harga). Berfokus pada alur konversi: keunggulan → bukti performa → cakupan → harga → perbandingan → ulasan → Q&A → cek ketersediaan.

### Fitur
- Header sticky: brand, navbar (scrollspy: Keunggulan, Cakupan, Harga, Perbandingan, Q&A), CTA "Cek ketersediaan", drawer nav di mobile
- **Hero**: headline, CTA, foto router (Unsplash) + caption, 4 stat mono dengan animasi count-up (99,95% uptime, 8 ms, 1 Gbps, 120 rb+)
- Strip jaminan: survei & instalasi gratis, tanpa FUP & kontrak, router WiFi 6 termasuk, dukungan 24/7
- **Keunggulan**: 6 kartu fitur dengan ikon FA (simetris, uptime, latensi, tanpa FUP, WiFi 6, instalasi cepat)
- **Infrastruktur**: split layout dengan foto panel fiber + 4 poin (rute ganda, NOC 24/7, kapasitas kuartalan, perangkat carrier) + chips stat
- **Performa**: 5 visualisasi SVG murni — line/area throughput 24 jam (unduh/unggah), ring uptime 99,95%, mini-stats latensi & jitter
- **Cakupan**: bar ketersediaan per kota (animasi saat terlihat), foto skyline, catatan kota segera hadir
- **Kegunaan**: 3 kartu use case dengan foto (streaming 4K, WFH, gaming & live)
- **Harga**: 4 paket (Lite/Home/Pro/Bisnis) dengan toggle **Bulanan/Tahunan** fungsional + badge "Paling populer"
- **Perbandingan**: tabel vs 2 provider fiktif (rasio unggah, latensi, FUP, kontrak, instalasi, WiFi 6, SLA) + grouped bar kecepatan & horizontal bar harga per Mbps
- **Ulasan**: 3 testimoni dengan avatar Unsplash + rating 4,8/5
- **Q&A**: accordion 8 pertanyaan dengan animasi buka/tutup
- **CTA + form**: form cek ketersediaan demo (validasi + toast personal), kontak telepon/WA 24/7
- Footer 4 kolom + sosial + disclaimer demo; responsif mobile-first, mendukung `prefers-reduced-motion`

### Catatan Desain
- Palet: hijau aksi `#176B40`/`#115230`, grafik `#2E9E67`/`#8CCBA6`, band gelap `#0E3F26`, tint `#D9EFE1`/`#E9F5EE`, netral `#F6FAF7`/`#EFF6F1`, tinta `#11251B`
- Anti AI-slop: tanpa gradien, tanpa glow/glassmorphism, radius maksimal 6px
- Kontras teks kecil diaudit — `--muted` final `#5C7367`; Lighthouse Accessibility/Best Practices/SEO = 100/100/100
- Bar cakupan kota: `.cov-track` & `.cov-fill` wajib `display: block` — elemen `span` inline mengabaikan `width`/`height` (fix v1.0.1, diverifikasi rasio terkomputasi 96/91/88/84/79%)

### Teknologi
- HTML5 semantic
- CSS3 (Custom Properties, Grid, Flexbox, animasi ringan)
- Vanilla JavaScript (IIFE, IntersectionObserver, tanpa dependensi chart)
- Chart digambar dengan SVG murni
- Google Fonts (Sora, Inter, IBM Plex Mono), Font Awesome 6 (hemat, 19 kelas diaudit), foto dari Unsplash (HTTP 200 + inspeksi visual)

### Preview
![[preview-landing-fiber-optik-go-green.png]]

### Link Terkait
- [[Progress Log]]

---

## 📰 News Blog — Noir Maroon

- **File**: `templates/news-blog-noir-maroon.html`
- **Kategori**: Blog / Portal Berita
- **Tanggal**: 2026-10-07
- **Versi**: v1.0.0
- **Status**: ✅ Selesai

### Deskripsi
Portal berita satu file **IndoPress** bertema **Noir Maroon** — gaya klasik koran: putih sebagai kanvas, bar hitam untuk utilitas, maroon untuk navbar dan aksen. Tiga header bertingkat (utility, masthead, navbar sticky), grid berita 15 post yang dapat difilter, dan footer bernavigasi lengkap dengan slot iklan. Tipografi editorial: Source Serif 4 (judul/brand) + Inter (body/UI) + IBM Plex Mono (meta/angka).

### Fitur
- **Header 1 (hitam)**: About, Privacy Policy, Cookies, Advertise, Signup, Login + ikon sosial (X/Twitter, YouTube, Pinterest, feed RSS)
- **Header 2 (masthead putih)**: logo IP + brand IndoPress + slogan, banner iklan contoh 468×90 (menaut ke slot iklan footer)
- **Header 3 (navbar maroon sticky)**: Home, 6 kategori, Latest News, Trending, Author, Contact Us + search box + tombol; drawer menu di mobile
- **Grid berita** (15 post, 6 kategori): thumbnail rasio 3:2, judul di bawah thumbnail, cuplikan (line-clamp), chip kategori + tag yang dapat diklik, avatar & nama penulis, waktu relatif ("5 menit lalu"), total views (ikon mata)
- **Filter fungsional**: kategori (chip filter + link navbar + link footer), tag (#ai, #umkm, dll), penulis (select 6 penulis), pencarian live (judul + cuplikan), sort Terbaru/Terpopuler (segmented + navbar, tersinkron), Load More 9 → 15, empty state + reset
- **Footer**: brand + visi & misi, sosial media, kolom kategori, Help & Support + email redaksi/ads (mailto), newsletter demo (validasi + toast), slot iklan 1:1 (300×300), copyright + legal links
- Toast demo untuk tautan yang belum tersedia; responsif mobile-first; mendukung `prefers-reduced-motion`

### Catatan Desain
- Palet: hitam `#141014`, maroon `#6B1620`/`#4C1119`/`#8A1F2D`/`#A62B3C`, tint `#F7E9EC`/`#FBF3F4`, netral `#FFFFFF`/`#F7F5F6`, garis `#E5DFE1`, muted `#6B5F63`; aksen latar gelap `#D06A7A`
- Anti AI-slop: tanpa gradien, tanpa shadow berlapis, radius 3–4px, garis 1px, ikon FA sangat hemat (9 kelas)
- Rasio penting diverifikasi terkomputasi: thumbnail 3:2 (458×305), avatar 24×24, iklan footer 1:1 (210×210)

### Teknologi
- HTML5 semantic
- CSS3 (Custom Properties, Grid, Flexbox, line-clamp)
- Vanilla JavaScript (IIFE; filter/sort/search/load-more/progressive enhancement — semua kartu ada di HTML)
- Google Fonts (Source Serif 4, Inter, IBM Plex Mono), Font Awesome 6 (hemat), foto & avatar dari Unsplash (HTTP 200 + inspeksi visual)

### Preview
![[preview-news-blog-noir-maroon.png]]

### Link Terkait
- [[Progress Log]]

---

## 🛒 E-Commerce — EZ-Fresh Orange Yellow

- **File**: `templates/ecommerce-ez-fresh-orange-yellow.html`
- **Kategori**: E-commerce / Toko Online
- **Tanggal**: 2026-10-07
- **Versi**: v1.0.0
- **Status**: ✅ Selesai

### Deskripsi
Halaman home toko online satu file **EZ-Fresh** bertema **Orange–Yellow** — kanvas light orange, kartu putih, aksen orange untuk aksi dan kuning untuk sorotan. Konversi dari template **Ogani** (Colorlib, multi-file + jQuery/Bootstrap) menjadi satu file HTML tanpa dependensi JS eksternal; hanya tampilan home yang diambil, tanpa fitur bilingual. Semua gambar dibungkus **thumbnail putih** agar menyatu dengan kanvas berwarna. Tipografi: Poppins (display), Inter (body), IBM Plex Mono (harga/angka).

### Fitur
- **Topbar**: email + info gratis ongkir; sosial media + tombol masuk
- **Header**: logo EZ-Fresh, search box (select kategori + input + tombol), wishlist & keranjang dengan badge angka + total rupiah live (demo)
- **Navbar**: dropdown "Semua Kategori" (6 kategori + jumlah produk), navigasi Home/Kategori/Produk/Promo/Blog/Kontak, chip promo; drawer menu di mobile
- **Hero**: sidebar kategori + carousel 3 slide (autoplay, dots 24px, panah, pause saat hover, hormat `prefers-reduced-motion`)
- **Kategori**: 6 kartu dengan gambar thumbnail putih + jumlah produk (klik → filter)
- **Produk unggulan**: 8 produk dengan tab filter (Semua/Sayuran/Buah/Susu & Telur/Daging & Ikan), badge Terlaris/Diskon/Premium, rating, harga (+ harga coret), tombol favorit (toggle) & tambah ke keranjang (badge + total hidup)
- **Pencarian fungsional**: global atau per kategori (select), empty state + catatan hasil + hapus pencarian
- **Banner promo**: 2 kartu (paket sayur mingguan, jus tanpa gula)
- **Rekomendasi**: 3 kolom (Produk Terbaru, Rating Terbaik, Pilihan Editor) berisi 9 item
- **Blog**: 3 kartu (gambar 3:2, tanggal, komentar, judul, cuplikan, tautan)
- **Footer**: brand + kontak (alamat/telepon/email), tautan, kategori, newsletter demo, sosial media, copyright + metode pembayaran (Visa/Mastercard/PayPal + chip GoPay/OVO/COD)
- Toast demo untuk tautan yang belum tersedia; responsif mobile-first

### Catatan Desain
- Palet final (disetujui user): fill aksi orange `#FFA600` (hover `#F09A00`) — selalu berpasangan dengan teks tinta `#33210F`; teks/ikon di latar terang memakai varian `#9E4E00` (`--orange-ink`); kuning `#FFC65C` untuk CTA/badge (teks tinta); tint `#FFE7D2`/`#FFF3CC`; kanvas `#FFF4E9`; kartu putih; garis `#F0DCC8`/`#E5C7A8`; tinta `#33210F`, sekunder `#6B4F33`, muted `#7E5F44`
- Anti AI-slop: tanpa gradien/glow/shadow, radius 3–6px, garis 1px, ikon FA hemat (26 kelas untuk seluruh halaman)
- Pembungkus `.thumb` putih (`display:block`) untuk semua gambar agar tidak "tabrakan" dengan kanvas light orange
- Rasio terverifikasi: produk 1:1, kategori 1:1, hero & blog 3:2, banner 16:10
- Fix revisi: badge `.count` diberi rule `[hidden] { display:none }` (atribut `hidden` kalah specificity dari `display:inline-grid`); brand "-Fresh" di footer gelap memakai orange terang `#FFA600`

### Teknologi
- HTML5 semantic
- CSS3 (Custom Properties, Grid, Flexbox, line-clamp)
- Vanilla JavaScript (IIFE; carousel, filter, pencarian, keranjang/favorit demo — tanpa jQuery/Bootstrap)
- Google Fonts (Poppins, Inter, IBM Plex Mono), Font Awesome 6 (hemat), 19 foto dari Unsplash (HTTP 200 + inspeksi visual)

### Preview
![[preview-ecommerce-ez-fresh-orange-yellow.png]]

### Link Terkait
- [[Progress Log]]