# Funarchy Charter

**Adopted:** [September 2026]  
**Status:** Open governance document - anyone can report a pollution or propose an amendment (see [03-amendment-process.md](03-amendment-process.md))

---

## Preamble

Funarchy is a cooperative of people building open-source solutions for productive workflows, education, and anarchist digital governance. We believe technology can encode our values - transparency, mutual aid, and freedom from exploitation - instead of encoding the values of platforms and corporations.

This charter is our promise to each other: who we are, what we stand for, and how we decide together.

---

## Five Core Principles

### 1. Openness

**Commitment:** All decisions, source code, and finances are public by default.

**What this means:**
- All code is open-source (GPL, MIT, or similar licenses)
- Strategic decisions are made in public (the public forum, open meetings - see [tooling.md](tooling.md))
- Monthly financial reports are published and auditable on-chain
- Documentation and learning materials are freely available
- No closed-door decisions; no "leadership only" information

**Why:** Transparency prevents corruption and abuse. It allows others to learn from, fork, and improve our work.

### 2. Non-Exploitation

**Commitment:** No member becomes wealthy from the labor of others. Benefits are shared equitably.

**What this means:**
- Members receive fair compensation for their labor (comparable to or above market rates)
- Surplus is never accumulated or paid out as dividends; it's reinvested in the mission
- Decision-making power is not tied to wealth or investment size
- The Founder's role does not confer permanent authority; power is progressively delegated
- No member can claim ownership of the cooperative's work

**Why:** Exploitation corrupts movements. Equitable compensation and shared ownership align individual and collective interests.

### 3. Sovereignty

**Commitment:** No single funder, person, or entity controls Funarchy's direction. Governance is community-based.

**What this means:**
- No supporter's contribution buys strategic control - advisers and funders advise, members decide
- Major decisions are made by members/cooperators, not investors
- Funding is deliberately diversified (donations, grants, SaaS, consulting) to prevent dependency
- New members have voting rights equal to founders
- If Funarchy ever becomes large, decision-making is decentralized to regional or domain-based teams

**Why:** Sovereignty ensures our values are our own, not borrowed from funders or boards of trustees.

### 4. Permissionlessness

**Commitment:** All work produced by Funarchy can be freely used, modified, and built upon by anyone.

**What this means:**
- All code is open-source with permissive or copyleft licenses
- All educational materials are open and remixable (CC-BY-SA or similar)
- Anyone can fork Funarchy's projects and create alternatives without permission
- We provide no vendor lock-in; users are never trapped in our platform
- We welcome forks and derivatives; we celebrate when others build on our work

**Why:** Permissionlessness prevents technology from becoming a tool of control. It lets anyone build on our work - including people we will never meet.

### 5. Co-Benefit

**Commitment:** All work serves both Funarchy's mission and the wider world of cooperatives, open-source projects, and self-organized communities.

**What this means:**
- We don't build products for profit; we build tools people can simply take and use - a kid learning math, a teenager writing their first program, a team organizing work without a boss, a community deciding its own rules
- Decisions consider impact on communities and allied organizations
- We share knowledge, not just code (documentation, case studies, lessons learned)
- We support other cooperative and open-source projects (mentorship, code review, grants)
- Success is measured in how many people our tools reach and help, not market share

**Why:** Co-benefit creates resilience. Our work survives and spreads because many hands carry it, not one company.

---

## How Change Happens: Pollutions and Solutions

Funarchy works problem-first. A **pollution** is a problem described as a
problem - a harm, a friction, an unclearance - never a prescribed fix. A
**solution** is a concrete proposal that answers one or more pollutions.
Anyone can report a pollution; anyone can propose a solution; only the
final decision depends on the governance phase below. This split is itself
an anarchist mechanism: describing problems requires no authority, so
power over "what hurts" belongs to everyone from day one, in every phase.

Not everything is a pollution. **Changing a rule** (charter, bylaws,
roadmap, a standing process) goes through a pollution and lands as a
solution - full pipeline in [03-amendment-process.md](03-amendment-process.md).
**Applying a rule** to a case (admitting a member, approving a budget,
executing a treasury transaction) is a decision under the phase rules
below, recorded in `decisions.md`.

Discussion happens in the public forum; outcomes land in the public
record - the repository, which anyone can clone, fork, and mirror. The
current tool bindings live in [tooling.md](tooling.md) and are themselves
swappable: Funarchy's governance must never depend on any single platform's
goodwill.

---

## Decision-Making by Phase

### Founder-Led Phase (Sep 2026 – until the second domain is carved)

**Who decides?** The Founder, with input from the Founding Adviser, the community, and - once joined - the Partner.

**How:**
1. Anyone (including the Founder) reports a pollution or proposes a solution in the public forum
2. The community discusses - window per [03-amendment-process.md](03-amendment-process.md) Step 3
3. The Founder decides, recording rationale in `decisions.md`
4. If community strongly disagrees, escalate to mediation by the Founding Adviser (and the Partner, once joined)

**Scope:** Strategic direction, new projects, budget allocation, member admission.

**This phase begins solo.** The Partner seat is open and is filled by
recognition, not recruitment - like every role in Funarchy, it names
responsibility already held: sustained, real operations work done
alongside the Founder, by someone the Founder accepts as an equal
counterweight. The work does not wait for the seat to fill; until the
Partner joins, the Founder decides alone and the treasury runs
single-signer with every transaction published (see
[04-treasury-wallet.md](04-treasury-wallet.md)). The Partner joining
is an event within this phase, not a phase of its own.

