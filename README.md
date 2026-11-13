# Halo, saya Muhammad Muhdar

Saya pengembang sistem informasi kesehatan. Sejak 2024 saya membangun aplikasi yang dipakai sehari-hari di rumah sakit:
- mutu dan keselamatan pasien;
- laboratorium yang terhubung langsung ke alat analyzer;
- radiologi;
- formulir rekam medis yang melengkapi SIMRS.

Saya mengutamakan aplikasi yang mudah dipakai petugas di ruangan, mengikuti regulasi Kemenkes, dan tetap berjalan di server rumah sakit yang sederhana, tanpa bergantung pada internet.

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

## Sistem rumah sakit yang pernah saya bangun

Kode sistem berikut tidak dibuka untuk umum karena dipakai di lingkungan rumah sakit.

| Sistem | Yang dikerjakan | Teknologi |
|---|---|---|
| Sistem Informasi Laboratorium (LIS) | Order dari SIMRS atau petugas, label barcode sampel, konektor analyzer (HL7 v2, port serial), verifikasi hasil dengan nilai rujukan dan nilai kritis, kontrol kualitas Westgard dan grafik Levey-Jennings, laporan PDF, hasil kembali ke SIMRS | TypeScript monorepo, sebelumnya Laravel + Filament |
| Sistem Informasi Radiologi (RIS) | Papan kerja real-time, alur order sampai laporan yang disahkan dokter radiologi, cetak PDF berkop instansi, riwayat dan perbandingan hasil, peran dengan hak akses yang bisa diatur | Next.js 16, Drizzle, Tailwind CSS |
| Dokumen pendamping SIMRS | Formulir rekam medis yang belum ada di SIMRS: diisi seperti kertas, ditandatangani di signature pad, lalu otomatis menjadi PDF; data pasien dibaca dari SIMRS Khanza | Next.js, Prisma, MariaDB, Playwright |
| Aplikasi pendukung | Kepegawaian, presensi, keuangan dan aset, informasi tempat tidur, sistem klinik | PHP/Laravel, JavaScript |

## Keterampilan

- **Bahasa:** TypeScript, JavaScript, PHP, SQL
- **Web:** Next.js, React, NestJS, Express, Hono, Laravel + Filament, Tailwind CSS, shadcn/ui
- **Database:** PostgreSQL, MySQL/MariaDB, Drizzle, Prisma
- **Integrasi kesehatan:** HL7 v2, komunikasi port serial dengan alat laboratorium, integrasi dengan SIMRS
- **Operasional:** Docker Compose, Linux, backup dan pemulihan di server on-premise, Git

## Proyek lain

- [express-ts-boilerplate](https://github.com/mmuhdar/express-ts-boilerplate): boilerplate Express + TypeScript.
- [go-laundry-api](https://github.com/mmuhdar/go-laundry-api): API aplikasi laundry dengan NestJS dan Prisma.
- [tevim-vscode](https://github.com/mmuhdar/tevim-vscode): konfigurasi Neovim (TeVim) dengan key binding ala VS Code.

## Kontak

Email: mmuhdar@gmail.com. Untuk MutuRS, silakan buka [issue](https://github.com/mmuhdar/mutu-rs/issues) di repositorinya.
