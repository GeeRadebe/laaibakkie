# 🚛 LaaiBakkie

> On-demand bakkie & truck hire for South Africa. Like Uber — but for moving stuff.

## Live Demo
Deploy `laaibakkie.html` via GitHub Pages → `https://<username>.github.io/laaibakkie`

## Features
- Book ½-ton bakkie → 8-ton rigid truck
- Live driver matching with radar search
- Real-time trip tracking
- Helpers toggle (+R80 each)
- **⚡ Lightning Network payments** — BOLT11 invoice + Lightning Address
- Cash, Card, SnapScan/Ozow support
- Driver dashboard — earnings, job accept/decline, wallet
- Sats/BTC equivalent display (rate-locked at booking)
- Gauteng-first city set

## Lightning Payment
- Wallet: `tediousguilty29@walletofsatoshi.com`
- Invoice expires after 90s
- Rate: ZAR → sats conversion locked at booking time
- Compatible: Wallet of Satoshi, Zeus, Muun, Phoenix, Breez, Blue Wallet

## Stack
Single-file HTML — no build step, no dependencies to install.
- React 18 (CDN)
- Babel Standalone (CDN)
- Tailwind CSS (CDN)
- QRCode.js (CDN)

## Deploy to GitHub Pages
```bash
git init
git add laaibakkie.html README.md
git commit -m "feat: LaaiBakkie v1 — bakkie hire + Lightning payments"
git branch -M main
git remote add origin https://github.com/<username>/laaibakkie.git
git push -u origin main
```
Then: **Settings → Pages → Source: main / root** → rename `laaibakkie.html` to `index.html` or set it as the page root.

## Pricing Formula
```
Total = Base + (R/km × distance) + (helpers × R80)
```

## Roadmap
- [ ] Supabase backend + PostGIS driver geo-matching
- [ ] Google Maps SDK (replace grid placeholder)
- [ ] Peach Payments / Ozow API
- [ ] CIPC + NATIS driver verification
- [ ] Nostr-based driver/customer messaging
- [ ] Live BTC/ZAR rate feed (CoinGecko API)

## License
MIT — T⁴Tech Solutions · Boksburg, Gauteng
