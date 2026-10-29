# MEMORY — Memori Proyek Raker IKU IKT 2026

Dokumen ini adalah memori bersama untuk semua agen. Perbarui saat ada fakta baru, keputusan, atau pertanyaan yang terbuka. Tandai setiap entri dengan tanggal (format YYYY-MM-DD, zona waktu Asia/Bangkok).

Status verifikasi: ✅ terverifikasi dari sumber langsung · ⚠️ dari instruksi/ingatan, perlu verifikasi · ❓ belum diketahui.

## 1. Identitas proyek
- Repositori: `sistekinuwg/raker-iku-ikt-2026` (branch kerja `arena/23f03359-raker-iku-ikt-2026`). ✅
- Isi repositori saat ini: hanya `README.md` (judul "Raker IKU IKT 2026"). ✅
- Lokasi pengguna: Malang, Jawa Timur, Indonesia. ✅
- Konteks institusi: nama file di Google Drive menyebut **UWG Malang** (mis. "Konsep_Rapat_Pimpinan_IKU_UWG_Malang", "LKPT UWG 2026", "LED UWG 2026"). Nama lengkap institusi belum dikonfirmasi. ⚠️
- Tahun fokus: 2026 (dokumen Master IKU/IKT periode 2026–2030). ✅

## 2. Sumber data yang diketahui (Google Drive)
Folder utama Drive: `1SekApOWOspiql5oM6d8H7KmNf75ZJowT` — **belum diunduh ke repo**. Akses langsung dari sandbox ke drive.google.com diblokir; isi diketahui lewat connector Google Drive. ✅

Subfolder dan berkas yang teridentifikasi:
- **Bahan Raker IKU** (`1qnlIHfhyNJvk0BxJI4KpX8COpmuf4ois`)
  - Master IKU_IKT Lengkap UWG 2026–2030 (Fix-update 271026), versi induk dan versi prodi (xlsx).
  - "0 IKU PT 2026 Permen2026 - Original ada rumus IKU.xlsx" (xlsx, ±347 KB).
  - Konsep Rapat Pimpinan IKU UWG Malang (docx).
  - Notulensi Koordinasi Tim Perumus Raker 19-10-2026 (docx).
  - Pembagian Tugas (docx).
  - LKPT UWG 2026 Submit Final (pdf).
  - LED UWG 2026 Submit Final (pdf).
  - Lamp. 3c PerBAN-PT 35/2025 IAPT 4.1 (pdf).
  - Salinan KM 500/M/2024 Standar Minimum Kinerja Dosen (pdf).
- **BAHAN SPMI 2020** (`1cB9Fq4goS1rNvzYAQksDAxRewJFMx-le`): Standar SPMI-Rev, Manual SPMI-Rev, Formulir SPMI, Kebijakan SPMI-Rev (pdf).
- **BAHAN RENSTRA** (`1Mr5zI0j-YBe9kS9PfgYJSMGcrkLQwsBV`): subfolder "RENSTRA UNIVERSITAS" dan "RENSTRA FAKULTAS". Isi belum ditelusuri. ❓

## 3. Regulasi acuan
- **BAN-PT IAPT 4.1**, Peraturan BAN-PT No. 35 Tahun 2025, untuk institusi (CRAM). ⚠️ Rujukan ke dokumen resmi harus diverifikasi (lihat lampiran 3c di Drive).
- **LAM INFOKOM 2.1**, untuk prodi rumpun Informatika/Komputer (9 kriteria). ⚠️ Versi dan matriks penilaian harus diverifikasi ke dokumen resmi LAM INFOKOM.
- **SPMI** internal UWG (dokumen 2020, direvisi). ✅ keberadaan dokumen; ❓ status revisi terkini.
- **KM 500/M/2024**: Standar Minimum Kinerja Dosen. ✅ keberadaan dokumen.

## 4. Keputusan
- 2026-10-29: Struktur memori agen dibuat (`AGENTS.md`, `CLAUDE.md`, `agent/`). Diminta pengguna agar dapat dipakai lintas-agen.
- 2026-10-29: Unduhan Drive via gdown gagal (jaringan sandbox). Opsi: pengguna menjalankan gdown lokal, atau unduh lewat connector ke folder terpisah yang di-ignore Git. Keputusan akhir belum diambil. ❓

## 5. Pertanyaan terbuka
- ❓ Nama lengkap institusi dan nama prodi yang diakreditasi (apakah satu atau beberapa prodi rumpun INFOKOM).
- ❓ Jenjang dan status akreditasi saat ini (institusi dan prodi), serta tanggal kedaluwarsa.
- ❓ Apakah bahan Drive boleh dimasukkan ke repositori, atau cukup disimpan di luar Git.
- ❓ Tahap kerja saat ini: penyusunan LED, reviu, atau persiapan AL.
- ❓ Data kinerja IKU/IKT tahun berjalan: sumber dan periodenya.

## 6. Log Keputusan
| Tanggal | Keputusan / Perubahan | Oleh |
|---|---|---|
| 2026-10-29 | Membuat AGENTS.md, CLAUDE.md, folder agent/ (SOUL, PERSONA, MEMORY, agents/, manifest.json) | Agen Arena |
