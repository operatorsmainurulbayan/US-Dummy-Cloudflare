# US Dummy Cloudflare Worker

Backend TEST untuk aplikasi Android US (Ujian Sekolah).

## Struktur
- `public/index.html`
- `src/index.js`
- `wrangler.jsonc`

## Cloudflare
Jika memakai Wrangler:
- Build command: `exit 0`
- Deploy command: `npx wrangler deploy`
- Preview command: `npx wrangler preview`

Setelah deploy, tes:
- `https://NAMA-WORKER.workers.dev/api/health`
- `https://NAMA-WORKER.workers.dev/api/exam`

`/api/exam` harus mengembalikan 5 soal dummy. `/api/submit` menerima POST JSON dari aplikasi Android.

Ini hanya backend TEST. Backend produksi tetap gunakan Supabase.
