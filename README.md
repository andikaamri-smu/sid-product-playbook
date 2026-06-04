# SID Product Playbook

Panduan internal tim produk PT Semesta Integrasi Digital, dibangun dengan [MkDocs](https://www.mkdocs.org/) + [Material theme](https://squidfunk.github.io/mkdocs-material/).

---

## Setup: Dari Nol ke Live di GitHub Pages

### Langkah 1 — Buat GitHub repo baru

1. Buka https://github.com/new
2. Nama repo: `sid-product-playbook`
3. Visibility: **Private** (rekomendasi untuk konten internal)
4. Jangan centang "Add README" — kita sudah punya
5. Klik **Create repository**

### Langkah 2 — Update config

Buka `mkdocs.yml` dan ganti dua baris ini:

```yaml
site_url: https://YOUR_GITHUB_USERNAME.github.io/sid-product-playbook
repo_url: https://github.com/YOUR_GITHUB_USERNAME/sid-product-playbook
```

Ganti `YOUR_GITHUB_USERNAME` dengan username GitHub kamu.

### Langkah 3 — Push ke GitHub

```bash
cd sid-product-playbook
git init
git add .
git commit -m "Initial commit: SID Product Playbook"
git branch -M main
git remote add origin https://github.com/YOUR_GITHUB_USERNAME/sid-product-playbook.git
git push -u origin main
```

### Langkah 4 — Aktifkan GitHub Pages

1. Buka repo di GitHub → **Settings** → **Pages**
2. Source: pilih **"GitHub Actions"**
3. Simpan

### Langkah 5 — Tunggu deploy

GitHub Actions akan otomatis build dan deploy. Cek progress di tab **Actions** di repo kamu. Biasanya selesai dalam 1-2 menit.

Setelah selesai, blog kamu live di:
`https://YOUR_GITHUB_USERNAME.github.io/sid-product-playbook`

---

## Cara Menambah Artikel Baru

1. Buat file `.md` baru di folder yang relevan:
   - `docs/kolaborasi/` — untuk artikel kolaborasi tim
   - `docs/ai-tips/` — untuk tips AI
   - `docs/tools/` — untuk panduan tools
2. Tambahkan entry baru ke bagian `nav:` di `mkdocs.yml`
3. Commit dan push ke `main` — halaman otomatis terupdate

---

## Preview Lokal (opsional)

Kalau ingin preview sebelum push:

```bash
pip install mkdocs-material
mkdocs serve
```

Buka http://localhost:8000 di browser.

---

## Struktur Folder

```
sid-product-playbook/
├── docs/
│   ├── index.md                        # Homepage
│   ├── kolaborasi/
│   │   └── cara-kolaborasi.md
│   ├── ai-tips/
│   │   └── ai-untuk-pm.md
│   └── tools/
│       └── cara-penggunaan-tools.md
├── .github/
│   └── workflows/
│       └── deploy.yml                  # Auto-deploy ke GitHub Pages
├── mkdocs.yml                          # Konfigurasi utama
└── README.md                           # File ini
```
