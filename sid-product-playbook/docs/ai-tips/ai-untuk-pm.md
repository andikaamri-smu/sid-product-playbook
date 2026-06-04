# Menggunakan AI dalam Pekerjaan Sehari-hari PM

tags: [ai, produktivitas, claude, cowork]

---

## Mengapa AI Penting untuk PM?

PM menghabiskan banyak waktu untuk hal-hal yang sebenarnya bisa didelegasikan: menulis draft dokumen, merangkum meeting, mencari referensi, atau memformat data. AI bisa menangani ini semua — sehingga kamu bisa fokus pada hal yang benar-benar butuh judgment manusia: keputusan strategis, empati ke pengguna, dan alignment stakeholder.

!!! info "Tools AI yang dipakai tim SID Product"
    - **Claude via Cowork** — untuk semua pekerjaan dokumen, wiki, dan riset
    - **Claude via web** — untuk brainstorm cepat
    - **NotebookLM** — untuk meringkas dokumen panjang atau riset

---

## 5 Use Case Terbaik AI untuk PM

### 1. Draft PRD lebih cepat

Daripada mulai dari halaman kosong, gunakan AI untuk menghasilkan draft awal berdasarkan konteks yang kamu berikan. Prompt yang efektif:

```
Buatkan draft PRD untuk fitur [nama fitur].
Konteks: [jelaskan masalah yang mau diselesaikan, siapa penggunanya, batasan teknis kalau ada].
Format: gunakan struktur Background → Problem Statement → Proposed Solution → UAC.
```

Hasilnya belum sempurna, tapi 70% lebih baik dari halaman kosong.

---

### 2. Rangkum meeting notes

Paste transcript atau catatan kasar ke Claude, lalu minta:

```
Ini adalah catatan rapat [nama rapat].
Tolong rangkum menjadi:
1. Keputusan yang diambil
2. Action items (dengan PIC kalau disebut)
3. Pertanyaan yang belum terjawab
```

---

### 3. Review dan challenge dokumen

Setelah menulis PRD atau proposal, minta AI untuk menjadi "devil's advocate":

```
Ini PRD saya untuk [fitur X].
Berperan sebagai Engineering Lead yang skeptis — apa saja yang lemah, ambigu, atau hilang dari dokumen ini?
```

Ini sangat membantu menemukan blind spot sebelum dokumen dibagikan ke tim.

---

### 4. Riset cepat

Kalau butuh benchmark atau referensi kompetitor:

```
Bagaimana [kompetitor A, B, C] menangani [masalah X]?
Fokus pada: UX flow, model bisnis, dan hal yang bisa kami pelajari.
```

Selalu verifikasi fakta penting dari hasil AI dengan sumber primer.

---

### 5. Drafting komunikasi sulit

Feedback ke stakeholder, eskalasi masalah, atau menolak request — AI bisa bantu menyusun kata-kata yang tepat:

```
Saya perlu menolak request dari [stakeholder] untuk [fitur X] karena [alasan].
Bantu saya menulis pesan yang jelas, tidak defensif, dan tetap menjaga hubungan baik.
```

---

## Cara Menulis Prompt yang Efektif

| Elemen | Contoh buruk | Contoh baik |
|---|---|---|
| **Konteks** | "Buatkan PRD" | "Buatkan PRD untuk fitur notifikasi pengingat ujian untuk siswa SMP" |
| **Format output** | (tidak disebutkan) | "Format sebagai: Background → Problem → Solution → UAC" |
| **Persona** | (tidak disebutkan) | "Berperan sebagai Senior PM yang berpengalaman di EdTech" |
| **Batasan** | (tidak disebutkan) | "Maksimal 500 kata, gunakan bahasa Indonesia yang formal tapi tidak kaku" |

---

## Yang TIDAK boleh didelegasikan ke AI

- **Keputusan akhir produk** — AI bisa bantu analisis, tapi keputusan tetap di PM
- **Penilaian empati pengguna** — AI tidak pernah berbicara langsung dengan pengguna kamu
- **Validasi data bisnis** — selalu cek angka dari sumber primer (BI, Finance)
- **Komunikasi sensitif** — draft boleh pakai AI, tapi tone dan nuansa harus kamu edit sendiri

---

## Tips Harian

!!! tip "Mulai hari dengan AI brief"
    Setiap pagi, paste to-do list dan agenda rapat ke Claude, lalu tanya: "Apa yang paling penting untuk diselesaikan hari ini, dan ada risiko apa yang harus saya antisipasi?" Ini membantu prioritisasi lebih sadar.

!!! tip "AI sebagai pair writer"
    Jangan tunggu dokumen 100% siap sebelum minta feedback AI. Paste draft kasar dan minta: "Apa yang paling perlu diperbaiki dari draft ini?"

---

*Terakhir diupdate: Juni 2026*
