# DESIGN — Portfolio Lamaran IT Support (Rizky)

Tanggal: 2026-09-22
Status: draf untuk review (belum implementasi)

## Register desain

### Arah estetika: "Teknikal Dossier"

Diri sebagai dokumen kerja teknis: cetakan biru/rekayasa. Kesan: rapi, presisi,
dapat diperiksa — sesuai peran yang dilamar (IT support = orang yang menegakkan
dokumentasi dan prosedur).

Ciri wajib:
- Grid asimetris dua kolom (bukan satu kolom center).
- Huruf besar pada judul; label meta/data memakai mono (rasa anotasi gambar kerja).
- Garis aturan/ruled lines sebagai pemisah; anotasi kecil bergaya teknik.
- Banyak ruang kosong; gelap-diatas-terang (dark text, light background).
- Satu warna aksen untuk highlight penting.

Dilarang (anti-slop):
- Gradien, glassmorphism, emoji-icon, dark-terminal gimmick, hero center dengan
  paragraf raksasa, stock-photo placeholder, template "wow".
- Semua keputusan tampilan harus bisa dijawab "kenapa" — bukan "biar keren".

### Kata-kata merek (untuk pilihan font & nada copy)
presisi · jelas · tepercaya

## Tipografi

- Load via Google Fonts link, maksimal 2 keluarga web font.
- Headings: **Space Grotesk** (geometris, teknis, modern).
- Labels/meta/data (kicker "DATA 01 — ", nomor, angka): **IBM Plex Mono**.
- Body: system-ui stack (tanpa font web → hemat performa).
- `lang="id"` pada `<html>`.

Skala:
- Fluid `clamp()` untuk judul; body 16–18px; rasio skala ≥ 1.25–1.333.
- Kicker label mono di atas judul tiap seksi.

## Layout

- Dua kolom asimetris (konten utama + kolom samping strimin).
- Irama: grup rapat antar-item, pemisahan luas antar-seksi ("jelas").
- Informasi kunci tampil di layar pertama (fold atas) — HRD menilai < 60 detik.
- Header: nama besar, label "IT Support", tagline, skill inti, dan pernyataan
  cita-cita wajib: memasuki bagian IT adalah cita-cita (diterjemahkan halus dari
  PRODUCT.md).

## Peta seksi (5, mengikuti PRODUCT.md)

1. **Data 01 — Header & Ringkasan**: nama, peran, tagline, skill inti,
   pernyataan cita-cita.
2. **Data 02 — Keahlian**: dikelompokkan (OS, Jaringan, Layanan Helpdesk/
   Ticketing, Keamanan, Cloud & Tools).
3. **Data 03 — Pengalaman & Proyek**: judul → dikerjakan → hasil/impact.
4. **Data 04 — Sertifikat & Kursus**.
5. **Data 05 — Kontak & Link**: email, nomor, GitHub/LinkedIn (placeholder
   `TODO` hingga disuplai user).

## Konten

- Konten sumber profil dari GitHub/LinkedIn user; data yang tipis diberi
  placeholder `TODO`, tidak dikarang.
- Salinan asli dalam bahasa Indonesia; nada profesional, minim adjektiva hampa.

## Kendala teknis

- Statis: satu `index.html` + CSS; JS minimal atau nol.
- Tinggal di `/home/rizky`.
- Implementasi dimulai hanya setelah spec ini direview/disetujui.

## Keputusan yang belum selesai
- URL GitHub/LinkedIn resmi (placeholder `TODO`).
- Data detail pengalaman/proyek/sertifikat bila profil sumber tipis.