# GUARDYXIS Fresh Site

A clean, functional market-intelligence frontend using live DexScreener market endpoints. It deliberately does not invent trending tokens, user history, security results, or placeholder actions.

## Included working features
- Live token/pair search
- Live trending discovery from DexScreener boosts
- Pair detail pages
- Live price/24h change/volume/liquidity/transactions
- Watchlist persisted in localStorage
- Functional alerts storage
- Dark/light theme persistence
- Refresh preference
- Responsive mobile layout
- GUARDYXIS trust-score presentation with explicit market-data limitations
- Error/empty/loading states

## Security integration
The browser must not contain a private security API key. The next production step is to connect the Netlify serverless function layer to GoPlus using an environment variable, then replace the estimated contract/holder portions of the score with verified security/holder evidence.

## Deploy
Upload the folder to Netlify or GitHub Pages. For the server-side security layer, use Netlify Functions and configure the provider secret in Netlify environment variables.
