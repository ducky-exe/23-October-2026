# Love Replay — Tyrell & Smelokuhle

A fully static, mobile-friendly, seven-chapter love-story website. **All 13 photographs are included**, and the filename references are already connected.

## Photo mapping

| File | Location |
|------|----------|
| `photos/1.jpg` | Chapter 2 — How It All Started; Chapter 5 collage first image |
| `photos/2.jpg` | Chapter 2 — A Day We'll Never Forget |
| `photos/3.jpg` | Chapter 2 — First Date, Kinda (Gold Reef City); Chapter 5 collage third image |
| `photos/4.jpg` | Chapter 2 — Early Favourites (Prize Giving) |
| `photos/5.jpg` | Chapter 2 — Matric Dance 2025 (converted from your HEIC upload) |
| `photos/6.jpg` | Chapter 6 — Sky City Visit; also the Chapter 7 finale background |
| `photos/7.jpg` | Chapter 4 — The Human Comfort Blanket Award AND Most Likely to Cry at a Movie |
| `photos/8.jpg` | Chapter 4 — The Biggest Softie |
| `photos/9.jpg` | Chapter 4 — Cutest Unplanned Moment |
| `photos/10.jpg` | Chapter 4 — Most Iconic Couple Moment |
| `photos/11.jpg` | Chapter 5 — Mall of the South (29 January 2026) |
| `photos/12.jpg` | Chapter 5 — Home Visit (6 April 2026) |
| `photos/13.jpg` | Chapter 5 — Dedicated middle collage photo |

The Chapter 5 collage uses **1 → 13 → 3**. All filenames are lowercase `.jpg`; the converted images have correct orientation. Embedded camera/GPS EXIF metadata was removed from the published JPGs.

## Deploy to Vercel using GitHub

1. **Unzip** the download. Open `Love-Replay-Ready-to-Deploy` and select its **contents**, including `index.html` and `photos/`.
2. Create a new GitHub repository and upload those contents **to the repository root** (not inside an extra folder).
3. In Vercel select **Add New → Project**, import your GitHub repository.
4. Choose framework preset **Other** (or leave it auto-detected as static), root directory `./`, and **no build command**.
5. Select **Deploy**. Vercel serves root `index.html` as the homepage.

You can also double-click `index.html` to preview locally; some browsers may handle audio differently when opened as a local file.

## If you want to edit anything later

Open `index.html` and find `/* ============ EDIT EVERYTHING HERE ============ */`. The `C` configuration controls the names, dates, stories, award answers, numbered photos, and optional chapter music. The remainder is the presentation engine.

## Chapter music (titles are configured; actual audio files not yet included)

Every screen shows its chapter song title and artist in the bottom music bar. The website is **already linked** to these paths; no code edits are necessary once MP3s are added:

| Chapter | Song shown on screen | File to add |
|---|---|---|
| 1 — Homepage | Rain Dance — Dave & Tems | `audio/ch1.mp3` |
| 2 — Our Story Began | Me and You — Tems | `audio/ch2.mp3` |
| 3 — Two Years / Our Wrapped | Eh Joh — Sam Deep | `audio/ch3.mp3` |
| 4 — Relationship Wrapped Awards | Shela — Sam Deep | `audio/ch4.mp3` |
| 5 — The Memories | Distant Lover — Marvin Gaye | `audio/ch5.mp3` |
| 6 — My Favourite Person | Ordinary — Alex Warren | `audio/ch6.mp3` |
| 7 — Finale | Sure Thing (Slowed) — Miguel | `audio/ch7.mp3` |

**Important:** The songs themselves are **not** in this ZIP. Until you provide the MP3 files, the website will play its built-in ambient track as a fallback, even though the desired song name appears in the footer. For chapter 1, tap the bottom play control while on the homepage to start its music; the main story button advances immediately to chapter 2. Browsers require a tap or click before audio playback. Only deploy audio recordings you have permission to publish.

## Notes

- No Node.js, npm dependencies, build step, or environment variables required.
- Photos are kept at their original visible resolution and exported as high-quality JPGs with orientation corrected.
- The opening screen says **2024–2026** and celebrates the two-year anniversary on **23 October 2026** (as written in the supplied site).
- The existing sample words in the "Our Wrapped" text tiles have intentionally been preserved rather than filled in with invented answers.
