# Funarchy Treasury Wallet Setup

**Purpose:** Hold all Funarchy treasury funds (salary-split inflow, donations, revenue) with full public transparency.

---

## Evolution Path

| Phase | Wallet | Signers | Trigger |
|-------|--------|---------|---------|
| Founder-Led Phase | Single-signer stablecoin wallet | Founder | Launch |
| Partner joins | Gnosis-Safe-style 2-of-2 multi-sig | Founder + Partner | First joint governance act |
| Federated Phase | Multi-sig 2-of-3 / 2-of-4 | Founder + Partner + stewards of carved domains (added as domains are carved) | Federated governance |

Single-signer at start is a pragmatic compromise: transparency comes from publishing every transaction monthly with on-chain links, not from signature count. The multi-sig upgrade is deliberately framed as the **first joint act** with the Partner - it makes shared control real on day one of the partnership.

One more honest fact: until a legal entity exists to hold the treasury, the funds are legally the Founder's personal property, whatever the reports call them. The reports state this rather than hide it (see the legal-form ladder in [02-roadmap.md](02-roadmap.md)).

---

## Setup (Founder-Led Phase)

1. Choose network. The deciding constraint is not gas price but which networks the cash-out rail accepts for deposits - a treasury on a chain the off-ramp won't take needs an extra hop every month. Polygon PoS is chosen because it is cheap, EVM-compatible (same wallets, Safe support), and accepted by the card route below.
2. Create the wallet (hardware wallet strongly recommended for the signing key)
3. Record the address here and in a public `treasury-address.md`
4. Test: send in and out a small amount (~$10 USDC), verify on the block explorer

Hold funds as **native USDC** (issued on Polygon by Circle), not the older bridged USDC.e - they are separate tokens with separate contract addresses, and services expecting one will not credit the other. Keep a few dollars of POL for gas; a stablecoin transfer costs well under a cent.

**Treasury Address:** `[recorded at creation]`  
**Network:** `Polygon PoS`

## Multi-Sig Upgrade (When the Partner Joins)

1. Deploy a Gnosis Safe with owners: Founder + Partner, threshold 2-of-2
2. Move treasury balance to the Safe (single transaction, published)
3. Update this document and `treasury-address.md`
4. From this point every outflow requires both signatures

## Adding Signers (Federated Phase)

1. Safe → Settings → Owners → Add Owner (domain steward's address)
2. Adjust threshold (e.g., 2-of-3, 2-of-4)
3. Existing signers approve the change on-chain
4. Update this document

---

## Transaction Flow

**Outflow (e.g., monthly salary):**
1. Initiator creates the transaction (recipient, amount, description)
2. Required signers approve in the Safe UI
3. Transaction executes; link recorded for the monthly report

**Spending (paying for hosting, agents, domains and similar):**

Most vendors Funarchy depends on do not accept stablecoins, so the treasury reaches them through a crypto debit card (currently Kolo, which accepts USDC deposits on Polygon PoS). The treasury tops the card up monthly with roughly one month of runway; the balance stays in the treasury wallet, not on the card. A card balance is the card provider's liability, not Funarchy's asset - keeping runway there and no more limits what a frozen account can cost.

Until a legal entity exists, the card is held personally by the Founder, for the same reason the treasury itself is legally personal property. This creates a real transparency gap: the top-up is public on-chain, but every purchase after it is invisible and mixed with personal spending. Two rules close it as far as it can be closed:

- Use a card dedicated to Funarchy spending, never one also used personally.
- Itemize every card purchase in the monthly report - vendor, date, amount, purpose - so the off-chain leg is at least stated, even though it cannot be independently verified. Reports say which figures are on-chain-verifiable and which rest on the Founder's word.

**Cash-out to fiat (Serbia):**
- Exchange route (licensed exchange → fiat → bank): ~2% + legal clarity
- Local legal conversion: ~4%
- All conversion costs are personal, not treasury expenses
- Banks supervised by the National Bank of Serbia cannot hold digital assets, so a licensed exchange is always the bridge; a business account on either rail requires a registered entity, which is a later step on the legal-form ladder in [02-roadmap.md](02-roadmap.md)

---

## Security Practices

- Private keys on hardware wallets; recovery phrases on paper in separate physical locations
- Never sign from a chat/email request - verify in the Safe UI directly
- Lost signer: remaining signers execute Remove Owner + Add Owner; update docs
- Signer personal addresses may stay pseudonymous; the treasury address is public

---

## Public Information

**Public:** treasury address, all transactions, monthly reports, signer roles (not necessarily identities)  
**Private:** private keys, recovery phrases, signers' personal wallet details
