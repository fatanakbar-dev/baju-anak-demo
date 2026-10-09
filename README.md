# Baju Anak Demo — "Si Kecil"

Mockup company profile 1 halaman untuk brand baju anak. Dibuat sebagai demo
portofolio untuk [AhliWebMurah](https://ahliwebmurah.my.id).

> **Catatan:** "Si Kecil" adalah nama placeholder — nama brand final menyusul
> dari klien.

## Live

- https://demo.ahliwebmurah.my.id (domain portofolio AhliWebMurah)

## Struktur

```
index.html          Halaman utama (1 halaman, section: hero, koleksi, tentang, kontak)
assets/             Gambar (hero, koleksi, tentang)
robots.txt          SEO
sitemap.xml         SEO
SEO-CHECKLIST.md    Checklist optimasi SEO demo
```

## Tech

HTML + CSS statis (tanpa build step), di-deploy sebagai Cloudflare Worker
dengan routes `demo.ahliwebmurah.my.id/*`. Tombol WhatsApp masih placeholder.

## Update

Setiap perubahan source di-push ke repo ini, lalu di-deploy ulang via wrangler.
