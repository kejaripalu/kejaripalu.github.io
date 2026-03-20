# Struktur Konten Hugo — Kementerian RI

Salin seluruh folder `content/` ini ke dalam proyek Hugo Anda.

---

## 📁 Struktur Lengkap

```
content/
├── _index.md              ← Homepage
├── profil/
│   └── _index.md          ← Halaman profil kementerian
├── berita/
│   ├── sistem-layanan-terintegrasi.md
│   ├── cpns-formasi-2025.md
│   ├── regulasi-tata-kelola-data.md
│   ├── beasiswa-unggulan-2025.md
│   └── mou-asean-2025.md
├── layanan/
│   └── _index.md          ← Halaman layanan publik
└── kontak/
    └── _index.md          ← Halaman kontak
```

---

## ✏️ Cara Menambah Berita Baru

Buat file baru di `content/berita/`:

```bash
hugo new berita/nama-berita-anda.md
```

Atau buat manual dengan format berikut:

```markdown
---
title: "Judul Berita Anda"
date: 2025-03-20
kategori: "Pengumuman"
tags: ["tag1", "tag2"]
summary: "Ringkasan singkat yang muncul di daftar berita."
---

Isi konten berita dalam format Markdown di sini...
```

### Pilihan `kategori`:
- `Pengumuman`
- `Kebijakan`
- `Program`
- `Regulasi`
- `Kegiatan`
- `Kemitraan`

---

## 📝 Tips Penulisan Konten

- Gunakan heading `##` untuk sub-judul
- Gunakan tabel Markdown untuk data terstruktur
- Gunakan `> teks` untuk kutipan penting
- Gunakan `**teks**` untuk penekanan
- Gunakan `- item` atau `1. item` untuk daftar

---

## 🔗 URL yang Dihasilkan

| File | URL |
|------|-----|
| `content/_index.md` | `/` |
| `content/berita/cpns-2025.md` | `/berita/cpns-2025/` |
| `content/profil/_index.md` | `/profil/` |
| `content/layanan/_index.md` | `/layanan/` |
| `content/kontak/_index.md` | `/kontak/` |
