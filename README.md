# Hi, I'm Muhammad Muhdar

I build software for hospitals. Since 2024, I've been making the apps hospital staff use every day:
- quality and patient safety
- lab systems that talk straight to the analyzers
- radiology
- medical record forms that fill the gaps in the hospital's main system (SIMRS)

I like keeping things practical: easy for ward staff to pick up, in line with Indonesia's Ministry of Health rules, and happy to run on a modest hospital server with no internet needed.

## Proyek open source

### [MutuRS](https://github.com/mmuhdar/mutu-rs)

Aplikasi indikator mutu rumah sakit, dari pengisian data ruangan sampai laporan ke Direktur, Dewan Pengawas, dan SIMAR Kemenkes. Isinya:
- 13 INM sesuai PMK 30/2022;
- verifikasi oleh Kepala Unit;
- Capaian ΣN/ΣD dengan Kelengkapan;
- Analisis, Tindak Lanjut, dan PDSA;
- validasi data PMKP 5;
- Laporan Triwulan dan Rekap SIMAR;
- insiden keselamatan pasien (PMK 11/2017);
- register risiko.

Dibangun dengan Next.js 16, PostgreSQL, dan Docker Compose, berlisensi AGPL-3.0.

[![Dashboard MutuRS](https://raw.githubusercontent.com/mmuhdar/mutu-rs/main/docs/gambar/dashboard.png)](https://github.com/mmuhdar/mutu-rs)

### [laris](https://github.com/mmuhdar/laris)

Aplikasi kasir (POS) desktop untuk toko kecil dan UMKM: warung, toko kelontong, dan minimarket kecil. Berjalan offline penuh di satu komputer, semua data ada di satu file, dan struk dicetak di printer thermal apa saja. Isinya:
- kasir dengan scan barcode, tombol cepat, harga grosir, dan satuan dus atau pak;
- bayar tunai, QRIS, transfer, kartu, atau kasbon;
- stok masuk dari pemasok, hutang pemasok, stok opname, dan mutasi stok;
- pelanggan dengan kasbon, batas kasbon, dan poin;
- retur sebagian, shift kasir, kas masuk/keluar, dan pengeluaran;
- laporan omzet, laba kotor dan bersih, jam ramai, dan nilai stok;
- pajak opsional, label harga dengan barcode, dan PIN pemilik.

Dibangun dengan Tauri 2, Rust + SQLite, dan SvelteKit, berlisensi GPL-3.0.

[![Layar Kasir laris](https://raw.githubusercontent.com/mmuhdar/laris/main/docs/screenshots/kasir.png)](https://github.com/mmuhdar/laris)

## Sistem rumah sakit yang pernah saya bangun

Kode sistem berikut tidak dibuka untuk umum karena dipakai di lingkungan rumah sakit.

| Sistem | Yang dikerjakan | Teknologi |
|---|---|---|
| Sistem Informasi Laboratorium (LIS) | Order dari SIMRS atau petugas, label barcode sampel, konektor analyzer (HL7 v2, port serial), verifikasi hasil dengan nilai rujukan dan nilai kritis, kontrol kualitas Westgard dan grafik Levey-Jennings, laporan PDF, hasil kembali ke SIMRS | TypeScript monorepo, sebelumnya Laravel + Filament |
| Sistem Informasi Radiologi (RIS) | Papan kerja real-time, alur order sampai laporan yang disahkan dokter radiologi, cetak PDF berkop instansi, riwayat dan perbandingan hasil, peran dengan hak akses yang bisa diatur | Next.js 16, Drizzle, Tailwind CSS |
| Dokumen pendamping SIMRS | Formulir rekam medis yang belum ada di SIMRS: diisi seperti kertas, ditandatangani di signature pad, lalu otomatis menjadi PDF; data pasien dibaca dari SIMRS Khanza | Next.js, Prisma, MariaDB, Playwright |
| Aplikasi pendukung | Kepegawaian, presensi, keuangan dan aset, informasi tempat tidur, sistem klinik | PHP/Laravel, JavaScript |

## Tech stack

- <img src="https://skillicons.dev/icons?i=ts" width="20" height="20" alt="" align="top"> TypeScript
- <img src="https://skillicons.dev/icons?i=js" width="20" height="20" alt="" align="top"> JavaScript
- <img src="https://skillicons.dev/icons?i=php" width="20" height="20" alt="" align="top"> PHP
- <img src="https://skillicons.dev/icons?i=rust" width="20" height="20" alt="" align="top"> Rust
- <img src="https://skillicons.dev/icons?i=nodejs" width="20" height="20" alt="" align="top"> Node.js
- <img src="https://skillicons.dev/icons?i=nextjs" width="20" height="20" alt="" align="top"> Next.js
- <img src="https://skillicons.dev/icons?i=react" width="20" height="20" alt="" align="top"> React
- <img src="https://skillicons.dev/icons?i=svelte" width="20" height="20" alt="" align="top"> Svelte, SvelteKit
- <img src="https://skillicons.dev/icons?i=tauri" width="20" height="20" alt="" align="top"> Tauri (aplikasi desktop)
- <img src="https://skillicons.dev/icons?i=nestjs" width="20" height="20" alt="" align="top"> NestJS
- <img src="https://skillicons.dev/icons?i=express" width="20" height="20" alt="" align="top"> Express, Hono
- <img src="https://skillicons.dev/icons?i=laravel" width="20" height="20" alt="" align="top"> Laravel + Filament
- <img src="https://skillicons.dev/icons?i=tailwind" width="20" height="20" alt="" align="top"> Tailwind CSS
- <img src="https://skillicons.dev/icons?i=postgres" width="20" height="20" alt="" align="top"> PostgreSQL
- <img src="https://skillicons.dev/icons?i=mysql" width="20" height="20" alt="" align="top"> MySQL / MariaDB
- <img src="https://skillicons.dev/icons?i=sqlite" width="20" height="20" alt="" align="top"> SQLite
- <img src="https://skillicons.dev/icons?i=prisma" width="20" height="20" alt="" align="top"> Prisma, Drizzle
- <img src="https://skillicons.dev/icons?i=docker" width="20" height="20" alt="" align="top"> Docker
- <img src="https://skillicons.dev/icons?i=linux" width="20" height="20" alt="" align="top"> Linux
- <img src="https://skillicons.dev/icons?i=git" width="20" height="20" alt="" align="top"> Git

Di sisi integrasi kesehatan: HL7 v2, komunikasi port serial dengan alat laboratorium, dan integrasi dengan SIMRS. Terbiasa memasang aplikasi di server rumah sakit sendiri (on-premise), lengkap dengan backup dan pemulihannya.

## Proyek lain

- [express-ts-boilerplate](https://github.com/mmuhdar/express-ts-boilerplate): boilerplate Express + TypeScript.
- [go-laundry-api](https://github.com/mmuhdar/go-laundry-api): API aplikasi laundry dengan NestJS dan Prisma.
- [tevim-vscode](https://github.com/mmuhdar/tevim-vscode): konfigurasi Neovim (TeVim) dengan key binding ala VS Code.

## Kontak

Email: mmuhdar@gmail.com. Untuk MutuRS atau laris, silakan buka issue di repositorinya masing-masing: [MutuRS](https://github.com/mmuhdar/mutu-rs/issues), [laris](https://github.com/mmuhdar/laris/issues).
