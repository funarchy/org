# Problem-first work in public — prior art

Reference notes on who actually writes down the problem they are
solving, who publishes progress against it, and what the numbers
behind "users are bought, not earned" really are. Gathered
2026-08-08 to ground the two-minute pitch ([pitch.md](../pitch.md),
part of the solution to pollution #4). This is a **research note** —
part of the governance process as groundwork: solutions may cite it
as evidence (see
[03-amendment-process.md](../03-amendment-process.md), Step 2), but
it binds nothing on its own. If anything in this file disagrees with
the charter, the charter governs.

The question each entry is examined against: **who writes the
problem down, who commits to solving it, and who reports back
whether it got solved?** Those are three different acts, and the
prior art splits cleanly across them.

## The headline finding

"Nobody writes down the problem" is false — problem-first writing is
widespread and in places *enforced*. What holds instead:

1. **Problems are written by users asking, not by companies
   committing.** Trackers overflow with user-authored problems;
   no company examined publishes the problem *it* has committed to
   solve as a precondition of its own work.
2. **Public roadmaps are feature cards, not problems.** Unity,
   Unreal, Blender, Rive — all "Add X" with votes, none "X is
   broken and here is how we'll know it isn't."
3. **Progress is reported against features, never against the
   problem.** A "Shipped" checkmark, not "is the problem gone."
4. **No organization examined combines** problem-first public work,
   public finances, public decisions, forkability, and
   unsellability. Each piece is proven somewhere; the combination
   is unoccupied.

## Problem-first templates (enforced)

**Godot proposals.** Feature proposals to the Godot engine go
through a dedicated tracker whose template's first required field is
"Problem or limitation" — before "Proposed improvement". Verbatim
guidance: "Don't write your problem as 'I need flour', write 'I
want to bake a cake'. To add flour is the proposed solution." And:
"If you do not provide a well-founded motivation, your proposal will
be closed." Counts as of 2026-08-08 (GitHub API): 11,879 proposals
total — 6,411 open, 5,468 closed. This is the strongest single piece
of prior art for the pollution/solution distinction — and the
strongest evidence for finding 1: thousands of user-written problems
sitting open, with no reciprocal commitment.
Sources:
[feature_proposal.yml](https://github.com/godotengine/godot-proposals/blob/master/.github/ISSUE_TEMPLATE/feature_proposal.yml),
[godot-proposals README](https://github.com/godotengine/godot-proposals),
[announcement](https://godotengine.org/article/introducing-godot-proposals-repository/).

**GitHub's default feature-request template** opens with "Is your
feature request related to a problem? Please describe." — a GitHub
code search for that phrase returns ~85,760 files (approximate;
files, not distinct projects). Problem-first prompting is the
industry *default*, not the exception.

**RFC lineage.** The Rust RFC template: "Any changes to Rust should
focus on solving a problem that users of Rust are having," and calls
Motivation "one of the most important sections of any RFC." Bevy
(game engine) uses the same pattern.
Sources:
[Rust 0000-template.md](https://github.com/rust-lang/rfcs/blob/master/0000-template.md),
[bevyengine/rfcs](https://github.com/bevyengine/rfcs).

**Oxide Computer RFDs.** 500+ public "Requests for Discussion" in
under five years, covering technical design, hardware selection,
process, culture, and their interview system. The closest thing
found to a company writing everything down in public — but the
finances are not public (VC-funded) and RFDs are discussions, not
commitments with acceptance criteria.
Sources: [RFD 1](https://oxide.computer/blog/rfd-1-requests-for-discussion),
[rfd.shared.oxide.computer](https://rfd.shared.oxide.computer/rfd/0001).

**Basecamp / Shape Up.** The internal pitch format is: Problem,
Appetite, Solution, Rabbit holes, No-gos. "The best problem
definition consists of a single specific story that shows why the
status quo doesn't work." Internal-facing, but published as a book;
and Basecamp's own homepage states a problem in plain text ("most
project management systems are bloated, complicated, and
confusing"). Counter-evidence to any claim that landing pages never
name problems.
Sources: [Shape Up ch. 6](https://basecamp.com/shapeup/1.5-chapter-06),
[basecamp.com](https://basecamp.com/).

**GitLab.** The entire operating handbook is public, including a
product-development flow with a Validation track: work is expected
to start from a validated problem before the Build track. In
practice the public direction pages read as feature themes, not
problem commitments — the handbook prescribes problem-first; the
public-facing artifacts don't carry it through.
Sources: [handbook.gitlab.com](https://handbook.gitlab.com/),
[problem validation](https://handbook.gitlab.com/handbook/product/ux/experience-research/problem-validation-and-methods/).

## Public roadmaps (feature cards, not problems)

- **Unity**: [unity.com/roadmap](https://unity.com/roadmap) +
  Unity Pulse feedback community; cards are features with comments.
- **Unreal**: public Productboard portal
  ([roadmap](https://portal.productboard.com/epicgames/1-unreal-engine-public-roadmap/));
  community threads complain it is not a commitment device.
- **Blender**: [code.blender.org/roadmap](https://code.blender.org/roadmap/),
  per-module roadmap tasks, weekly meeting notes, public design
  tasks — the most transparent development process of the group,
  still organized by project/feature, not by problem.
- **Rive**: ran a Planned / In Progress / Completed board at
  feedback.rive.app/roadmap; that hostname no longer resolved as of
  2026-08-08. Landing page states no problem; leads with
  capabilities ("The Interactive experience engine") — but there is
  no paywall-before-trial either (free editor, downloads CTA).

## Open finances / open-startup prior art

- **Ghost** (non-profit foundation, UK): "Our legal constitution
  ensures that the company can never be bought or sold, and one
  hundred percent of our revenue is reinvested into the product and
  the community." Live public dashboard, 2026-08-08: ARR
  $11,055,673; MRR $921,306; net churn 2.92%; 30,557 customers;
  ~35 staff; MIT-licensed; no VC.
  Source: [ghost.org/about](https://ghost.org/about/).
- **Buffer**: public metrics dashboard, 2026-08-08: ARR $25.84M;
  MRR $2.15M; 79,075 customers; ARPU $27.23; LTV $453.83; churn
  5.82%; 238,532 MAU. Every employee's name, role, location, and
  salary published since 2013.
  Sources: [buffer.com/metrics](https://buffer.com/metrics),
  [buffer.com/open](https://buffer.com/open).
- **Plausible Analytics**: bootstrapped, no VC; $1M ARR in 2022,
  $3.1M ARR by 2024; public traffic stats and revenue write-ups.
  Source: [How we built a $1M ARR open source SaaS](https://plausible.io/blog/open-source-saas).
- **Open Collective**: platform for fully transparent budgets;
  Open Source Collective fiscally hosts 2,500+ projects.
  Source: [opencollective.com](https://opencollective.com/).

Ownership mechanics (Ghost, foundations, co-ops, steward-ownership)
are covered in [ownership-models.md](ownership-models.md); notable
here: Igalia (worker co-op, ~90–130 people, equal pay, consensus
assembly) writes nothing public about problems or finances —
co-op structure and public record are independent axes.

## Marketing economics ("users are bought")

"Thousands of dollars a head" is true only for enterprise B2B SaaS.
Verified 2025 benchmarks: SMB B2B SaaS CAC $200–$700; mid-market
$1,200–$2,000; long-cycle enterprise $1,000–$5,000+. Mobile games
are the opposite pole: ~$25B global UA spend in 2025, but median
CPIs in single dollars (hyper-casual ~$0.40 Android; tier-one
averages ~$4.22 iOS / $2.97 Android).

The robust formulation is the **ratio**: median $2 of sales &
marketing to acquire $1 of new ARR (Benchmarkit 2025), blended CAC
up 10% since 2022. From filings:

| Company | Period | Revenue | S&M | % of revenue |
|---|---|---|---|---|
| Asana | FY2025 (ended 2025-01-31) | $723.9M | $420.0M | 58% |
| monday.com | FY2025 | $1.23B | $586.8M | 48% |
| Unity | FY2024 | $1,813.3M | $752.6M | 41.5% |
| Atlassian | FY2024 | $4.35B | ~$877M | ~20% |
| Figma | FY2025 | $1,056M | $201.4M | 19.1% |

Sharpest single datapoint: Asana spent $420.0M on S&M in a year its
revenue grew $71.4M — $5.88 of marketing per $1 of new revenue —
with a $255.5M net loss. Counterpoint that supports the zero-ads
position: Figma (19.1%) and Atlassian (historically low-touch,
~20%) show low S&M is a winning strategy, not an ascetic one.
Sources:
[Asana Q4 FY2025 8-K Ex-99.1](https://www.sec.gov/Archives/edgar/data/1477720/000147772025000033/asana8-kex991q4fy25.htm),
[monday.com FY2025 results](https://ir.monday.com/news-and-events/news-releases/news-details/2026/monday-com-Announces-Fourth-Quarter-and-Fiscal-Year-2025-Results/default.aspx),
[Unity FY2024 results](https://investors.unity.com/news/news-details/2025/Unity-Reports-Fourth-Quarter-and-Fiscal-Year-2024-Financial-Results/default.aspx),
[Figma S-1](https://www.sec.gov/Archives/edgar/data/1579878/000162828025033742/figma-sx1.htm),
[B2B SaaS CAC benchmarks](https://www.poweredbysearch.com/learn/b2b-saas-cac-benchmarks/),
[mobile UA benchmarks](https://foxdata.com/en/blogs/2026-mobile-game-user-acquisition-cost-benchmarks-how-much-should-you-spend/).

## How the stories actually end

"The story always ends with the exit" is too kind. Observed endings:

- **The shutdown.** InVision: ~$350M raised, $2B peak valuation,
  revenue halved to $50M by 2022, Freehand sold to Miro in 2023,
  service shut down at the end of 2024. Nobody exited rich.
  Sources: [Fast Company](https://www.fastcompany.com/91006037/invision-former-ux-trailblazer-ending-services-figma-adobe),
  [techstartups.com](https://techstartups.com/2024/01/11/unicorn-startup-invision-once-valued-at-2-billion-shuts-down-after-burning-through-356-2-million-of-investors-money/).
- **The retroactive squeeze.** Unity Runtime Fee: announced
  September 2023 (per-install fee applied retroactively), developer
  revolt within a week, CEO John Riccitiello out in October 2023,
  fee fully cancelled September 2024 — replaced by seat-price
  increases. The gamedev-native proof of "own the environment,
  don't rent it by the seat": a company that owns the engine could
  change the terms under everyone at once.
  Source: [PC Gamer](https://www.pcgamer.com/gaming-industry/a-year-after-outraging-developers-blowing-up-its-reputation-and-saying-goodbye-to-its-ceo-unity-decides-runtime-fees-are-a-bad-idea-so-its-getting-rid-of-them/).
- **The blocked exit.** Adobe's $20B acquisition of Figma was
  abandoned under regulatory pressure (December 2023); Figma IPO'd
  in 2025 instead.

## To research

- Whether any company publishes acceptance criteria for its own
  work and reports against them (closest candidates: Oxide RFDs,
  Blender design tasks; neither closes the loop publicly).
- Wikimedia/Debian-style governance: problem-first at
  community-scale, but not companies selling a product.
- Where Rive's roadmap went (host unresolvable 2026-08-08) — moved
  or retired matters for citing it either way.
- Sleeping-giant counterexamples: Valve (no public anything,
  thrives), which caps how far "transparency wins" can be pushed as
  an empirical claim.
