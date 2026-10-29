# AGENTS.md — Raker IKU IKT 2026

Berkas ini adalah titik masuk utama untuk agen AI apa pun (Codex, Claude Code, Cursor, Gemini CLI, Arena Agent, dll.) yang bekerja di repositori ini.

## 1. Konteks proyek
- Repositori: `sistekinuwg/raker-iku-ikt-2026`
- Tujuan: mendukung **Rapat Kerja (Raker) IKU dan IKT tahun 2026** serta penyusunan dokumen akreditasi institusi dan program studi.
- Bahasa kerja: **Bahasa Indonesia formal** (istilah teknis boleh Inggris bila lazim di dokumen akreditasi).

## 2. Urutan membaca wajib sebelum bekerja
1. `agent/SOUL.md` — nilai dan prinsip dasar agen.
2. `agent/PERSONA.md` — peran, gaya bahasa, dan format jawaban.
3. `agent/MEMORY.md` — fakta proyek, keputusan, dan hal yang masih terbuka.
4. `agent/agents/` — definisi agen spesialis; pilih yang sesuai tugas.
5. `agent/manifest.json` — daftar machine-readable untuk orkestrasi.

## 3. Aturan kerja lintas-agen
- **Jangan mengarang data.** Angka IKU/IKT, skor, dan regulasi hanya boleh berasal dari file sumber atau dari pengguna. Jika tidak ada, tandai sebagai `[PERLU DATA]`.
- **Rujukan regulasi wajib**: sebutkan dasar (BAN-PT IAPT 4.1 / Perban 35/2025 untuk institusi; LAM INFOKOM 2.1 untuk prodi) pada setiap rekomendasi akreditasi.
- **Format jawaban akreditasi**: *Analisis Ketercapaian/Standar → Identifikasi Celah (Gap) → Rekomendasi Narasi/Data.*
- **Reviu draf LED**: beri skor rubrik 1–4 per poin, lalu sertakan *revised draft* yang bersifat evaluatif.
- **Dokumen sumber tidak diubah tanpa izin.** Jika membuat versi revisi, simpan sebagai berkas baru dan sebutkan perubahannya.
- **Git**: kerjakan hanya pada branch `arena/23f03359-raker-iku-ikt-2026`. Jangan membuat atau push ke branch lain. Jangan menghapus `.git`.
- **Kredensial**: jangan pernah menulis token, kata sandi, atau kredensial ke dalam berkas repo.
- **Data pribadi**: data dosen/mahasiswa (NIDN, NIM, gaji, dsb.) tidak boleh di-commit tanpa instruksi eksplisit; anonimkan bila dipakai sebagai contoh.

## 4. Pemetaan tugas → agen
| Tugas | Agen |
|---|---|
| Reviu/penyusunan LED institusi, LKPT, CRAM | `agent/agents/iapt-institusi.md` |
| Reviu/penyusunan LED prodi, LKPS, 9 kriteria | `agent/agents/lam-infokom-prodi.md` |
| Penyelarasan SPMI dengan fakta prodi | `agent/agents/spmi-alignment.md` |
| Analisis dan validasi data IKU/IKT (xlsx) | `agent/agents/iku-ikt-data.md` |
| Persiapan Asesmen Lapangan (AL) | `agent/agents/asesmen-lapangan.md` |

## 5. Perintah umum
- Tidak ada build/test formal saat ini. Verifikasi cukup dengan membaca ulang berkas dan memeriksa konsistensi angka.
- Setelah mengubah berkas di `agent/`, perbarui `agent/MEMORY.md` bagian *Log Keputusan* bila ada keputusan baru.
