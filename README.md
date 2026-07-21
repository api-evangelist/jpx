# JPX (Japan Exchange Group) (jpx)

JPX (Japan Exchange Group) operates the Tokyo Stock Exchange, Osaka Exchange, and Tokyo Commodity Exchange, and sells Japanese market data through its JPX Market Innovation & Research arm. Its developer-facing product is the J-Quants API - a self-serve, subscription REST API (Free/Light/Standard/Premium plans, x-api-key auth, base https://api.jquants.com/v2) delivering historical equities OHLCV/minute/tick bars, indices, derivatives, financial statements, short-selling and margin data, EDINET filings, and TDnet disclosures, plus bulk CSV download, an MCP server, and a CLI - licensed to individual investors only. Institutional real-time data (FLEX Standard and FLEX MBO order-book feeds) and corporate historical data (J-Quants Pro via API/SFTP/Snowflake, J-Quants DataCube) are sales-gated services.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/jpx/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/jpx/refs/heads/main/apis.yml)

## Tags

- Financial
- Market Data
- Stocks
- Exchange
- Trading
- Derivatives
- Indices
- Reference Data
- Japan

## Timestamps

- **Created:** 2026-07-21
- **Modified:** 2026-07-21

## APIs

### J-Quants Equities API

Listed issue master, daily and morning-session OHLCV, minute bars and tick trades (add-on), earnings calendar, and weekly trading by investor type for Tokyo Stock Exchange equities, under /v2/equities/* endpoints.

- **Human URL:** [https://jpx-jquants.com/en/spec/eq-master](https://jpx-jquants.com/en/spec/eq-master)
- **Base URL:** `https://api.jquants.com/v2`

#### Tags

- Stocks
- OHLCV
- Tick Data
- Listed Issues

#### Properties

- [Documentation](https://jpx-jquants.com/en/spec/eq-master)
- [API Reference](https://jpx-jquants.com/en/spec/eq-bars-daily)

### J-Quants Markets API

Market-structure datasets under /v2/markets/* - trading calendar, short sale position reports, short ratio by sector, weekly margin interest, daily margin alerts, and breakdown trading data.

- **Human URL:** [https://jpx-jquants.com/en/spec/mkt-cal](https://jpx-jquants.com/en/spec/mkt-cal)
- **Base URL:** `https://api.jquants.com/v2`

#### Tags

- Short Selling
- Margin Trading
- Trading Calendar

#### Properties

- [Documentation](https://jpx-jquants.com/en/spec/mkt-cal)
- [API Reference](https://jpx-jquants.com/en/spec/mkt-short-sale)

### J-Quants Indices API

Daily OHLC for TOPIX and other JPX indices under /v2/indices/* endpoints, with plan-gated access (TOPIX from Light, full index set from Standard).

- **Human URL:** [https://jpx-jquants.com/en/spec/idx-bars-daily](https://jpx-jquants.com/en/spec/idx-bars-daily)
- **Base URL:** `https://api.jquants.com/v2`

#### Tags

- Indices
- TOPIX

#### Properties

- [Documentation](https://jpx-jquants.com/en/spec/idx-bars-daily)
- [API Reference](https://jpx-jquants.com/en/spec/idx-bars-daily-topix)

### J-Quants Financials API

Corporate financial data under /v2/fins/* - summary report figures (EPS, forecasts), detailed BS/PL/CF statements, and cash dividend data sourced from TDnet disclosures.

- **Human URL:** [https://jpx-jquants.com/en/spec/fin-summary](https://jpx-jquants.com/en/spec/fin-summary)
- **Base URL:** `https://api.jquants.com/v2`

#### Tags

- Financial Statements
- Dividends
- Fundamentals

#### Properties

- [Documentation](https://jpx-jquants.com/en/spec/fin-summary)
- [API Reference](https://jpx-jquants.com/en/spec/fin-details)

### J-Quants Derivatives API

Daily OHLC for Osaka Exchange futures and options under /v2/derivatives/*, including Nikkei 225 options (Standard plan) and the full futures/options universe (Premium plan).

- **Human URL:** [https://jpx-jquants.com/en/spec/drv-bars-daily-fut](https://jpx-jquants.com/en/spec/drv-bars-daily-fut)
- **Base URL:** `https://api.jquants.com/v2`

#### Tags

- Futures
- Options
- Derivatives

#### Properties

- [Documentation](https://jpx-jquants.com/en/spec/drv-bars-daily-fut)
- [API Reference](https://jpx-jquants.com/en/spec/drv-bars-daily-opt)

### J-Quants EDINET Data API

Structured data extracted from EDINET regulatory filings under /v2/edinet/* - major shareholders, cross-shareholdings (policy holdings), and large volume holding reports.

- **Human URL:** [https://jpx-jquants.com/en/spec/edinet-major-shareholders](https://jpx-jquants.com/en/spec/edinet-major-shareholders)
- **Base URL:** `https://api.jquants.com/v2`

#### Tags

- EDINET
- Shareholders
- Filings

#### Properties

- [Documentation](https://jpx-jquants.com/en/spec/edinet-major-shareholders)
- [API Reference](https://jpx-jquants.com/en/spec/edinet-cross-shareholdings)

### J-Quants TDnet Disclosure API

Add-on access to TDnet timely-disclosure documents - a disclosure index (/td/list), document file retrieval (/td/files), and bulk CSV download (/td/bulk) covering five years of filings.

- **Human URL:** [https://jpx-jquants.com/en/spec/td-list](https://jpx-jquants.com/en/spec/td-list)
- **Base URL:** `https://api.jquants.com/v2`

#### Tags

- TDnet
- Disclosures
- Documents

#### Properties

- [Documentation](https://jpx-jquants.com/en/spec/td-list)
- [API Reference](https://jpx-jquants.com/en/spec/td-files)

### J-Quants Bulk Download API

File-based delivery alongside the REST endpoints - list available bulk files (/bulk/list) and download gzipped CSV extracts (/bulk/get) for supported datasets.

- **Human URL:** [https://jpx-jquants.com/en/spec/bulk](https://jpx-jquants.com/en/spec/bulk)
- **Base URL:** `https://api.jquants.com/v2`

#### Tags

- Bulk
- CSV
- Files

#### Properties

- [Documentation](https://jpx-jquants.com/en/spec/bulk)
- [API Reference](https://jpx-jquants.com/en/spec/bulk-list)

## Common Properties

- [Website](https://www.jpx.co.jp/english/)
- [Portal](https://jpx-jquants.com/en)
- [Documentation](https://jpx-jquants.com/en/spec)
- [GitHub Organization](https://github.com/J-Quants)
- [LinkedIn](https://www.linkedin.com/company/japan-exchange-group)
- [Blog](https://qiita.com/j_quants)
- [Pricing](https://jpx-jquants.com/en#pricing)
- [Sign Up](https://jpx-jquants.com/en/register)
- [Terms of Service](https://www.jpx.co.jp/english/term-of-use/index.html)
- [Privacy Policy](https://www.jpx.co.jp/english/corporate/governance/security/personal-information/index.html)
- [Support](https://jpx-jquants.com/en/help)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
