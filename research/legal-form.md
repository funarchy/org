# Legal form — Serbian options for an unowned entity

Reference notes on the legal forms available to Funarchy in Serbia,
examined against one requirement: **no one can ever extract value
from Funarchy except as pay for work.** This is a **research note** —
part of the governance process as groundwork: solutions may cite it
as evidence (see [03-amendment-process.md](../03-amendment-process.md),
Step 2), but it binds nothing on its own. If anything here disagrees
with the charter, the charter governs.

Companion note: [ownership-models.md](ownership-models.md) examines
who holds the residual claim at Proton and others. This note asks the
narrower question of which Serbian legal instrument delivers that
answer.

**Nothing here is legal or tax advice.** Every figure is dated and
sourced; rates change annually and the qualitative tests below are
decided case by case. Confirm with Serbian counsel and an accountant
before filing anything.

## The vocabulary problem

"Non-profit" is ambiguous and the ambiguity caused a real error. Two
distinct things travel under the name:

- **A non-profit legal form** — a charity, a 501(c)(3), an e.V., a
  Serbian `udruženje` or `fondacija`. Defined by the
  non-distribution constraint: surplus can never be paid to members
  or owners, only spent on the stated mission.
- **A non-distributing commercial entity** — an ordinary trading
  company whose constitution forbids anyone from taking profit out.

Ghost is the second, not the first. Funarchy wants the constraint,
not the charity status. The precise word is **non-distributing**.

A Serbian `zadruga` is neither: it is a member-owned commercial
entity whose assembly decides on distributing annual profit.

## Prior art: how the projects Funarchy resembles are held

| Project | Form | Jurisdiction | Owners |
|---|---|---|---|
| Ghost | Company limited by guarantee | Singapore | none |
| Godot | `Stichting` (foundation) | Netherlands | none |
| Blender | `Stichting` + trading BV | Netherlands | none |
| Proton | For-profit AG under a foundation | Switzerland | foundation + employees |

Ghost Foundation Limited (UEN 201605007D, incorporated 2016-02-29) is
a public company limited by guarantee — no share capital, no
shareholders. Its constitution provides that it cannot be bought or
sold and that profit is reinvested. It trades commercially at
multi-million-dollar scale and pays salaries. The founders own
nothing.

A Singapore CLG is a *form* charities commonly use; Ghost is not a
registered charity. This is the clearest available demonstration that
"non-distributing" and "commercial" are compatible.

## Serbian legal forms compared

| | `Zadruga` | `Udruženje` | `Fondacija` | `Zadužbina` |
|---|---|---|---|---|
| Members? | yes, own it | yes | **no members** | no members |
| Min. founders | 5 natural persons | 3 | 1 | 1 |
| Min. assets | — | — | none stated in law | €30,000 |
| Non-distribution | **no** — assembly votes on profit | yes | yes | yes |
| Commercial activity | unlimited | "manjeg obima" | "sporedna delatnost" | "sporedna delatnost" |
| Public-benefit purpose required | no | no | **yes** | optional |

### `Fondacija` — the closest instrument

The Law on Endowments and Foundations defines a `fondacija` as a
*"pravno lice bez članova i osnovne imovine"* — a legal person
**without members and without basic assets** — established for the
charitable pursuit of a public-benefit goal. That is structurally
what Ghost achieved by constitution, available directly in Serbian
law.

- **Art. 45** — may earn income by directly conducting economic
  activity, subject to three conditions: the activity relates to the
  foundation's goals, it is provided for in the statute, and it is a
  *"sporedna delatnost"* (ancillary activity). Unlike the Law on
  Associations, no quantitative threshold is stated — the test is
  qualitative.
- **Art. 47(2)** — property *"ne može se deliti osnivačima, članovima
  organa upravljanja, zaposlenima"*: cannot be divided among
  founders, governing-body members, or employees.
- **Art. 47(4)** — permits appropriate awards, reimbursement of
  justified costs, and **salaries**. No cap is stated in this law.
- **Art. 55(2)** — on dissolution, assets may pass only to another
  `zadužbina`, `fondacija` or `udruženje`.

