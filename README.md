# SlideAkmalV1 — Slaid Interaktif Cipta Sistem Percuma

![Version](https://img.shields.io/badge/version-v1.0.0-blue)
![Status](https://img.shields.io/badge/status-production-green)
![Stack](https://img.shields.io/badge/stack-HTML%20%2B%20CSS%20%2B%20Vanilla%20JS-blue)
![Hosting](https://img.shields.io/badge/hosting-GitHub%20Pages-222222)
![License](https://img.shields.io/badge/license-MIT-yellow)

Laman slaid interaktif **Slide Akmal V1** bertajuk **Cipta Sistem Percuma**. Set slaid ini mengikut gaya Custom Gemini AUD: latar putih-biru yang bersih, aksen emas, penanda kemajuan, kawalan papan kekunci, mod skrin penuh, dan susun atur slaid yang stabil pada paparan pembentangan.

Kandungan ditulis dalam Bahasa Melayu Malaysia dengan ayat diplomatik, sesuai untuk kegunaan taklimat atau pembentangan rasmi di Kuala Lumpur, Malaysia.

**Domain production:** https://slideakmalv1.akmalmarvis.com

- Laman langsung (GitHub Pages): https://akmal4244.github.io/SlideAkmalV1/

## Kandungan

- [Ciri-Ciri Utama](#ciri-ciri-utama)
- [Kandungan Slaid](#kandungan-slaid)
- [Teknologi](#teknologi)
- [Struktur Direktori](#struktur-direktori)
- [Pemasangan](#pemasangan)
- [Konfigurasi](#konfigurasi)
- [Deployment](#deployment)
- [Status Projek](#status-projek)
- [Kredit](#kredit)

## Ciri-Ciri Utama

- **22 slaid interaktif** dalam satu fail `index.html` — tiada dependency runtime luaran.
- **Navigasi papan kekunci**, penanda kemajuan, dan mod skrin penuh (`requestFullscreen`).
- **Kotak teks prompt boleh disalin** (`navigator.clipboard`) untuk borang, paparan data, log masuk dan prompt sistem penuh.
- **Slaid interaktif** untuk peserta memasukkan nama sistem, tujuan, pengguna, ciri, medan data dan pilihan penerbitan sebelum prompt penuh dijana.
- **Slaid 21 menjana kod Apps Script automatik** berdasarkan maklumat slaid interaktif, termasuk setup Google Sheets, `doGet(e)`, `doPost(e)` dan tab data.
- **Slaid 22 menyediakan panduan mengajar** langkah demi langkah supaya peserta faham objektif kelas, aliran sistem dan tindakan selepas setup.
- **Ujian statik automatik** (`tests/static.test.mjs`) yang menyemak kewujudan aset, saiz gambar, bilangan slaid (22), dan kandungan wajib deck.

## Kandungan Slaid

- Cara membina sistem web ringkas menggunakan alat percuma
- Google AI Studio dan Antigravity sebagai pembantu kod
- Google Sheets sebagai pangkalan data mudah
- Google Apps Script sebagai API ringkas (termasuk isu CORS)
- GitHub Pages dan Cloudflare Pages untuk penerbitan percuma
- Gambar sebenar berkaitan kod, spreadsheet dan ruang kerja pembangunan sebagai sokongan visual

### Sumber Gambar

Gambar sebenar dalam folder `assets` dimuat turun daripada Unsplash untuk kegunaan pembentangan pendidikan:

- Komputer riba dengan kod oleh Daniil Komov
- Paparan spreadsheet oleh Rodrigo Rodrigues | WOLF ART
- Ruang kerja kod oleh AltumCode

## Teknologi

| Lapisan | Teknologi |
|---|---|
| Markup & gaya | HTML5 + CSS3 (inline dalam `index.html`) |
| Interaktiviti | Vanilla JavaScript (navigasi, clipboard, fullscreen, penjana prompt & kod) |
| Ujian | Node.js (`node:assert`, `node:fs`) — `tests/static.test.mjs` |
| Preview lokal | `http-server` melalui `npx` (port 8026) |
| Hosting | **GitHub Pages** (branch `main`, folder `/root`) |

## Struktur Direktori

```text
SlideAkmalV1/
├── index.html                     # Keseluruhan deck 22 slaid (HTML + CSS + JS)
├── .nojekyll                      # Elak pemprosesan Jekyll di GitHub Pages
├── package.json                   # Skrip npm: test, start
├── tests/
│   └── static.test.mjs            # Ujian statik deck (aset, slaid, kandungan)
└── assets/
    ├── jata-negara.svg            # Logo Jata Negara
    ├── mohamad-nurakmal.png       # Potret pembentang
    ├── photo-code-laptop.jpg      # Gambar Unsplash (kod)
    ├── photo-spreadsheet.jpg      # Gambar Unsplash (spreadsheet)
    └── photo-workspace-code.jpg   # Gambar Unsplash (ruang kerja)
```

## Pemasangan

Perlukan Node.js (untuk ujian dan preview sahaja — laman itu sendiri statik):

```powershell
git clone https://github.com/akmal4244/SlideAkmalV1.git
cd SlideAkmalV1
npm test     # jalankan ujian statik
npm start    # hidangkan di http://localhost:8026
```

Alternatif: buka `index.html` terus dalam pelayar tanpa Node.

## Konfigurasi

Tiada fail `.env` atau konfigurasi luaran. Semua kandungan slaid dan gaya diedit terus dalam `index.html`. Pastikan `npm test` lulus selepas sebarang perubahan.

## Deployment

**GitHub Pages (kaedah utama):** repositori ini disediakan untuk GitHub Pages. Selepas perubahan dihantar ke `main`, Pages diterbitkan pada URL di atas menggunakan sumber cabang `main` dan folder `/root`.

**cPanel JimatHosting (domain production):** untuk hidangkan pada `slideakmalv1.akmalmarvis.com`, upload `index.html` dan folder `assets/` ke document root `/home2/akmalmar/public_html/slideakmalv1/` melalui cPanel File Manager.

## Status Projek

**Production** — laman live di GitHub Pages dan digunakan sebagai bahan taklimat/pembentangan.

## Kredit

Sistem Dibangunkan Sepenuhnya Oleh Akmal Marvis © 2026
