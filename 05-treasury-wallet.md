# Funarchy Treasury Wallet Setup

**Purpose:** Hold all Funarchy treasury funds (salary-split inflow, donations, revenue) with full public transparency.

---

## Evolution Path

| Phase | Wallet | Signers | Trigger |
|-------|--------|---------|---------|
| Founder-Led Phase | Single-signer stablecoin wallet | Founder | Launch |
| Partner joins | Gnosis-Safe-style 2-of-2 multi-sig | Founder + Partner | First joint governance act |
| Federated Phase | Multi-sig 2-of-3 / 2-of-4 | Founder + Partner + domain leads | Federated governance |

Single-signer at start is a pragmatic compromise: transparency comes from publishing every transaction monthly with on-chain links, not from signature count. The multi-sig upgrade is deliberately framed as the **first joint act** with the Partner - it makes shared control real on day one of the partnership.

---

## Setup (Founder-Led Phase)

1. Choose network: Ethereum mainnet or Polygon (Polygon recommended - cheaper gas)
2. Create the wallet (hardware wallet strongly recommended for the signing key)
3. Record the address here and in a public `treasury-address.md`
4. Test: send in and out a small amount (~$10 USDC), verify on the block explorer

**Treasury Address:** `[recorded at creation]`  
**Network:** `[Ethereum | Polygon]`

## Multi-Sig Upgrade (When the Partner Joins)

1. Deploy a Gnosis Safe with owners: Founder + Partner, threshold 2-of-2
2. Move treasury balance to the Safe (single transaction, published)
3. Update this document and `treasury-address.md`
4. From this point every outflow requires both signatures

## Adding Signers (Federated Phase)

1. Safe → Settings → Owners → Add Owner (domain lead's address)
2. Adjust threshold (e.g., 2-of-3, 2-of-4)
3. Existing signers approve the change on-chain
4. Update this document

---

## Transaction Flow

**Outflow (e.g., monthly salary):**
1. Initiator creates the transaction (recipient, amount, description)
2. Required signers approve in the Safe UI
3. Transaction executes; link recorded for the monthly report

**Cash-out (Serbia):**
- Exchange route (Kraken/Coinbase → fiat → bank): ~2% + legal clarity
- Local legal conversion: ~4%
- All conversion costs are personal, not treasury expenses

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
