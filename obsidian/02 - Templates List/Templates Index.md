# 📄 Templates Index

> **Daftar semua template HTML yang tersedia di projek ini**
> - Update setiap kali ada template baru
> - Gunakan nama file template (tanpa ekstensi .html)
> - Link ke dokumentasi tiap template

## 📋 Daftar Template

### 🎨 Portfolio
| Nama Template | Status | Tanggal Dibuat | Versi | Link |
|---------------|--------|----------------|-------|------|
| - | - | - | - | - |

### 💼 Landing Page
| Nama Template | Status | Tanggal Dibuat | Versi | Link |
|---------------|--------|----------------|-------|------|
| - | - | - | - | - |

### 📝 Blog
| Nama Template | Status | Tanggal Dibuat | Versi | Link |
|---------------|--------|----------------|-------|------|
| - | - | - | - | - |

### 🛍 E-commerce
| Nama Template | Status | Tanggal Dibuat | Versi | Link |
|---------------|--------|----------------|-------|------|
| - | - | - | - | - |

### 📊 Marketing Report
| Nama Template | Status | Tanggal Dibuat | Versi | Link |
|---------------|--------|----------------|-------|------|
| marketing-report | ✅ Selesai | 2026-10-06 | v1.1.0 | [[marketing-report]] |

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

## 📊 Marketing Report

- **File**: `templates/marketing-report.html`
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
![[preview-marketing-report.png]]

### Link Terkait
- [[Progress Log]]