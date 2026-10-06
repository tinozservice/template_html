# 📐 Style Guide - Template HTML

> **Panduan gaya dan konvensi penulisan kode template HTML**
> - Ikuti panduan ini untuk konsistensi semua template

## 📁 Struktur File Template

### Struktur Projek (Output)
Semua output template disimpan di direktori `templates/`, bukan di root projek.
```
template-html/
├── AGENTS.md
├── obsidian/                # Vault dokumentasi (HUB, Log, Memory, dsb)
└── templates/               # SEMUA output template HTML
    └── nama-template.html
```

### Struktur Template Tunggal (single-file, direkomendasikan)
Template dapat berdiri sendiri dalam satu file HTML (HTML + CSS + JS inline), tanpa dependensi eksternal.
```
templates/
└── nama-template.html
```

### Struktur Template Multi-File (opsional)
Jika template memerlukan aset terpisah, gunakan subfolder di dalam template.
```
templates/
└── nama-template/
    ├── nama-template.html   # File utama template
    ├── css/
    │   └── style.css        # CSS utama
    ├── js/
    │   └── script.js        # JavaScript (jika diperlukan)
    └── assets/
        ├── images/
        ├── fonts/
        └── icons/
```

## 💻 Konvensi HTML

### Doctype & Meta Tags
```html
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Deskripsi template ini">
    <title>Nama Template - VibeCode Template</title>
</head>
```

### Struktur Semantic
```html
<header>
    <nav>...</nav>
</header>

<main>
    <section>...</section>
    <article>...</article>
</main>

<footer>...</footer>
```

### CSS
```css
/* Gunakan CSS Custom Properties */
:root {
    --primary-color: #007bff;
    --secondary-color: #6c757d;
}

/* Mobile-first approach */
@media (min-width: 768px) {
    /* Desktop styles */
}
```

### JavaScript
```javascript
// Gunakan IIFE untuk scoping
(function() {
    'use strict';
    
    // Kode Anda di sini
})();
```

## 🎨 Panduan Desain

### Color Palette
- Primary: `#007bff`
- Secondary: `#6c757d`
- Success: `#28a745`
- Background: `#ffffff`
- Text: `#212529`

### Tema Referensi — Deep Ocean + Light Blue Sky
Dipakai oleh [[marketing-report]]; dapat dijadikan acuan untuk template bertema serupa.
- Deep Ocean (tinta): `#0b2b3f`, `#0f4c75`, `#1f6f9e`
- Light Blue Sky (tint): `#3f8fba`, `#6fb3d6`, `#a8d0e8`, `#eef4f8`
- Aksen hemat: teal `#2f8f83`, amber `#b9822f`, coral `#b0505f`

### Tema Referensi — Golden Hour (Orange–Kuning)
Dipakai oleh [[hotel-booking-golden-hour]]; dapat dijadikan acuan untuk template bertema hangat.
- Oranye: `#A84A0F` (aksi/tombol), `#C25A14` (aksen), `#7C350B` (hover)
- Kuning-amber: `#E2A23C` (highlight, bintang), `#F0C87E` (soft), `#F5E3C2` (tint)
- Netral krem: `#FAF6EE` (page), `#FDF4E3` (tint panel), `#FFFDF8` (panel harga), `#E9DCC5` (garis)
- Tinta hangat: `#31241A` (teks), `#5E4B39` (sekunder), `#7E6A54` (muted)
- Tipografi: Fraunces (display serif), Inter (body), IBM Plex Mono (angka/harga); ikon Font Awesome seperlunya

### Tema Referensi — Slate Cyan (Gray–Cyan)
Dipakai oleh [[portfolio-slate-cyan]]; dapat dijadikan acuan untuk template bertema dingin/tech.
- Slate netral: `#16202B` (tinta), `#33404E` (sekunder), `#4C5A6A` (slate), `#6B7887` (muted)
- Garis & latar: `#DEE5EA` (garis), `#EBF0F3` (garis soft), `#F7F9FA` (page), `#F1F5F7` (panel), `#FFFFFF` (kartu)
- Cyan: `#0F7387` (aksi), `#12879D` (aksen), `#1FA0B5` (terang), `#BFE5EC`/`#DFF2F6`/`#F0F9FB` (tint)
- Tipografi: Space Grotesk (display), Inter (body), IBM Plex Mono (label/angka); ikon Font Awesome seperlunya

### Prinsip Anti AI-Slop (WAJIB)
- Hindari gradien berlebihan dan warna rainbow; gunakan palet terbatas / ramp satu hue
- Hindari shadow berlapis, glow neon, dan glassmorphism (`backdrop-filter: blur`)
- Batasi `border-radius` (mis. 2–4px); hindari `999px` di mana-mana
- Utamakan flat color, garis tipis (1px), dan whitespace yang lapang
- Tipografi tegas: hierarki jelas, boleh memakai aksen monospace untuk angka/label
- Animasi seperlunya dan halus; hormati `prefers-reduced-motion`

### Typography
- Font utama: `Inter, system-ui, sans-serif`
- Ukuran dasar: `16px`
- Line-height: `1.6`

## ✅ Checklist Sebelum Commit

- [ ] Nama file sesuai pedoman (bukan `index.html`)
- [ ] Validasi HTML di [W3C Validator](https://validator.w3.org/)
- [ ] Responsive di berbagai ukuran layar
- [ ] Update vault Obsidian (Log, Templates Index, Memory)
- [ ] Dokumentasi lengkap di folder Documentation