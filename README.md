# Hi, I'm Muhammad Muhdar

I build software for hospitals. Since 2024, I've been making the apps hospital staff use every day:
- quality and patient safety
- lab systems that talk straight to the analyzers
- radiology
- medical record forms that fill the gaps in the hospital's main system (SIMRS)

I like keeping things practical: easy for ward staff to pick up, in line with Indonesia's Ministry of Health rules, and happy to run on a modest hospital server with no internet needed.

## Open source

### [MutuRS](https://github.com/mmuhdar/mutu-rs)

A quality indicator app for Indonesian hospitals. It covers the whole loop, from ward staff entering monthly data to reports for the director, the supervisory board, and the Ministry's SIMAR system:
- the 13 national quality indicators (INM, PMK 30/2022)
- verification by unit heads
- hospital-wide results calculated as ΣN/ΣD, with completeness tracking
- analysis, follow-ups, and PDSA cycles
- data validation (PMKP 5)
- quarterly reports and SIMAR recap
- patient safety incidents (PMK 11/2017)
- risk register

Built with Next.js 16, PostgreSQL, and Docker Compose. Licensed under AGPL-3.0.

[![MutuRS dashboard](https://raw.githubusercontent.com/mmuhdar/mutu-rs/main/docs/gambar/dashboard.png)](https://github.com/mmuhdar/mutu-rs)

## Hospital systems I've built

These ones are private, since they run inside a hospital.

| System | What it does | Stack |
|---|---|---|
| Laboratory Information System (LIS) | Takes orders from SIMRS or lab staff, prints barcode labels for samples, pulls results from analyzers (HL7 v2, serial port), checks them against reference ranges and critical values, runs QC with Westgard rules and Levey-Jennings charts, prints PDF reports, and sends results back to SIMRS | TypeScript monorepo, rebuilt from Laravel + Filament |
| Radiology Information System (RIS) | Real-time worklist, the full flow from order to a report signed off by the radiologist, PDF printouts with the hospital letterhead, patient history and side-by-side comparison, configurable roles and permissions | Next.js 16, Drizzle, Tailwind CSS |
| SIMRS companion forms | Medical record forms that SIMRS doesn't have yet: filled in like paper, signed on a signature pad, and turned into a PDF automatically; patient data is read from SIMRS Khanza | Next.js, Prisma, MariaDB, Playwright |
| Supporting apps | HR, attendance, finance and assets, bed availability, clinic system | PHP/Laravel, JavaScript |

## Tech stack

- <img src="https://skillicons.dev/icons?i=ts" width="20" height="20" alt="" align="top"> TypeScript
- <img src="https://skillicons.dev/icons?i=js" width="20" height="20" alt="" align="top"> JavaScript
- <img src="https://skillicons.dev/icons?i=php" width="20" height="20" alt="" align="top"> PHP
- <img src="https://skillicons.dev/icons?i=nodejs" width="20" height="20" alt="" align="top"> Node.js
- <img src="https://skillicons.dev/icons?i=nextjs" width="20" height="20" alt="" align="top"> Next.js
- <img src="https://skillicons.dev/icons?i=react" width="20" height="20" alt="" align="top"> React
- <img src="https://skillicons.dev/icons?i=nestjs" width="20" height="20" alt="" align="top"> NestJS
- <img src="https://skillicons.dev/icons?i=express" width="20" height="20" alt="" align="top"> Express, Hono
- <img src="https://skillicons.dev/icons?i=laravel" width="20" height="20" alt="" align="top"> Laravel + Filament
- <img src="https://skillicons.dev/icons?i=tailwind" width="20" height="20" alt="" align="top"> Tailwind CSS
- <img src="https://skillicons.dev/icons?i=postgres" width="20" height="20" alt="" align="top"> PostgreSQL
- <img src="https://skillicons.dev/icons?i=mysql" width="20" height="20" alt="" align="top"> MySQL / MariaDB
- <img src="https://skillicons.dev/icons?i=prisma" width="20" height="20" alt="" align="top"> Prisma, Drizzle
- <img src="https://skillicons.dev/icons?i=docker" width="20" height="20" alt="" align="top"> Docker
- <img src="https://skillicons.dev/icons?i=linux" width="20" height="20" alt="" align="top"> Linux
- <img src="https://skillicons.dev/icons?i=git" width="20" height="20" alt="" align="top"> Git

On the healthcare side, I work with HL7 v2, serial connections to lab instruments, and SIMRS integrations. I'm also used to running apps on the hospital's own servers, backups and restores included.

## Other projects

- [express-ts-boilerplate](https://github.com/mmuhdar/express-ts-boilerplate): an Express + TypeScript starter.
- [go-laundry-api](https://github.com/mmuhdar/go-laundry-api): a laundry app API built with NestJS and Prisma.
- [tevim-vscode](https://github.com/mmuhdar/tevim-vscode): my Neovim (TeVim) setup with VS Code-style key bindings.

## Get in touch

Email me at mmuhdar@gmail.com. For MutuRS, feel free to open an [issue](https://github.com/mmuhdar/mutu-rs/issues).