**When the Partner joins:** the Founder and the Partner govern as
co-founders. From that day, wherever these documents say "the Founder,"
read "the Founders, jointly" - strategic decisions require both, the
treasury requires both keys (the 2-of-2 multi-sig upgrade is the same
event), and disagreement means the change doesn't happen: status quo
holds, then mediation. Day-to-day, each stewards their own half - the Founder
technology, the Partner operations: the two **founding domains**, the
first, coarse version of Funarchy's domain map. **The detailed partnership terms are
co-written with the Partner as one of the first joint acts - this seat is
not pre-designed; its occupant designs it.**

**This phase is intentionally founder-led because:**
- Speed matters (we're registering and launching fast)
- Early-stage decisions are foundational; they're hard to reverse
- Small group reduces coordination overhead while building trust

### Federated Phase (begins when the second domain is carved; estimated 2027)

**Who decides?** Stewards of carved domains + the Founder.

**Domains are carved, not pre-designed.** Funarchy always has a domain map; it starts coarse - technology (the Founder) and operations (the Partner), the founding domains. A new domain is carved from that map by the people doing real work in it, through the same pollution → solution pipeline as any other governance change. A carve proposal must show three things: sustained real work already happening in the area, more than one person doing it, and someone already taking and holding responsibility for the area, whom the others accept. That person becomes the domain's **steward** - stewardship is recognition of responsibility already held; the work exists first, the role names it. No numeric thresholds - it is judged at the decision step, case by case. The approving amendment defines the domain's scope, its steward, and how the steward is replaced, and is recorded in `amendment-log.md`. The first carved domain is delegation - still the Founder-Led Phase. This phase begins at the second, because federation means more than one steward: only then does "stewards reach consensus" mean anything. The switch is the event, not the calendar. If this feels abstract, [06-carved-domains.md](06-carved-domains.md) walks through worked examples - two carves that pass the test, and one that fails it.

**How:**
1. Pollutions and solutions flow exactly as before - the mechanics never change between phases
2. Domain-internal decisions: the steward decides, with team input
3. Cross-domain decisions: stewards reach consensus (the Founder breaks ties if needed)
4. Strategic decisions: same as the Founder-Led Phase, but stewards decide instead of the Founder alone

**Scope:** Each carved domain is semi-autonomous; decisions affecting multiple domains or the whole cooperative need consensus.

**This phase decentralizes because:**
- Organization is larger; founder-led bottlenecks emerge
- Domain experts are better suited to make decisions in their area
- Community trust is established; safer to delegate

### Assembly Phase (18+ months)

**Who decides?** Community assembly (all members + invited contributors).

**How:**
1. Pollution → solution → discussion (the same window, async) - the same pipeline, now with an assembly at the decision step
2. Assembly vote (monthly or quarterly)
3. Voting mechanism: Quadratic voting, delegated voting, or consensus (to be designed in the Federated Phase)
4. Major decisions require 70%+ support

**Scope:** Strategic direction, charter amendments, budget, new projects, member admission.

**This phase achieves the anarchist goal because:**
- Power is genuinely distributed
- No single person (including the Founder) can unilaterally decide
- Decisions are made by those doing the work

---

## Values in Practice

### How We Hire & Build Community

- We look for people aligned with the five principles, not just technical skill
- We hire for diversity of experience and perspective (not homogeneity)
- We pay fairly and transparently
- We invest in onboarding and mentorship (not just task assignment)
- We celebrate people who help others grow

### How Roles Are Held

- Responsibility over leadership: roles are earned by proactively taking and holding responsibility, never granted to those who seek position
- A steward is recognized after the fact - the work exists first, the role names it
- Every role is revocable; how it is replaced is defined when the role is created

### How We Make Decisions

- We start from problems, not prescriptions - pollutions name what hurts; solutions compete to answer them
- We prefer consensus over voting, but vote if consensus stalls
- We document our decisions (why we chose X over Y) so future members can understand our thinking
- We regularly revisit decisions; nothing is final
- We are willing to fail and learn together

### How We Handle Disagreement

- We listen carefully to dissenting voices
- We assume good intent; we don't tolerate bad-faith attacks
- We use mediation before escalation
- If someone fundamentally disagrees with our five principles, they should fork and build their own thing - we respect that

### How We Relate to Other Movements

- We are part of the cooperative economy, open-source software, and anarchist organizing
- We learn from and support other projects in these movements
- We are not dogmatic; we learn from projects with different values
- We celebrate forks and derivatives of our work

---

## Amending This Charter

This charter is alive. It changes as we learn and grow.

**To propose an amendment:**
1. Report the pollution - what hurts, who it affects, cost of not fixing, acceptance criteria
2. Propose the solution - the exact new text, answering the pollution
3. Discussion window: per [03-amendment-process.md](03-amendment-process.md) Step 3 - it closes on silence, not on a fixed date, and the durations live there so they cannot drift
4. Decision: the Founder (Founder-Led Phase), steward consensus (Federated Phase), or assembly vote (Assembly Phase)
5. If approved, the solution lands in this document and is recorded in `amendment-log.md`

Full pipeline: [03-amendment-process.md](03-amendment-process.md).

**What cannot change:** The five core principles are non-negotiable. If a future Funarchy wants different values, they should fork.

---

## How This Document Relates to Bylaws

- **Charter** = our values and promises to each other (this document)
- **Bylaws** = the legal rules filed with the Serbian government (`07-bylaws.md`)
- Both must align; if they diverge, the charter guides updates to the bylaws

---

## Signatures of Founding Members

**jkbo** - Founder & Primary Coordinator (Founder-Led Phase)  
**Date:** [September 2026]

**Partner** - position open (equal operational partner & governance counterweight)  

**Founding Adviser** - informal advisory role, outside the regulated flow

---

## Amendment Log

[Maintained in `amendment-log.md`]
