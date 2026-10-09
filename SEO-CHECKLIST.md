# SEO & Speed Checklist — setiap situs client baru

Dipakai sebelum demo dikirim ke customer. Template dari audit bajuanak.fatanakbar.my.id (2026-10-06).

## Wajib (sales-visible)
- [ ] `<title>` ≤ 60 karakter, ada keyword brand/niche
- [ ] `<meta name="description">` ≤ 160 karakter, kalimat ajakan
- [ ] **Open Graph tags**: og:title, og:description, og:image (URL ABSOLUT), og:url, og:type — biar preview WhatsApp/Telegram muncul kartu, bukan link polos
- [ ] Twitter Card `summary_large_image`
- [ ] `<link rel="canonical">` ke URL final
- [ ] `lang="id"` di `<html>`

## Struktur konten
- [ ] Satu `<h1>` per halaman, H2 deskriptif per section
- [ ] Semua `<img>` punya `alt` deskriptif (bukan "image1.jpg")
- [ ] robots.txt + sitemap.xml ada dan return 200

## Kecepatan (target: < 1MB total assets)
- [ ] Foto ≤ ~150KB per file (JPEG q70-75, progressive); resize ke lebar tampil maks
- [ ] Hero: `fetchpriority="high"`, jangan lazy
- [ ] Gambar bawah-fold: `loading="lazy"` + `decoding="async"`
- [ ] CSS/JS inline kalau kecil; hindari render-blocking berat
- [ ] Test curl: HTML < 50KB, TTFB < 1s

## Jangan lupa
- [ ] Backup file asli sebelum kompres (raw/orig_backup/)
- [ ] Setelah edit: mirror ke folder deploy + redeploy + verifikasi live (curl + cek preview WA)

Skor acuan: bajuanak demo ~8/10 setelah pass ini (naik ke ~9 dengan WebP/AVIF + preload hero).
