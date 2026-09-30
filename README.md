# GUARDYXIS V14 — Reference Complete

This build is a careful UI/interaction reconstruction of the supplied GUARDYXIS reference image.

## Included
- Dashboard with stat cards, trending cards, recent scans and security banner
- Token Scan with market metrics, candlestick-style chart, risk panel and watchlist/share actions
- Trending table with filters and GeckoTerminal refresh attempt
- Charts page
- Risk Analysis
- Advanced Holder Intelligence UI
- Watchlist with local persistence
- Alerts
- Reports + print/save-PDF
- Settings
- Account/Google OAuth UI shell
- Responsive mobile navigation
- DexScreener live token search with safe fallback data
- Minimal Express backend with RugCheck security endpoint
- No wallet private keys or passwords are collected

## Run
1. Install Node.js 18+.
2. `npm install`
3. `npm start`
4. Open `http://localhost:8787`

## Important
The Google sign-in screen is a UI shell only. Production authentication must be connected to a real OAuth/Firebase/Google Identity configuration.

Market/security providers can rate-limit or become unavailable. The interface therefore distinguishes live provider results from safe fallback demo values instead of pretending fallback data is live.
