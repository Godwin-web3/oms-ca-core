# OMS + Corporate Actions Core

Chain-agnostic foundation for **corporate actions and beneficial ownership** on tokenized stocks.

Order management is a secondary module.

## Primary product

A shared layer that correctly handles dividends, splits, reverse splits, ticker changes, and spinoffs, and resolves beneficial ownership when tokens sit in wallets, vaults, or other contracts.

Useful for:
- Lending protocols (collateral accuracy after splits/dividends)
- Wallets and portfolio trackers
- Tax and accounting tools
- Market makers and prop shops
- Any system that holds or uses tokenized stocks

## Consumer app

Static positions viewer deployed at: https://oms-ca-positions.vercel.app

Paste a wallet on Robinhood Chain (or other supported chains) to see corrected holdings after corporate actions.

## Setup

```bash
npm install
cp .env.example .env
# fill SUPABASE_URL, SUPABASE_KEY, FMP_API_KEY
npm run api
```

See TOKENS.md for real contract addresses.
