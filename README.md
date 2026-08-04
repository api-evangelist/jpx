# JPX (Japan Exchange Group) (jpx)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
