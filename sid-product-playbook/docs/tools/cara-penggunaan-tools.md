# ClickUp, Notion & Cowork — Panduan Penggunaan

tags: [tools, clickup, notion, cowork, workflow]

---

## Overview: Tool untuk Apa?

| Tool | Fungsi utama | Jangan dipakai untuk |
|---|---|---|
| **ClickUp** | Task management, PRD, sprint tracking | Dokumentasi panjang, notes meeting |
| **Notion** | Meeting notes (MOM), database referensi | Task tracking harian |
| **Cowork (Claude)** | Drafting dokumen, riset, wiki management | Sumber kebenaran data bisnis |
| **Figma** | Design, prototype, UI review | Task tracking atau dokumentasi |

---

## ClickUp

### Struktur Workspace SID

```
Workspace: SID
└── Space: Tribe 3 (T3)
    ├── Folder: [Domain/Area]
    │   ├── List: Sprint N
    │   └── List: Backlog
    └── Docs: PRD repository
```

### Cara Membuat Task yang Baik

Task yang baik di ClickUp memiliki:

1. **Judul yang jelas** — "Buat fitur X" bukan "Fitur X"
2. **Deskripsi** — Konteks singkat, link PRD kalau ada
3. **Assignee** — Satu orang PIC, bukan multiple tanpa kejelasan
4. **Due date** — Tanggal konkret, bukan "ASAP"
5. **Status yang akurat** — Update status sesuai progress aktual

!!! warning "Anti-pattern"
    Task dengan status "In Progress" selama 2 minggu tanpa update adalah tanda bahwa ada blocker yang belum dieskalasikan. PM harus proaktif menanyakan.

### Status Task di SID

| Status | Artinya |
|---|---|
| `Open` | Belum dimulai, sudah diprioritaskan |
| `In Progress` | Sedang dikerjakan |
| `In Review` | Menunggu review/approval |
| `Done` | Selesai dan terverifikasi |
| `Blocked` | Ada blocker — wajib ada comment penjelasan |

### PRD di ClickUp

PRD disimpan di **ClickUp Docs** (bukan di task deskripsi). Setiap PRD memiliki struktur:

- Overview & Change Log
- Background (Problem Statement + Proposed Solution)
- OKR
- Target Audience
- Scope & Phase
- User Story & UAC
- Risk Management
- Dependencies

---

## Notion

Notion dipakai **khusus untuk Meeting Notes (MOM)** sejak April 2026.

### Cara Membuat MOM Baru

1. Buka database **Meeting Notes** di Notion
2. Klik **New** → pilih template MOM
3. Isi field: Meeting name, Date, Category, Attendees
4. Tambahkan Summary (1-2 kalimat) di field Summary
5. Tulis konten lengkap di body page

### Kategori Meeting

- `Planning` — Sprint planning, roadmap review
- `Standup` — Daily / weekly standup
- `Presentation` — Demo, showcase ke stakeholder
- `Retro` — Sprint retrospective
- `Customer call` — Interview pengguna, discovery call

!!! tip "Tips"
    Isi field **Summary** dengan 1-2 kalimat yang menangkap inti rapat. Ini yang akan muncul di list view dan sangat berguna saat kamu perlu trace keputusan lama.

---

## Cowork (Claude)

Cowork adalah interface Claude yang terhubung ke wiki dan tools tim. Ini berbeda dari claude.ai biasa karena punya akses ke:

- Wiki lokal (Google Drive → Product Wiki)
- ClickUp (baca dan tulis task)
- Notion (buat dan update MOM)
- Figma (baca design context)

### Use Case Utama di Cowork

=== "Draft Dokumen"
    Minta Claude draft PRD, Request Doc, atau One Pager berdasarkan konteks yang kamu berikan. Gunakan skill `/prd-generator`.

=== "Update Wiki"
    Paste notes atau dokumen apapun dan minta: "Simpan ini ke wiki." Claude akan routing ke lokasi yang tepat.

=== "Review PRD"
    Share link ClickUp atau paste PRD, lalu gunakan skill `/prd-reviewer` untuk mendapat feedback terstruktur.

=== "Riset Cepat"
    Tanya apapun tentang kompetitor, best practice, atau framework — Claude akan search dan synthesize hasilnya.

### Tips Penggunaan Cowork yang Efektif

1. **Berikan konteks dulu** — Sebutkan kamu PM Tribe berapa, featurenya apa, dan audiensnya siapa
2. **Minta format spesifik** — "Format sebagai tabel", "Tulis dalam Bahasa Indonesia", "Maksimal 300 kata"
3. **Iterasi** — Draft pertama belum sempurna; minta revisi spesifik, bukan "perbaiki secara umum"
4. **Verifikasi output** — Terutama untuk data, angka, dan klaim faktual

---

## Panduan Quick Decision: Tool Mana yang Dipakai?

```
Punya task baru?
→ ClickUp

Selesai meeting?
→ Notion (MOM)

Perlu draft dokumen?
→ Cowork (Claude)

Ada keputusan produk penting?
→ Wiki (Decisions/) via Cowork

Perlu update design?
→ Figma
```

---

*Terakhir diupdate: Juni 2026*
