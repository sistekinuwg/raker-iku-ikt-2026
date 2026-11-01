# Catatan Kegiatan Belum Tercatat

Dibuat: 01-11-2026 19:08 (Asia/Bangkok)
Branch: `arena/0e59477f-raker-iku-ikt-2026`
Sumber: riwayat kerja sesi ini. Belum tercatat di `agent/MEMORY.md` atau `analisis/001_*`.

## 1. Sumber Google Drive yang belum ada di MEMORY.md
MEMORY.md baru mencatat folder UWG. Dua folder lain belum tercatat.

| Set | ID folder | Isi | Status |
|---|---|---|---|
| KPT 3 prodi | `195jXbBCZp0qgxqkBB_tqf6Ro2mWhOxrb` | 3 DOCX: Buku KPT Teknik Informatika, Buku KPT STI Final, KPT OBE Bisdig | Terindeks (001) |
| FSTI | `1-ySBlqQgF3yH-SPfg1xh0sPafT-gfFsw` | 17 berkas: 4 xlsx + 13 PDF instrumen APS Diploma I–III dan Sarjana/Sarjana Terapan | Terindeks (001) |

Struktur FSTI: subfolder "INSTRUMEN UNGGUL LAM-INFOKOM" → "1. Program Diploma" (Diploma I, II, III) dan "2. Program Sarjana" (Sarjana, Sarjana Terapan).

Tiga matriks "Diploma - Matriks Penilaian.pdf" memiliki nama dan ukuran sama, serta md5 identik (`b0c5e44c…`).

## 2. Status salinan lokal (`google_drive/`)
- Salinan lokal 47 berkas (UWG 27, KPT 3, FSTI 17) pernah berhasil diunduh.
- Folder `google_drive/` tidak ada pada 01-11-2026. Workspace sudah di-reset beberapa kali sebelumnya, dan folder ini hilang setiap kali.
- Hanya indeks (`001_indeks_referensi_30102026_0925.md`) yang tersimpan di Git.
- Folder `google_drive/` di-ignore oleh `.gitignore` (PR #2).

## 3. Perbedaan ukuran xlsx antar-unduhan
Tiga xlsx UWG dan dua xlsx FSTI menunjukkan ukuran berbeda di setiap unduhan. Contoh: Permen2026 347.334 → 372.417 byte. Versi aktual di Drive belum diverifikasi. Ini sudah dicatat di indeks 001 (bagian 5 dan 7).

## 4. Izin berbagi Google Drive (diperiksa 01-11-2026)
| Folder | Link siapa pun | Role | Catatan |
|---|---|---|---|
| UWG | aktif | writer | owner istiadi@widyagama.ac.id; 8 izin, termasuk 2 akun Gmail pribadi |
| KPT | aktif | writer | owner fsti@widyagama.ac.id; 2 izin |
| FSTI | aktif | writer | owner fsti@widyagama.ac.id; 2 izin |

- Siapa pun dengan link bisa mengedit ketiga folder. Ini belum diubah.
- Verifikasi akses dari browser belum dilakukan. Sandbox tidak bisa menjangkau drive.google.com.
- Keputusan belum diambil: mengubah ke reader (`make_public` role reader), dan apakah izin editor per email dipertahankan.

## 5. Riwayat PR dan branch
| PR | Branch | Isi | Status |
|---|---|---|---|
| #1 | `arena/23f03359-raker-iku-ikt-2026` | AGENTS.md, CLAUDE.md, folder agent/ | Merged |
| #2 | `arena/6d2a021e-raker-iku-ikt-2026` | `.gitignore` untuk `google_drive/` | Merged |
| #3 | `arena/384ca5a0-raker-iku-ikt-2026` | Aturan penamaan analisis, indeks 001 | Merged (`ca94814`) |

Pada beberapa momen, workspace kembali ke kondisi lama dan perubahan yang sudah di-push tampak sebagai perubahan lokal yang belum ter-commit. Setiap kali, branch lokal disinkronkan dengan `git merge --ff-only` ke remote.

## 6. Temuan audit yang belum diperbaiki
Audit atas file agen (`AGENTS.md`, `agent/PERSONA.md`, `agent/manifest.json`, `agent/agents/*`) menemukan:
- Klaim regulasi yang disajikan sebagai fakta tanpa penanda verifikasi, misalnya "masa berlaku akreditasi 8 tahun" di PERSONA.md.
- `manifest.json` mencantumkan "Permen 2026 (rumus IKU)" sebagai dasar regulasi. Itu hanya nama file, bukan isi peraturan.
- Rujukan ke lampiran dan dokumen resmi yang belum dibaca.
- Beberapa file terlalu panjang untuk aturan "no verbose".

Perbaikan belum dikerjakan.

## 7. Keputusan yang masih terbuka
1. Ubah izin ketiga folder dari writer ke reader?
2. Unduh ulang 47 berkas dan tambahkan checksum SHA-256 ke indeks?
3. Terapkan perbaikan audit pada file agen?
4. Perbarui `agent/MEMORY.md` dengan sumber KPT, FSTI, dan status salinan lokal?
