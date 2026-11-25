# Competing Protocols in Agentic Commerce

**Brief updated:** 2026-11-24  
**Based on corpus through:** 2026-11-24  
**Sources:** prior protocol brief sources + Klarna notes + DC360 Nov 2026 agentic retail report

The “protocol wars” aren’t one race — they’re overlapping stacks competing for different jobs.

## 1. Commerce / agent interaction layer

| Protocol | Backers (in corpus) | Job |
| --- | --- | --- |
| **ACP (Agentic Commerce Protocol)** | Stripe + OpenAI | Product data, cart, programmatic purchase (incl. Instant Checkout); SPTs for scoped pay credentials |
| **UCP (Universal Commerce Protocol)** | Google + Walmart/Wayfair/Etsy/Shopify/Target (+ Newegg, Gap, Macy’s…) | Common commerce language into Google AI shopping; merchant-of-record preserved; catalog + checkout path |
| **PAP (Personal Agent Protocol)** | Meta, Shopify, Stripe, Walmart, Synchrony | Secure agent-to-agent, permissions, trust framework |
| **Shopify Agentic Storefronts** | Shopify (platform, not open protocol) | Catalog syndication to ChatGPT/Perplexity + merchant checkout control |
| **Klarna Agentic Product Protocol (APP)** | Klarna | Hosted catalog API for AI agents; ingest Google/Shopify/Amazon/Facebook/CSV/JSON feeds; connect-once multi-agent discovery |

**Read:** ACP is the clearest *named* open checkout protocol. UCP/PAP look like competing/overlapping “how agents talk commerce & trust” standards. Shopify’s stack often *uses* ACP via Stripe rather than fully replacing it. **Klarna APP** is a BNPL-led catalog syndication path — inventory/discovery without requiring Adyen/Stripe.

## 2. Network trust / payment-authorization layer

| Protocol / platform | Who | Job |
| --- | --- | --- |
| **Visa Intelligent Commerce (VIC)** + **Trusted Agent Protocol** | Visa | Agent identity, directory, agent tokens, intent |
| **Mastercard Agent Pay / Agent Connect** | Mastercard | Tokenized agent pay, verifiable intent, trust intelligence |
| **Amex ACE** | Amex | Registered agents + Agent Purchase Protection / intent |

**Read:** Visa vs Mastercard (and Amex’s closed ACE path) compete to be the **trust rail** — who verifies the agent and attaches intent to the payment. Chase resisting VIC while doing a ChatGPT bilateral is that fight in practice.

## 3. Credential / payment-method model

- **Stripe-style one-time virtual cards (VCNs)** — bootstrap: works on today’s merchants
- **Network tokens** (Agent Pay / ChatGPT Wallet / VIC-style) — networks’ preferred long-term model with agent/intent metadata
- **Klarna Open Payment Handler** — published spec so any PSP can plug Klarna into AI agent checkout; **Adyen Agentic** first live (Nov 20 2026); not Adyen-exclusive by design
- Split from **Klarna APP** (discovery): pay handler ≠ catalog; merchants with independent Klarna can use APP for inventory exposure, but agent-native Klarna pay may still need a handler implementer (PSP/orchestrator) until a confirmed standalone Klarna agent checkout exists

Mastercard frames VCNs as a temporary bridge. Klarna’s stack is a parallel fight on **two layers**: catalog syndication (APP vs Shopify/ChatGPT feeds) and **non-card agent pay** (Open Payment Handler vs card-only Wallet).

## 4. Soft-benefit / brand knowledge layer

- **Shopify Knowledge Base** — merchants control what agents say about their brand (early soft-benefit legibility)
- Thesis: without machine-readable soft benefits, agents optimize price/availability/speed → Amazon/Walmart (and Chase-scale FS) win by default
- Financial services still lacks a clear soft-benefit equivalent in-corpus

## 5. Enterprise inter-agent / security protocols (adjacent)

McKinsey lists these as **under development / not fully mature** for securing agent-to-agent collaboration:

| Protocol | Who |
| --- | --- |
| **Model Context Protocol (MCP)** | Anthropic |
| **Agent Connect Protocol** | Cisco (not Mastercard Agent Connect) |
| **Agent2Agent (A2A)** | Google |
| **Agent Communication Protocol** | IBM |

Enterprise controls that pair with them: IAM for agents as principals, authenticated/logged inter-agent comms, I/O guardrails, full behavioral traceability, sandboxes/kill switches.

## 6. Adjacent, not the same fight

- **MCP / WebMCP (Imprint, Square, OpenAI playbook)** — also used as merchant/agent tooling for rewards/ops/cart actions
- **Plaid Agent Detection / permissioned write** — bank-data gatekeeping for agentic finance

## Synthesis

The sharpest **commerce** competitions are **ACP (+ SPTs/VCNs) vs network token suites (VIC / Agent Pay / ACE)** on payments/trust, and **PAP / UCP / ACP / Shopify channels** on discovery/checkout. Separately, enterprise **A2A security protocols** (MCP / Cisco ACP / Google A2A / IBM ACP) are immature but name the same underlying problem: authenticated, auditable agent identity and action — which is why synthetic-agent-identity risk in McKinsey maps to Trusted Agent / directory debates in payments.