Sources disagree on minimum assets: the statutory definition says a
`fondacija` has none, while some practitioners cite a nominal ~€1,000.
Verify before filing.

### Why not the others

- **`Zadruga`** — requires 5 natural persons and permits profit
  distribution by assembly decision. Fails the core requirement
  unless a constraint is bolted on (see social-enterprise status
  below).
- **`Udruženje`** — economic activity limited to *"manjeg obima"*,
  explicitly scoped to what is needed to achieve the association's
  goals. A SaaS business as primary revenue is a poor fit.
- **`Zadužbina`** — €30,000 in basic assets, with no compensating
  advantage over a `fondacija`.

### Social-enterprise status as an alternative constraint

The Law on Social Entrepreneurship (Sl. glasnik RS 14/2022, in force
2022-11-16) offers a different route: keep a commercial form and add
a statutory constraint.

- **Art. 8** — available to entrepreneurs, commercial subjects
  (companies and **cooperatives**), and civil-sector subjects.
- **Art. 10** — *"Imovina subjekta socijalnog preduzetništva ne može
  se deliti njegovim članovima"*; salaries and legitimate expenses
  excepted.
- **Art. 11** — at least **50% of profit** reinvested or donated to
  another social-entrepreneurship subject.
- **Art. 12** — at least one-third participation in decision-making
  for the relevant group.

This is the instrument that would make a `zadruga` non-distributing.
It is weaker than a `fondacija`: members still exist and still hold a
residual claim, and the reinvestment obligation is 50%, not all.
Recorded here because it is the strongest available option for anyone
who wants to keep cooperative form.

## Foreign registration and why it fails here

Registering a Dutch `stichting` or a Singapore CLG would sidestep the
"sporedna delatnost" question entirely, and is literally what Ghost,
Godot and Blender did.

It fails for Funarchy on one rule: **a legal entity is a Serbian tax
resident if it is established in Serbia *or has its place of
effective management and control there*.** A foreign foundation
directed by a Serbia-resident Founder is very likely a Serbian tax
resident regardless of where it is registered — producing Serbian
corporate tax *plus* foreign registration, banking, accounting and
filing costs.

Ghost's structure works because its management is not in a
jurisdiction that would claim it. Funarchy's is.

## Tax (2026 rates)

### Payroll — identical under every structure

A Serbian resident's salary is taxed the same way whether the payer
is a `fondacija`, a `d.o.o.`, or a foreign entity.

| | 2026 |
|---|---|
| Income tax | 10% above RSD 34,221/month non-taxable |
| Employee contributions | 19.90% — PIO 14, health 5.15, unemployment 0.75 |
| Employer contributions | 15.15% — PIO 10, health 5.15 |
| Max. monthly contribution base | RSD 732,820 (5× average) |
| Max. annual contribution base | RSD 8,793,840 |
| Annual surtax | +10% above 3× average annual income; +25% above 6× |

The contribution cap matters at Funarchy's target salary levels:
contributions stop growing above RSD 732,820/month, so the payroll
layer lands near 26% effective at high salaries, before the annual
surtax.

### Entity level

- **Corporate income tax:** 15% flat.
- **Non-profit exemption:** profit up to RSD 400,000 is exempt, but
  only if *all* conditions hold — no distribution to founders,
  employees or board; **salaries not above double the sector average
  in the commercial sector**; all profit used for the stated
  objectives; no unfair competition with private business. The salary
  condition puts this exemption out of reach at Funarchy's intended
  pay levels. Losing an exemption is not illegality — it means paying
  15% on remaining profit.
- **Dividends between two Serbian resident legal entities:** exempt.
  This is the clean route for moving money from a future `d.o.o.` up
  to the `fondacija`.
- **Donations:** deductible only up to 5% of total revenue — the
  wrong route for the same purpose.

### Paying people abroad

Withholding tax of 20% applies to payments to non-residents for a
*specific list*: dividends, royalties, interest, market research,
accounting and audit, and legal and business consulting, plus certain
lease payments — reducible by double-tax treaty.

