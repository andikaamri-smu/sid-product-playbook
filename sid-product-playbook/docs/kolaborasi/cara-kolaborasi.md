# Cara Kolaborasi Antar Tim Produk

tags: [kolaborasi, workflow, handoff]

---

## Prinsip Dasar

Kolaborasi yang baik dimulai dari **kejelasan ekspektasi**, bukan dari banyaknya rapat. Sebelum meminta waktu orang lain, pastikan konteksnya sudah siap.

!!! tip "Aturan Praktis"
    Kalau kamu bisa menyampaikannya secara async (tulisan, dokumen, loom), lakukan itu dulu. Sinkronisasi (rapat) hanya untuk hal yang membutuhkan diskusi dua arah secara real-time.

---

## Alur Kerja Standar

### 1. PM → Engineering (Handoff)

Sebelum fitur masuk sprint, pastikan PRD sudah memuat:

- **Background & Problem Statement** — Engineer harus paham *mengapa* fitur ini dibuat, bukan hanya *apa* yang harus dibangun
- **UAC (User Acceptance Criteria)** — Kriteria yang jelas dan terukur, bukan ambigu
- **Edge cases** — Skenario di luar happy path sudah dipikirkan PM, bukan ditemukan saat dev
- **Dependencies** — Fitur mana yang harus selesai dulu, atau tim mana yang perlu dilibatkan

!!! warning "Anti-pattern yang harus dihindari"
    Jangan handoff PRD yang belum final dengan kata "nanti kita discuss lagi." Ini membuang waktu Engineer untuk membaca sesuatu yang akan berubah.

---

### 2. PM → Design

- Briefing desain menggunakan **One Pager atau PRD draft** — bukan lisan saja
- Sertakan referensi visual kalau ada (kompetitor, contoh flow yang bagus)
- Tentukan deadline review di awal, bukan mendekati sprint start

---

### 3. Lintas Tribe (Cross-tribe)

Ketika sebuah fitur membutuhkan kontribusi dari tribe lain, gunakan **Request Doc** (bukan langsung Slack). Request Doc berisi:

| Field | Isi |
|---|---|
| Requestor | Nama PM + Tribe |
| Deadline dibutuhkan | Tanggal konkret |
| Output yang diminta | Apa yang dibutuhkan dari tribe lain |
| Context | Kenapa ini penting, dampak kalau tidak selesai |
| ClickUp link | Link ke PRD atau task terkait |

> Request Doc memastikan tribe lain bisa mengalokasikan kapasitas dengan tepat, bukan terkejut di menit terakhir.

---

## Channels Komunikasi

| Konteks | Channel |
|---|---|
| Update status cepat, pertanyaan singkat | Slack DM / channel tim |
| Diskusi yang butuh keputusan | Rapat sync + MOM di Notion |
| Permintaan ke tribe lain | Request Doc di ClickUp |
| Feedback desain | Komentar langsung di Figma |
| Eskalasi ke stakeholder | Dokumen tertulis (One Pager / deck) |

---

## Tips Agar Rapat Efektif

1. **Kirim agenda sebelum rapat** — minimal 1 jam sebelumnya
2. **Tentukan decision maker** di awal — siapa yang punya suara final?
3. **Catat keputusan, bukan hanya diskusi** — MOM harus berisi action items dengan PIC dan deadline
4. **Standing meeting maksimal 30 menit** — kalau perlu lebih, ada yang salah dengan agenda-nya

---

## Template MOM (Minutes of Meeting)

```
## [Nama Rapat] — [Tanggal]

**Attendees:** [Nama-nama]
**Facilitator:** [Nama PM]

### Agenda
1. ...
2. ...

### Keputusan
- [Keputusan 1]
- [Keputusan 2]

### Action Items
| Action | PIC | Deadline |
|---|---|---|
| ... | ... | ... |

### Hal yang di-defer / belum diputuskan
- ...
```

---

*Terakhir diupdate: Juni 2026*
