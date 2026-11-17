# State of Agentic Commerce

**Brief updated:** 2026-11-16  
**Corpus coverage through:** 2026-11-16  
**Sources:**  
- [`sources/stripe vs shopify agentic.md`](../sources/stripe%20vs%20shopify%20agentic.md)  
- [`sources/2026-11-16-openai-wallet-plaid-imprint.md`](../sources/2026-11-16-openai-wallet-plaid-imprint.md)  
- [`sources/11.14.26.md`](../sources/11.14.26.md)  
- [`sources/11.10.26 udpate - Executive Summary.md`](../sources/11.10.26%20udpate%20-%20Executive%20Summary.md)

## Snapshot

Agentic commerce is **real but tiny in GMV**. The fight is over **trust / intent / liability**, **who owns the consumer interface vs the payment rail**, and whether checkout bootstraps on **virtual cards (Stripe-like)** or **network tokens (Visa/Mastercard / ChatGPT Wallet)**. Platforms (Shopify) and brand wallets (Imprint) are racing on **merchant discoverability and relationship control**.

## From sources

### Early proof points & volume

- Industry consensus (Nov 10 update): heavy investment, **negligible volume** today (e.g. Uber ~500 AI Uber Eats / 4 ride txs in a major week). *(exec summary 2026-11-10)*
- **Meta Muse** is the breakout consumer signal: 10M US/CA users, #1 App Store, ~25% DAU, shopping-led, avg basket >$200; Plaid/Stripe seeing elevated connector/txn activity. *(same)*

### Rails & credentials

- **ChatGPT Wallet**: network tokens end-to-end, biometric per-purchase approval, Chase bespoke enrollment; no OpenAI commission at launch; Amex ACE first integration. *(2026-11-16 note)*
- **Stripe**: ACP (+ OpenAI), **Shared Payment Tokens**, Agentic Commerce Suite, Agent Toolkit, Link for agents — payments/protocol rail across stacks. *(Stripe vs Shopify)*
- **Virtual cards:** Stripe-like one-time VCNs are the **near-term bootstrap** (works on existing merchant acceptance); Mastercard frames VCNs as a temporary bridge and prefers fully tokenized network-native flows. Forecast in exec summary: VCN ~2026–2028, network tokens for scale/risk ~2028–2032. *(exec summary)*
- **Visa / Mastercard**: VIC / Agent Pay + agent directories, verifiable intent, agent tokens; Visa ~50 AI partners in production. *(exec summary + CRC 11.14)*

### Platforms & merchants

- **Shopify**: Agentic Storefronts, Catalog, Universal Cart, Checkout Kit — keep branded checkout/attribution; Magics/Sidekick for merchant ops; AI-referred conversion reportedly +64%. *(Stripe vs Shopify + exec summary)*
- **Imprint**: co-brand + MCP so brand credentials stay in the agent wallet. *(2026-11-16 note)*
- **Squaremates / Affirm**: seller agents + agents picking 0% BNPL. *(CRC 11.14)*

### Trust, banks, data

- Intent verification rising as the new auth question (“did the agent buy what was authorized?”). *(exec summary)*
- **Plaid Agent Detection** + path to governed agent write access. *(2026-11-16 note)*
- Banks (e.g. BofA) still push human-in-the-loop; big-tech agents push autonomy. *(exec summary)*

## Synthesis

1. **Interface vs rail:** Muse/ChatGPT win attention first; networks/PSPs fight to own trust metadata on the payment.
2. **VCN now, tokens later:** Named virtual-card path is the **Stripe-style intermediary VCN**; ChatGPT Wallet / network Agent Pay are the token alternative merchants and networks prefer long-term.
3. **Shopify vs Stripe:** complementary more than identical — Stripe = open protocol + pay; Shopify = merchant discovery + controlled checkout.
4. **Trust stack is the product:** identity, delegated authority, intent, liability — ahead of GMV.

## Gaps / freshness

- Primary filings / exact product docs for ACP, VIC, Muse metrics not in-corpus beyond these notes.
- Chase–OpenAI bilateral terms and Amex ACE coverage details still inferred.

*Ask in chat to add sources or say “refresh the brief” after new intakes.*
