# Website Denny Sihombing - Dokumentasi Struktur Baru

## Overview

Website ini telah dikembangkan dengan struktur navigasi yang lebih terorganisir dan scalable untuk mendukung profil akademik yang lebih profesional.

## Struktur Navigasi Baru

### Menu Utama

```
Home
About  → /about/
Teaching → /teaching/
Research → /research/
Resources → /resources/
Contact → /contact.html
```

## Struktur Folder yang Telah Dibuat

### ✅ Sudah Dibuat:

```
/
├── about/
│   └── index.html  (Halaman profil lengkap dengan statistik, expertise, dan koneksi)
├── index.html  (Homepage - perlu diupdate navigasinya)
├── wiki/  (sudah ada)
├── courses  (sudah ada)
├── decision-support-systems.html  (sudah ada)
└── denny.png  (sudah ada)
```

### 🔄 Perlu Dibuat:

```
teaching/
├── index.html  (Halaman utama teaching dengan daftar mata kuliah)
├── decision-support-systems.html  (Detail mata kuliah DSS)
├── machine-learning.html  (Detail mata kuliah Machine Learning)
└── digital-transformation.html  (Detail mata kuliah Digital Transformation)

research/
├── index.html  (Halaman research dengan daftar publikasi & proyek)
└── publications.html  (Daftar lengkap publikasi)

resources/
├── index.html  (Halaman utama resources)
├── wiki.html  (Redirect atau deskripsi Wiki)
└── decision-lab.html  (Deskripsi Decision Lab)

contact.html  (Form kontak / collaboration)
```

## Yang Perlu Dikembangkan

### 1. **Update Homepage (`index.html`)**

**Yang perlu diubah:**
- Update navigasi untuk mengarah ke halaman terpisah (bukan anchor)
- Tambah section "What I Do" dengan 3 pilar utama
- Perbaiki CTA (Call-to-Action) yang lebih spesifik

**Navigasi baru:**
```html
<ul class="nav-links">
    <li><a href="/">Home</a></li>
    <li><a href="/about/">About</a></li>
    <li><a href="/teaching/">Teaching</a></li>
    <li><a href="/research/">Research</a></li>
    <li><a href="/resources/">Resources</a></li>
    <li><a href="/contact.html">Contact</a></li>
</ul>
```

### 2. **Halaman Teaching**

**teaching/index.html**

Konten yang harus ada:
- Daftar 3 mata kuliah utama (DSS, Machine Learning, Digital Transformation)
- Untuk setiap mata kuliah:
  - Deskripsi singkat
  - Tools yang digunakan
  - Link ke halaman detail
  - Link ke silabus/materi (jika ada)
- Section "For Students" dengan:
  - Panduan topik skripsi/tesis
  - Template laporan
  - Link ke Wiki & Decision Lab

**teaching/decision-support-systems.html**
**teaching/machine-learning.html**
**teaching/digital-transformation.html**

Untuk setiap halaman detail mata kuliah:
- Deskripsi lengkap mata kuliah
- Tujuan pembelajaran
- Topik yang dibahas
- Tools & teknologi
- Contoh proyek (tanpa data sensitif)
- Link download silabus
- Testimoni mahasiswa (opsional)

### 3. **Halaman Research**

**research/index.html**

Konten:
- Ringkasan area riset
- Highlight 5-10 publikasi terbaru dalam tabel:
  - Tahun
  - Judul Singkat
  - Venue/Jurnal
  - Topik (DSS/MCDM/DT)
  - Link DOI
- Ongoing projects
- Research highlights (kontribusi praktis)
- Link ke Google Scholar, ORCID, ResearchGate

### 4. **Halaman Resources**

**resources/index.html**

Konten:
- 2 kartu utama:
  1. **Wiki** - Catatan terstruktur untuk mahasiswa
  2. **Decision Lab** - Platform pembelajaran MCDM/DSS
- Section "For Practitioners":
  - Template MCDM
  - Rubrik evaluasi
  - Sample datasets
- Coming soon: Online courses/microcredentials

### 5. **Halaman Contact**

**contact.html**

Konten:
- Form sederhana atau instruksi untuk:
  - Thesis supervision
  - Guest lecture invitation
  - Research collaboration
  - Consulting/workshop
- Email & social media links
- Office hours (jika ada)

## Template HTML Standar

Semua halaman baru sebaiknya menggunakan struktur dan style yang sama dengan `about/index.html` untuk konsistensi:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>[Page Title] - Denny Sihombing</title>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <style>
        /* Salin CSS dari about/index.html */
    </style>
</head>
<body>
    <nav>
        <div class="nav-container">
            <a href="/" class="logo">Denny Sihombing</a>
            <ul class="nav-links">
                <li><a href="/">Home</a></li>
                <li><a href="/about/">About</a></li>
                <li><a href="/teaching/">Teaching</a></li>
                <li><a href="/research/">Research</a></li>
                <li><a href="/resources/">Resources</a></li>
                <li><a href="/contact.html">Contact</a></li>
            </ul>
        </div>
    </nav>

    <!-- Main Content Here -->

    <footer>
        <p>&copy; 2024 Denny Sihombing. All rights reserved.</p>
    </footer>
</body>
</html>
```

## CSS Variables (Warna)

Untuk konsistensi branding:

```css
:root {
    --orange: #ff6b35;
    --orange-hover: #e55a2b;
    --orange-light: #fff5f2;
    --dark: #1a202c;
    --gray: #4a5568;
    --light-gray: #f7f8f9;
    --border: #e2e8f0;
}
```

## Checklist Implementasi

- [x] Buat struktur folder `about/`
- [x] Buat halaman `about/index.html`
- [ ] Update `index.html` (navigasi + konten baru)
- [ ] Buat folder & halaman `teaching/`
- [ ] Buat folder & halaman `research/`
- [ ] Buat folder & halaman `resources/`
- [ ] Buat halaman `contact.html`
- [ ] Test semua link navigasi
- [ ] Responsive design check

## Best Practices

1. **Konsistensi Navigasi**: Semua halaman harus punya navigasi yang sama
2. **Breadcrumb**: Tambahkan breadcrumb untuk halaman turunan
3. **CTA yang Jelas**: Setiap halaman punya minimal 1 call-to-action
4. **Mobile-First**: Pastikan responsive di semua perangkat
5. **SEO**: Setiap halaman punya `<title>` dan meta description yang unik
6. **Loading Speed**: Minimalkan ukuran gambar dan CSS

## Contact untuk Kolaborasi

Untuk pertanyaan atau saran pengembangan website:
- GitHub: [@dsihombing](https://github.com/dsihombing)
- Website: [dsihombing.github.io](https://dsihombing.github.io)

---

**Last Updated**: 10 Desember 2024
**Status**: 🚧 Dalam pengembangan
