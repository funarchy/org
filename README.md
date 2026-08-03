# Funarchy Governance

## Who is writing this

I'm [jkbo](https://github.com/jkb0o). I've been building software for
more than two decades - backend, game servers, frontend, gamedev, engine
internals (in the open: [belly](https://github.com/jkb0o/belly) and
[pecs](https://github.com/jkb0o/pecs) in the Bevy engine ecosystem,
among [sixty-odd repos](https://github.com/jkb0o?tab=repositories)) -
and for the last seven years as CTO at Funexpected, where I've built the
Funexpected Math product since its first commit in 2019.

## What this is about to be

**Funarchy** - a workers' cooperative that builds open-source tools for
people creating together: cooperative workflows, education, and
governance instruments for communities that want to decide their own
rules. The products are described in [products/](products/README.md);
the values are encoded - not decorated - in the [charter](01-charter.md):
openness, non-exploitation, sovereignty, permissionlessness, co-benefit.

The defining design decision: **founder power is built to dissolve.**
Governance moves from Founder-Led to Federated to Assembly on a stated
timeline with stated triggers, and the documents below are written so
that the organization outgrows its founder by design, not by accident.

## How these documents were made

Honestly: together with an agent, the way the products argue software
should be made. Every page here went through multiple iterations - 23
commits on this document set so far, and counting. The
[charter](01-charter.md) and the [products folder](products/README.md)
are reviewed line by line (including an adversarial multi-reviewer
pass); the bylaws, roadmap, and the rest are still in progress and read
accordingly. This repository is itself the first demonstration of the
workflow Funarchy exists to build.

## The open seat

I am looking for a **partner** - not an employee, not an investor, an
equal. **2-of-2 from the very beginning:** strategic decisions require
both of us, the treasury requires both keys, and if we disagree, the
change simply does not happen. Capital is not the ask; shared authority
and the operational half of the organization are. The partnership terms
are deliberately not pre-designed - co-writing them is the first joint
act (the full transition clause is in the [charter](01-charter.md)).

## Read this

Reviewed line by line - I stand behind every sentence, in this order:

| # | Document | What it is |
|---|----------|------------|
| 1 | [Charter](01-charter.md) | Our five core principles and how decisions get made. Everything downstream derives from this document. |
| 2 | [Products overview](products/README.md) | The agent-age manifesto, the four commitments, the stack, honest statuses. |
| 3 | [llm wiki](products/01-llm-wiki.md) | Curated, versioned knowledge agents navigate cheaply - and humans read too. |
| 4 | [Pollutions & Solutions](products/02-pollutions-n-solutions.md) | Problem-first cooperation for any real-world process. |
| 5 | [Funarchy Space](products/03-space.md) | Self-hosted, agent-native environment a team shares. |
| 6 | [RPPS](products/04-rpps.md) | Pollutions & Solutions running inside Space, enforced by tooling. |
| 7 | [PMS](products/05-pms.md) | Architecture that makes agent iteration token-cheap and collision-free. |
| 8 | [scenepad](products/06-scenepad.md) | PMS in TypeScript - Space becomes a general-purpose app engine. |
| 9 | [Type Space](products/07-type-space.md) | A keyboard-mastery game growing into a cooperative creativity tool. |

## Read at your own risk

Drafted, iterated with the agent, but not yet reviewed with the same
care - expect these to change:

| Document | What it is |
|----------|------------|
| [Bylaws](02-bylaws.md) | The legal encoding of the charter, drafted for filing as a Serbian zadruga (workers' cooperative). |
| [Roadmap](03-roadmap.md) | How governance evolves: founder-led → federated domains → community assembly, with dates and success criteria. |
| [Amendment Process](04-amendment-process.md) | How anyone proposes a change to the charter, bylaws, or roadmap - and how it gets decided and filed. |
| [Treasury Wallet](05-treasury-wallet.md) | How the money is held and who can move it, from single-signer through federated multi-sig. |
| [Onboarding Guide](06-onboarding-guide.md) | A new cooperator's first month. |

**Living records** (unnumbered - appended to, not read in sequence):

- [`tooling.md`](tooling.md) - the registry binding tool-neutral terms ("public forum", "public record") to current tools; swapping a tool changes one line here, not the charter
- `treasury-reports/` - monthly public financial reports
- `amendment-log.md` - history of approved changes with rationale *(created with the first amendment)*
- `decisions.md` - Founder-Led Phase decision log: what was decided, why *(created at launch)*
- `treasury-address.md` - the public wallet address *(created at wallet setup)*

## Precedence

If two documents disagree, the **charter** governs. The bylaws are its legal expression; the roadmap is its timeline. Where the filed Serbian bylaws and this repository diverge in wording, the filed document is legally binding and this repository is the working source of truth between filings.

The five core principles in the charter are the one thing that cannot be amended. A Funarchy that wants different values should fork rather than amend.

## Proposing a change

Funarchy works problem-first: report a **pollution** (the problem, described as a problem), then anyone may propose a **solution** (the exact new text). Full pipeline: [04-amendment-process.md](04-amendment-process.md). Anyone may report or propose - you do not need to be a member.
