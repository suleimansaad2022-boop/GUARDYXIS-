# GUARDYXIS V16 — Full Functional Build

This build extends the GUARDYXIS reference interface into an interactive dashboard where navigation and feature actions trigger their assigned data workflows.

## Functional areas
- Dashboard
- Solana token search / scanner
- Live market search through the GUARDYXIS backend
- Trending token retrieval through GeckoTerminal
- Real OHLCV retrieval and canvas candlestick rendering
- Risk/security retrieval through RugCheck
- Advanced holder retrieval and concentration display
- Evidence-backed Trust Score engine
- Watchlist persistence
- Alerts
- Reports / print-to-PDF
- Settings and data export
- Account / Google OAuth interface shell
- Desktop + mobile action ordering

## Trust Score
The score is a weighted evidence model:
- Contract Security: 25%
- Live Swap Activity: 20%
- Liquidity Depth: 20%
- Holder Concentration: 15%
- Official Announcements: 10%
- Status Conflicts: 10%

Only factors with provider evidence contribute to the current weighted result. Unknown evidence is shown as unknown rather than being silently treated as safe.

Bands:
- 90–100 Excellent
- 75–89 Good
- 60–74 Fair
- 40–59 Poor
- 0–39 Very Poor

## Run
Node.js 18+:
1. `npm install`
2. `npm start`
3. Open `http://localhost:8787`

The app uses server-side provider routing so browser CORS issues are reduced. Provider outages/rate limits are surfaced rather than represented as live data.

Google authentication remains an OAuth UI shell until real Google/Firebase credentials are configured.
