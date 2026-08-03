# Funarchy Products

Seven products - two in production, five taking shape - one story: tools
for people creating together in the age of agents.

---

## The claim

Humanity is entering a new age of product creation - creation with the
help of agents. This is not a feature added to the old way of working; it
is a different way of working. And everything we build with - our
libraries, our patterns, our workflows - was invented before agents
existed and was never designed for them. It all has to be rethought, not
retrofitted.

Nobody rethinks it neutrally. Agent providers profit from token usage, so
the tooling they push will drift - not by conspiracy, by incentive -
toward workflows that burn more tokens: regenerate instead of reuse,
re-derive instead of remember, prompt harder instead of design better.
The defaults will not be on your side.

## Four commitments

Every Funarchy product is designed around four commitments, in this order:

1. **Cooperation first.** Our products are built for people creating
   *together* - not for turning one person into a one-person orchestra.
   Every person carries their own domain knowledge, talents, skills, and
   vision; tools should let those strengths combine, not replace them with
   one operator conducting a fleet of agents. Most agent tooling today
   sells the opposite: the lonelier you work, the better it sells. We
   refuse the premise. Our products are built *around* cooperation - it is
   the center they orbit, not a feature they integrate.
2. **Maximum usefulness.** Tools that solve real problems for real teams,
   measured by reach and help, not engagement.
3. **Token-spend effectiveness.** Architecture and knowledge design that
   make every agent interaction cheap: curated context instead of
   re-derivation, small regenerable units instead of whole-codebase
   prompting. We will publish token-spend measurements from real
   production use as the products open-source - this commitment is
   checkable, and should be checked.
4. **Minimum vendor lock-in.** Self-hosted, plain-text, model-agnostic,
   forkable. If any provider - including an agent provider - turns
   hostile, you can leave and keep everything: your data, your tools,
   your workflows.

## The stack

Each product stands alone; together they form a stack, and each layer
proves the one below it. The first four layers are proven by daily
production use at Funexpected today; scenepad will prove PMS, and Type
Space will prove the whole stack.

The file numbers are the reading order: each page assumes you have read
the pages it depends on, and every dependency has a smaller number.

| Layer | Product | In one line |
|---|---|---|
| Knowledge | [llm wiki](01-llm-wiki.md) | curated, versioned knowledge that agents navigate cheaply and humans read too |
| Method | [Pollutions & Solutions](02-pollutions-n-solutions.md) | problem-first cooperation for any real-world process |
| Place | [Funarchy Space](03-space.md) | self-hosted, agent-native environment a team shares |
| Flow | [RPPS](04-rpps.md) | Pollutions & Solutions running inside Space, enforced by tooling |
| Pattern | [PMS](05-pms.md) | architecture that makes agent iteration token-cheap and collision-free |
| Engine | [scenepad](06-scenepad.md) | PMS in TypeScript - Space becomes a general-purpose app engine |
| Proof | [Type Space](07-type-space.md) | a keyboard-mastery game growing into a cooperative creativity tool, built on all of the above |

**On the name "Space":** it is a deliberate family name. A Space is a
place people enter to work, learn, or create *together*. Funarchy Space
is the first; Type Space is the second; there may be more.

## Status

Honesty over polish - here is exactly what exists today:

| Product | Status today | Open-source target |
|---|---|---|
| llm wiki | in production at Funexpected; open-sourcing pending agreement with current maintainers, otherwise rewritten from scratch | Q4 2026 |
| Pollutions & Solutions | practiced daily in Funexpected's development; general write-up pending | Sep 2026 |
| Funarchy Space | in daily production use at Funexpected (internal tool); rename + extraction underway | Sep-Oct 2026 |
| RPPS | in production as Space's workflow layer; renamed on open-sourcing | Oct 2026 |
| PMS | specification written; reference implementation in progress | Q4 2026 |
| scenepad | extraction into a standalone monorepo started | Q4 2026 - Q1 2027 |
| Type Space | concept; design starts after Funarchy launch; the first product born inside Funarchy | prototype 2027 |

**On intellectual property, plainly:** Space, RPPS, scenepad, and the
Pollutions & Solutions practice were built by the Funarchy founder inside
Funexpected, whose founder has agreed in principle that this work
open-sources on the author's terms. The llm wiki is the exception - it
has other maintainers, and open-sourcing it awaits their agreement; if
that does not come, it will be rewritten from scratch, which is why its
date carries more risk than the others.

## How this funds the cooperative

These products are free and open-source, forever - that is the
[Permissionlessness principle](../01-charter.md). The
cooperative earns from hosting Space for teams that prefer one click to
self-managing, and from integration consulting. The founder's baseline
salary is already covered by an existing salary-split arrangement, so
the organization starts near break-even rather than on a burn-down
runway; hosting and consulting fund growth. Full financial model with
numbers: [governance docs](../README.md).