**Software development is not on that list.** A foreign developer
contracting from abroad can generally be paid with no Serbian
withholding, and is taxed at home.

A non-resident board member taking a fee does receive Serbian-source
income. Unpaid board seats avoid the question entirely and are normal
for foundations.

### `Preduzetnik` as the payment route

A `preduzetnik` electing `lična zarada` pays contributions only on
the declared personal salary (capped at RSD 732,820/month), with
profit above that taxed at 10%. For high, stable income this is more
efficient than employment.

Two constraints:

- **Flat-rate (`paušal`) is capped at RSD 8,000,000/year** in
  revenue — roughly €68,000. Above that, bookkeeping is mandatory.
- **`Test samostalnosti`** — nine criteria; meeting five or more
  makes the `preduzetnik` "non-independent" and reclassifies the
  income at **20% of gross with no cost deduction, plus PIO 25.5%
  and health 10.3%**. The test **applies to foreign clients too**.
  A `preduzetnik` invoicing Funarchy would score at minimum on
  "≥70% of income from one client over 12 months" and "≥130 days for
  the same client over 12 months," with "client provides the tools"
  and "bears no independent business risk" plausibly also counting.
  This risk exists regardless of whether Funarchy's entity is
  domestic or foreign.

## Open questions for counsel

1. Where is the line on *"sporedna delatnost"* for a `fondacija`?
   What share of income may come from SaaS and consulting before the
   activity stops being ancillary?
2. May a `fondacija` found and wholly own a `d.o.o.`? The Law on
   Endowments and Foundations is silent.
3. Does *"anarchist digital governance models"* register as an
   `opštekorisni cilj`, or is a descriptive gloss needed? A
   `fondacija`'s purpose must be public-benefit and is
   ministry-supervised — this question is heavier than it was for a
   `zadruga`.
4. Minimum basic assets for a `fondacija`: none per the statutory
   definition, or a nominal amount in practice?
5. Can the statute seat the governing board with the people doing
   the work, and does that survive registration?
6. Does the `test samostalnosti` bite differently when the
   `preduzetnik` is the foundation's Founder rather than a
   subordinate contractor?

## Sources

Serbian law —
[Zakon o zadužbinama i fondacijama](https://www.paragraf.rs/propisi/zakon_o_zaduzbinama_i_fondacijama.html),
[Zakon o udruženjima](https://www.paragraf.rs/propisi/zakon_o_udruzenjima.html),
[Zakon o zadrugama](https://www.paragraf.rs/propisi/zakon_o_zadrugama.html),
[Zakon o socijalnom preduzetništvu](https://www.paragraf.rs/propisi/zakon-o-socijalnom-preduzetnistvu.html).

Tax —
[PwC: Serbia corporate residence](https://taxsummaries.pwc.com/serbia/corporate/corporate-residence),
[PwC: withholding taxes](https://taxsummaries.pwc.com/serbia/corporate/withholding-taxes),
[PwC: corporate deductions](https://taxsummaries.pwc.com/serbia/corporate/deductions),
[Council on Foundations: Nonprofit law in Serbia](https://cof.org/country-notes/nonprofit-law-serbia),
[Novi iznosi osnovica doprinosa za 2026](https://www.prlegal.rs/new-contribution-base-amounts-for-2026/),
[Test samostalnosti — 9 kriterijuma](https://www.paragraf.rs/100pitanja/posao/test-samostalnosti-za-preduzetnike-kriterijumi-objasnjenja-u-skladu-sa-zakonom.html),
[Zunic Law: corporate income tax 2026](https://zuniclaw.com/en/corporate-income-tax-in-serbia-2026).

Prior art —
[Ghost: about](https://ghost.org/about/),
[Ghost: moving to Singapore](https://ghost.org/changelog/moving-to-singapore/),
[Ghost Foundation Limited registry entry](https://www.sgpbusiness.com/company/Ghost-Foundation-Limited),
[Godot Foundation](https://godot.foundation/),
[Blender Foundation](https://en.wikipedia.org/wiki/Blender_Foundation),
[KVK: the stichting](https://www.kvk.nl/en/rules-and-laws/the-stichting/).
