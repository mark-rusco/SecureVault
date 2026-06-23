# SecureVault v3 — Password & Crypto Seed Phrase Manager (PWA)

Clean modern UI inspired by the Tarsi app design. Mobile-first, offline-first PWA with real client-side encryption.

## Highlights
- Bold typographic headers (30px title, subtle subtitle)
- Plain stroke SVG icons throughout (no emoji clutter)
- Outlined pill filter tabs (All / Strong / Weak / Recent)
- White background with green accent, soft shadows
- Floating pill-shaped bottom navigation + separate green FAB
- Vibrant solid-color cards with per-card color customization (12 swatches)
- Per-card password strength meter with label
- Inline INSIGHT card (quote-style) + WEEKLY ACTIVITY mini-bars
- Full Insights tab: vault health, donut chart, weekly bars, strength breakdown
- 20 website templates + 10 wallet templates with auto favicons
- AES-GCM 256 / PBKDF2-SHA256 250k iterations
- Auto-lock on idle, encrypted backup/restore, master password change
- Fully responsive (1/2/3/4 columns), safe-area aware, PWA installable

## Files
| File | Purpose |
|------|---------|
| `index.html` | Shell + styles |
| `app.js` | Logic, crypto, render, insights |
| `sw.js` | Service worker (offline) |
| `manifest.webmanifest` | PWA manifest |
| `icon-192.png`, `icon-512.png` | App icons |

## Deploy
Upload all files to any HTTPS host (GitHub Pages, Netlify, Vercel). HTTPS is required for PWA install + Service Worker.

## Security
- AES-GCM 256-bit encryption via Web Crypto API
- PBKDF2-SHA256, 250,000 iterations
- Vault decrypted only in RAM; wiped on lock & idle
- Clipboard auto-clears 30s after copy
- No recovery by design — export an encrypted backup right after setup
