# 📐 Style Guide - Template HTML

> **Panduan gaya dan konvensi penulisan kode template HTML**
> - Ikuti panduan ini untuk konsistensi semua template

## 📁 Struktur File Template

### Struktur Dasar
```
template-nama/
├── nama-template.html       # File utama template
├── css/
│   ├── style.css           # CSS utama
│   └── reset.css           # CSS reset (opsional)
├── js/
│   └── script.js           # JavaScript (jika diperlukan)
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