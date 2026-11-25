---
id: klarna-app-and-open-payment-handler-architecture-2026-11-23
title: "Klarna Agentic Product Protocol + Open Payment Handler architecture"
date: 2026-11-23
added_at: 2026-11-23T09:06:00-05:00
source_type: note
topics:
  - agentic-commerce
  - payments
  - bnpl
  - discovery
  - protocols
  - orchestration
entities:
  - Klarna
  - Adyen
  - Stripe
  - Shopify
  - Google
  - Amazon
  - Facebook
  - Gr4vy
url: null
---

# Klarna direct merchant path for agentic commerce

**Yes. Klarna has a direct-to-merchant path for agentic commerce**, and it is developing two separate pieces of infrastructure:

1. **Agentic product discovery** – allowing AI agents to discover and compare a merchant's products directly.
2. **Agentic payments/checkout** – allowing AI agents to complete purchases using Klarna as the payment method.

Importantly, Klarna is not positioning this exclusively as a Stripe or Adyen capability. It has published infrastructure intended to be usable by merchants and other payment providers.

## 1. Direct merchant integration: Klarna Agentic Product Protocol

Klarna's Agentic Product Protocol (APP) provides a hosted API for merchants to expose their product catalogs to AI agents.

- Connect using existing Google Merchant, Shopify, Amazon, Facebook Catalog, CSV, or JSON feeds.
- Make products discoverable to participating AI agents.
- Expose standardized product information, pricing, and availability.
- Connect once rather than building individual integrations for each AI platform.

Klarna announced this in December 2025, with the specification and API available to merchants and developers.

## 2. Agentic payments: Klarna Open Payment Handler

On November 20, 2026, Klarna announced its integration with Adyen Agentic.

Key points:

- AI agents can present Klarna as a payment option.
- Consumers can select Pay in Full, interest-free installments, or financing.
- The consumer reviews and confirms the purchase.
- Merchants already accepting Klarna through Adyen can enable this without another integration.
- Adyen implemented this using Klarna's published **Open Payment Handler** specification.

Klarna explicitly says the specification allows any payment provider to add Klarna to AI agent checkout. Adyen is the first live implementation announced.

## 3. What does this mean for a merchant integrating directly with Klarna?

There are three potential integration paths:

| Path | Purpose |
| --- | --- |
| Klarna Agentic Product Protocol | Product discovery by AI agents |
| Klarna direct payment APIs | Merchant-owned Klarna payment integration |
| Klarna Open Payment Handler | Enable Klarna in agent-driven checkout through a payment provider |

Klarna already supports direct merchant payment integration through its APIs, including authorization, capture, refunds, and tokenization.

**One important distinction:** The direct product-discovery protocol and the open payment-handler specification are verified. Documentation confirming that Klarna currently offers merchants a complete standalone, direct-to-Klarna agent checkout implementation without a PSP or agent-platform integration has not been found.

## 4. Architectural view

```
AI Shopping Agent
  → Product discovery and purchase request

Merchant / Commerce Platform
  → Catalog, pricing, inventory, order management

Payment Orchestration
  → Agentic payment handler / PSP

Klarna
  → Customer approval, financing decision and payment authorization
```

Klarna is building both sides of agentic commerce, not just a new BNPL checkout button.

**Open question:** Will Klarna let an orchestration provider (e.g. Gr4vy) implement its Open Payment Handler directly, rather than requiring the merchant to use Adyen or Stripe — making Klarna available to multiple merchants and AI shopping agents through one integration?
