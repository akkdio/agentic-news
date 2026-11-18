# Competing Protocols in Agentic Commerce

**Brief updated:** 2026-11-16  
**Based on corpus through:** 2026-11-16  
**Sources:** exec summary (`sources/11.10.26 udpate - Executive Summary.md`), Stripe vs Shopify note, OpenAI/Plaid/Imprint note, CRC digest (`sources/11.14.26.md`)

The “protocol wars” aren’t one race — they’re overlapping stacks competing for different jobs.

## 1. Commerce / agent interaction layer

| Protocol | Backers (in corpus) | Job |
| --- | --- | --- |
| **ACP (Agentic Commerce Protocol)** | Stripe + OpenAI | Product data, cart, programmatic purchase (incl. Instant Checkout); SPTs for scoped pay credentials |
| **UCP (Universal Commerce Protocol)** | Shopify + ecosystem | Common language for commerce interactions across agents |
| **PAP (Personal Agent Protocol)** | Meta, Shopify, Stripe, Walmart, Synchrony | Secure agent-to-agent, permissions, trust framework |
| **Shopify Agentic Storefronts** | Shopify (platform, not open protocol) | Catalog syndication to ChatGPT/Perplexity + merchant checkout control |

**Read:** ACP is the clearest *named* open checkout protocol. UCP/PAP look like competing/overlapping “how agents talk commerce & trust” standards. Shopify’s stack often *uses* ACP via Stripe rather than fully replacing it.

## 2. Network trust / payment-authorization layer

| Protocol / platform | Who | Job |
| --- | --- | --- |
| **Visa Intelligent Commerce (VIC)** + **Trusted Agent Protocol** | Visa | Agent identity, directory, agent tokens, intent |
| **Mastercard Agent Pay / Agent Connect** | Mastercard | Tokenized agent pay, verifiable intent, trust intelligence |
| **Amex ACE** | Amex | Registered agents + Agent Purchase Protection / intent |

**Read:** Visa vs Mastercard (and Amex’s closed ACE path) compete to be the **trust rail** — who verifies the agent and attaches intent to the payment. Chase resisting VIC while doing a ChatGPT bilateral is that fight in practice.

## 3. Credential model (not a protocol name, but the real technical rivalry)

- **Stripe-style one-time virtual cards (VCNs)** — bootstrap: works on today’s merchants
- **Network tokens** (Agent Pay / ChatGPT Wallet / VIC-style) — networks’ preferred long-term model with agent/intent metadata

Mastercard explicitly frames VCNs as a temporary bridge; the exec summary casts this as **Stripe bootstrap vs network token endgame**.

## 4. Adjacent, not the same fight

- **MCP (Imprint, Square)** — agent tooling/API surface for rewards/ops, not a card-network protocol
- **Plaid Agent Detection / permissioned write** — bank-data gatekeeping for agentic finance

## Synthesis

The sharpest competitions are **ACP (+ SPTs/VCNs) vs network token suites (VIC / Agent Pay / ACE)** on payments/trust, and **PAP / UCP / ACP / Shopify channels** on how agents discover and transact with merchants. Same industry, different layers — winners can coexist if discovery stays relatively open and payment authorization stays closed/curated.
