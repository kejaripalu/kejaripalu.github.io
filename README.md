# Template Website Kementerian — Hugo + Tailwind CSS

Template website pemerintah yang elegan dan modern menggunakan Hugo SSG dengan Tailwind CSS via CDN.

---

## 📁 Struktur File

```
kementerian-template/
├── hugo.toml                          # Konfigurasi utama Hugo
└── layouts/
    ├── _default/
    │   └── baseof.html                # Base layout (HTML, Tailwind config, font)
    ├── index.html                     # Halaman Beranda
    ├── partials/
    │   ├── header.html                # Navigasi + top bar
    │   └── footer.html                # Footer lengkap
    ├── berita/
    │   └── list.html                  # Daftar berita + sidebar
    └── profil/
        └── single.html                # Halaman profil, visi & misi
```

---

## 🚀 Cara Instalasi

### 1. Salin ke direktori Hugo Anda
```bash
cp -r kementerian-template/* /path/to/hugo-project/
```

### 2. Buat konten berita
```bash
hugo new berita/nama-berita.md
```
Isi front matter minimal:
```yaml
---
title: "Judul Berita"
date: 2025-03-15
kategori: "Pengumuman"
summary: "Ringkasan singkat berita ini."
---
```

### 3. Jalankan server Hugo
```bash
hugo server -D
```

---

## 🎨 Desain

| Elemen | Detail |
|--------|--------|
| **Warna Utama** | Navy `#1a2540` — Emas `#d4a917` |
| **Font Heading** | Playfair Display (serif, elegan) |
| **Font Body** | Plus Jakarta Sans (bersih, modern) |
| **CSS Framework** | Tailwind CSS via CDN |
| **Tema** | Putih elegan, formal, profesional |

---

## 📄 Halaman yang Tersedia

- **Beranda** (`/`) — Hero, Layanan Unggulan, Berita, Pimpinan, CTA
- **Berita** (`/berita`) — Grid + sidebar filter + pagination
- **Profil** (`/profil`) — Tentang, Visi Misi, Statistik
- **Header** — Top bar ticker, navigasi dropdown, mobile menu
- **Footer** — Kolom info, sosial media, link cepat

---

## ✏️ Kustomisasi

Ganti info instansi di `hugo.toml`:
```toml
[params]
  description = "..."
  address = "..."
  phone = "..."
  email = "..."
```

Ubah warna di `baseof.html` bagian `tailwind.config`:
```js
colors: {
  gold: { 500: '#d4a917' },   // Ganti warna aksen
  navy: { 900: '#1a2540' },   // Ganti warna utama
}
```
