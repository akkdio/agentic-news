# State of Agentic Commerce

**Brief updated:** 2026-11-18  
**Corpus coverage through:** 2026-11-18  
**Sources:**  
- [`sources/2026-11-18-chatgpt-wallet-merchant-checkout.md`](../sources/2026-11-18-chatgpt-wallet-merchant-checkout.md)  
- [`sources/stripe vs shopify agentic.md`](../sources/stripe%20vs%20shopify%20agentic.md)  
- [`sources/2026-11-16-openai-wallet-plaid-imprint.md`](../sources/2026-11-16-openai-wallet-plaid-imprint.md)  
- [`sources/11.14.26.md`](../sources/11.14.26.md)  
- [`sources/11.10.26 udpate - Executive Summary.md`](../sources/11.10.26%20udpate%20-%20Executive%20Summary.md)  
- [`briefs/competing-protocols.md`](competing-protocols.md)

## Snapshot

Agentic commerce is **real but tiny in GMV**. OpenAI’s **ChatGPT Wallet** (Nov 13 limited Pro rollout with Amex, Chase, Mastercard, Visa) doubles down on **merchant-owned checkout + network tokens**, after Instant Checkout. The fight remains **trust / intent / fraud false positives**, **bot auth at the CDN**, and **VCN bootstrap vs network-token rails**.

## From sources

### ChatGPT Wallet (newest product facts)

- Launched **Nov 13** with **Amex, Chase, Mastercard, Visa**; limited **U.S. ChatGPT Pro**; dots pay via **merchants’ existing checkouts**, not in-ChatGPT Instant Checkout. *(2026-11-18 article)*
- Strategy arc: Instant Checkout (Sep 2025) → merchant apps (Mar) → Wallet “fit existing systems.” *(same)*
- Per-purchase biometric approval → **network token**; merchant and agent never see PAN; rewards/dispute protections retained. Full delegation (spend/category/time limits) is future-state. *(same + prior analysis note)*
- **Commerce Partner Playbook**; claim/verify business; **Web Bot Auth** for CDN/firewall; **WebMCP** for cart/availability; PSP partners Adyen, Checkout.com, Stripe; fraud partners Forter, Riskified, Sardine, Signifyd. *(same)*
- **Amazon blocked Muse** (Sep) — retailer refusal is a live blocker. *(same)*

### Rails & credentials

- Analysis note: Wallet on network tokens (vs single-use VCNs merchants hate); no OpenAI commission at launch; Chase bespoke enrollment; Amex ACE first integration. *(2026-11-16 note)*
- **Stripe**: ACP + SPTs + Suite; VCN-style bootstrap still the near-term path in exec-summary framing. *(Stripe vs Shopify + exec summary)*
- **Visa Intelligent Commerce Connect** / **Mastercard Agent Connect**; Visa + BILL + Billtrust B2B invoice-agent pilot. *(2026-11-18 article + exec summary)*

### Platforms & merchants

- **Shopify** Agentic Storefronts / Catalog / Universal Cart / Checkout Kit. *(Stripe vs Shopify)*
- **Imprint** co-brand + MCP; **Squaremates** / **Affirm** 0% agent BNPL thesis. *(prior sources)*

### Trust, banks, data

- Intent verification as new auth; Muse as consumer proof point; volumes still tiny. *(exec summary)*
- **Plaid Agent Detection** + governed write path. *(2026-11-16 note)*

## Synthesis

1. **OpenAI chose merchant checkout over owning Instant Checkout** — aligns Wallet with retailer control and network tokens.
2. **Acceptance is the bottleneck:** bot/fraud infra and Amazon-style blocks matter as much as card rails; playbook + Web Bot Auth + fraud vendors are the unlock.
3. **Networks’ Connect products** and Wallet partners are converging on the same trust/integration layer Visa/Mastercard already claim.
4. **VCN vs tokens** remains the technical rivalry; Wallet is a public bet on the token side for consumer agents.

## Gaps / freshness

- No named retailers accepting Wallet yet in-corpus.
- Chase bilateral / Amex ACE coverage terms still thin.

*Ask in chat to add sources or say “refresh the brief” after new intakes.*
