# QR Code Generator

A beautiful, fast, and privacy-friendly QR Code Generator built with pure HTML, CSS, and JavaScript. No frameworks, no backend, no tracking â€” everything runs in your browser.

Enter any text or URL and generate a QR code instantly. Fully supports Unicode, including Khmer, Thai, Chinese, Arabic, emoji, and more.

## âœ¨ Features

- **Instant generation** â€” type text or a URL, hit Generate (or press Enter)
- **Full Unicode / UTF-8 support** â€” Khmer, Thai, Chinese, Arabic, emoji, etc. all encode correctly and decode on every phone scanner
- **Smart error correction** â€” automatically picks the best level (H â†’ Q â†’ M â†’ L) so you get maximum data capacity and scannability
- **Live byte counter** â€” shows your text size against the ~2,900-byte QR limit
- **High-quality downloads** â€” crisp 600px PNG with a proper quiet zone
- **Dark & light mode** â€” toggle in the header; remembers your choice and follows your system preference on first visit
- **Fixed frosted-glass header** â€” stays visible while scrolling
- **Fully responsive** â€” works great on phones, tablets, and desktops
- **Zero backend** â€” your text never leaves your device

## ðŸš€ Live Demo

Hosted on GitHub Pages:

```
https://<your-username>.github.io/<repo-name>/
```

## ðŸ› ï¸ Tech Stack

| Piece | Choice |
|---|---|
| Structure & styling | Plain HTML + CSS (custom properties for theming) |
| QR encoding | [qrcode-generator](https://www.npmjs.com/package/qrcode-generator) v1.4.4 (UTF-8 byte mode, via CDN) |
| Rendering | HTML5 Canvas |
| Khmer input font | [Noto Sans Khmer](https://fonts.google.com/noto/specimen/Noto+Sans+Khmer) (via Google Fonts) |

No build step, no dependencies to install.

## ðŸ“¦ Getting Started

### Run locally
1. Download or clone this repository
2. Open `index.html` in any modern browser â€” that's it!

```bash
git clone https://github.com/<your-username>/<repo-name>.git
cd <repo-name>
# then just open index.html in your browser
```

### Deploy on GitHub Pages
1. Create a new repository on GitHub
2. Upload `index.html` (and `README.md`)
3. Go to **Settings â†’ Pages**
4. Under **Source**, pick **Deploy from a branch** â†’ **main** / **(root)** â†’ **Save**
5. Your site goes live at `https://<your-username>.github.io/<repo-name>/` in about a minute

## ðŸ“ Limits (QR standard)

A single QR code (version 40, byte mode) holds up to **~2,950 bytes**:

- ~1,250 characters with the highest error correction (H)
- Roughly **~980 Khmer characters** (Khmer takes 3 bytes per character in UTF-8)

The tool warns you as you approach the limit. Very long codes get dense â€” for best scanning, keep text under ~1,000 characters.

## ðŸ“„ License

Released under the [MIT License](LICENSE). Feel free to use, modify, and share.

## ðŸ’š Credits

Created with â¤ï¸ by **[Lai Honest](https://facebook.com/mizterlai)**
