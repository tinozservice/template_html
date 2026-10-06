# AGENTS.md - Aturan untuk AI Agents

## Tujuan Projek
Projek ini bertujuan untuk menghasilkan template dalam bentuk HTML.

## Aturan Penamaan File
- **DILARANG** memberi nama file HTML dengan nama `index.html`
- Beri nama file sesuai dengan nama template atau style tema yang dihasilkan
- Contoh: `portfolio-modern.html`, `landing-page-corporate.html`, `blog-minimal.html`

## Struktur Direktori Output (Rekomendasi)
- **WAJIB**: semua file template HTML disimpan di dalam direktori khusus `templates/`
- **DILARANG** menyimpan file template langsung di root projek, agar root tetap bersih
- Struktur yang direkomendasikan:
  ```
  template-html/
  ├── AGENTS.md
  ├── obsidian/            # Vault dokumentasi (HUB, Log, Memory, dsb)
  └── templates/           # SEMUA output template HTML
      ├── marketing-report-deep-ocean.html
      └── ...
  ```
- Aset pendukung (jika ada) disimpan di subfolder di dalam template masing-masing, contoh: `templates/marketing-report-deep-ocean/assets/`
- Nama direktori lain yang dapat dipakai: `output/` atau `dist/`. Jika memilih nama berbeda, gunakan satu nama secara konsisten di seluruh projek
- Setiap penambahan/pemindahan template wajib diperbarui di vault Obsidian (khususnya [[Templates Index]])

## Penggunaan Vault Obsidian
- **Vault Obsidian** berfungsi sebagai:
  - Log progres pengerjaan template
  - HUB (pusat informasi) projek
  - Memory jangka panjang projek
  - Data list semua template yang dihasilkan
  - Dokumentasi dan catatan teknis
- Semua agent AI harus memprioritaskan membaca Log dan HUB yang ada di vault Obsidian
- Update vault Obsidian secara reguler dengan progres dan temuan baru

## Aturan Akses Folder
- **DILARANG** membaca seluruh folder secara massal tanpa alasan yang jelas
- Agent AI hanya boleh mengakses/membaca folder yang relevan dengan tugasnya
- **Prioritas utama**: Log dan HUB yang ada di vault Obsidian
- Pastikan untuk memeriksa vault Obsidian terlebih dahulu sebelum mengeksplorasi struktur folder lainnya

## Kontribusi
- Setiap perubahan atau penambahan template harus dicatat di vault Obsidian
- Patuhi konvensi penamaan yang telah ditetapkan
- Jaga dokumentasi di vault tetap up-to-date

## Penghindaran Desain AI Slop
- **DILARANG** menggunakan desain yang khas AI-generated slop
  - Gradien warna berlebihan (terutama rainbow/linear gradient yang berulang)
  - Pola desain yang terlalu khas AI (shadow berlapis, border-radius berlebihan)
  - Styling yang terlalu generic dan over-designed
- Buat desain yang natural, minimalis, dan memiliki karakter unik
- Fokus pada fungsionalitas dan estetika yang bersih