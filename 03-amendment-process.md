# Amendment Process: How Funarchy Evolves

Funarchy governs its own evolution with the same problem-first method its
products implement: **pollutions and solutions**. This document defines the
method self-containedly and applies it to governance.

Amendments touch three governing documents:

1. **Charter** ([01-charter.md](01-charter.md)) - values, principles, decision-making
2. **Roadmap** ([02-roadmap.md](02-roadmap.md)) - timeline, milestones, success criteria
3. **Bylaws** ([07-bylaws.md](07-bylaws.md)) - the legal encoding, filed with the Serbian registry when the cooperativa is registered

They are connected: charter changes often require bylaw updates; major
roadmap shifts need charter approval.

---

## Pollutions and solutions

A **pollution** is a problem, described as a problem: a harm, a friction,
an injustice, an unclearance. Never a prescribed fix. A **solution** is a
concrete proposal that answers one or more pollutions - for governance,
that means a change to the charter, bylaws, roadmap, or a standing process.

The split is deliberate and it distributes power:

- **Reporting a pollution requires no authority.** Anyone - member,
  cooperator, outside contributor - can say "this hurts" without knowing
  or deciding what to do about it.
- **Proposing a solution requires no authority either.** Anyone can answer
  an open pollution, including with a competing proposal.
- **Only the decision is phase-gated** (see Step 4). As governance evolves
  Founder-Led → Federated → Assembly, the pollution and solution mechanics
  never change - only who gives the nod.

Prescribing solutions is a form of authority; describing problems is not.
Problem-first is how the amendment process itself encodes the sovereignty
and openness principles.

---

## What needs a pollution - and what does not

**Changes go through pollutions.** If it changes a governing document
(charter, bylaws, roadmap) or a standing process, it starts as a pollution
and lands as a solution.

**Decisions do not.** Applying existing rules to a case - admitting a
member, approving a budget, executing a treasury transaction, scheduling
an assembly - is a decision under the current phase rules, recorded in
`decisions.md`. Do not write a fake pollution ("Pollution: Alice is not
yet a member") to dress a decision as a problem; that corrodes the
problem-first discipline.

**The boundary rule:** changes a rule → pollution. Applies a rule → decision.

---

## Step 1: Report the pollution

Open a pollution in the public forum (current binding: [tooling.md](tooling.md))
with these required fields:

```
## What's polluted
[The problem as observed - behavior, harm, friction. Not a fix.]

## Who it affects and how
[Members, cooperators, community, outsiders?]

## Cost of not fixing
[What decays if this stays as it is?]

## Acceptance criteria
[How we know the pollution is gone.]
```

An optional _Proposed solution_ sketch is allowed only to clarify the
picture - it is never a call to action; the solution decides.

### Triage: prioritization (interim mechanism)

After a pollution is filed, the phase decider (Founder-Led Phase: the
Founder) assigns it a **public priority**. Priority orders the decider's
attention - which pollutions get solved first - and signals proposers
where solutions are most welcome.

What priority is **not**:

- **Not a validity judgment.** A low-priority pollution is still a real
  pollution; no one is told their problem doesn't exist.
- **Not a gate.** Anyone may propose a solution to any open pollution at
  any time, regardless of its priority.
- **Not final.** Priorities are public and arguable - challenge one in
  the pollution's discussion, and the decider answers.

Guardrail: low priority must never become a silent graveyard. If a
pollution sits unaddressed while its reporter keeps caring, that
disagreement about priority is itself worth discussing openly.

This mechanism is deliberately minimal. Designing a proper prioritization
and validation process - one that scales past a single decider - is
future work for the Federated Phase, and a fitting early test case for
Funarchy's own governance instruments.

**Example:**

```
## What's polluted
The charter requires assembly votes to reach 70% support, but abstentions
count against the threshold. Two proposals with clear majority support
have failed because quorum-but-abstaining members were counted as "no".

## Who it affects and how
Every assembly participant; proposals die that the community actually wants.

## Cost of not fixing
The assembly learns that voting is futile; participation drops.

## Acceptance criteria
Abstentions are counted in quorum but not against the support threshold,
and the charter says so explicitly.
```

## Step 2: Propose the solution

A solution is a change to the governing documents, proposed against the
public record (currently: a pull request), with:

- **The exact new text** - governance is text; the diff is the proposal.
- **The pollution(s) it answers**, linked and closed by it.
- **Brief rationale** - a screenful, arguable, not a generated dump.

Competing solutions to the same pollution are welcome; the decision step
picks one (or none).

## Step 3: Discuss

- Where: on the solution, in the public forum.
- Who: anyone. No voting yet - clarify, surface consequences, suggest
  amendments to the amendment, or file a competing solution.

### The discussion window

A solution may be decided once all three of these hold, tested at
the moment of deciding:

1. every substantive comment bearing on the clock is at least
   **72 hours** old, and
2. **24 hours** have passed since the current text was proposed, and
3. either everyone who will make this decision (Step 4), apart from
   the proposer, has recorded agreement with the current text, or
   **72 hours** have passed since the current text was proposed.

"Since the current text was proposed" means since the solution was
opened, or since its text last changed, whichever is later. A change
to the text is a new proposal: the clocks of conditions 2 and 3
restart, and agreement with the old text does not count as agreement
with the new - people agree to text, and after a change it is
different text. Comment ages in condition 1 are untouched by
changes: a comment's clock belongs to its author, so an edit cannot
launder away a fresh objection.

The 24 hours are a floor with no exception. A window shorter than a
day excludes whoever is asleep, by construction - it would make
Funarchy choose whose timezone counts.

Agreement is recorded on the solution in the public forum; the
concrete forms are bound in [tooling.md](tooling.md). When nobody
but the proposer is eligible to decide, condition 3 is satisfied by
its first branch at the floor: open it, sleep on it, decide
tomorrow.

**Whose comments bear on the clock: cooperators' and the
deciders'.** Anyone may comment - outside comments are input the
deciders weigh, and the verdict's rationale must answer the ones it
sets aside - but only recognized voices hold the window. A
cooperator may **second** an outside comment, taking responsibility
for it; it then bears on the clock as their own. Sustained,
valuable outside contribution is how cooperators are recognized -
an admission decision under the phase rules, recorded in the
decision log; recognition confers standing, never pay and never a
claim.

A **substantive comment** raises a problem not already answered,
proposes different text, or asks a question that has not been
answered. Approvals, acknowledgements, editorial nits, and
repetition of answered points do not move the clock. The
commenter's labelling stands unless the decider records why it
does not.

The proposer may extend the window at any time, for any reason.
Nobody may shorten it - including the decider.

**This is the only place these durations are stated.** The charter,
the roadmap and the bylaws point here instead of repeating a
number, so the rule cannot drift apart from itself.

Why it is built this way: a window exists so that those with
standing to object get time to object - and, stated honestly, that
is narrower than "anyone": outsiders are heard through answers and
seconding, not through the clock, so an open forum cannot stall
decisions it holds no responsibility for. Elapsed days buy nothing
when nobody is there, so a flat fortnight left the founding period
choosing between waiting on an empty room and visibly breaking its
own rule. This closes as soon as everyone who could decide has
agreed, or once discussion has gone quiet; it holds open while
recognized argument continues. One rule covers one participant and
fifty.

## Step 4: Decide (phase-dependent)

The handshake, per the current governance phase:

- **Founder-Led Phase:** the Founder decides, with a written rationale
  (one paragraph minimum). Once the partnership begins, "the Founder"
  reads "the Founders, jointly" - both must agree, and a deadlock means
  the status quo holds.
- **Federated Phase:** the relevant domain stewards reach consensus
  and record it.
- **Assembly Phase:** the assembly votes per the voting mechanism.

The verdict - approved or rejected, by whom, and why - is recorded on the
solution itself, and states when the discussion window opened, when it
closed, and that it was met.

This applies to the decider's own solutions on exactly the same terms.
The point is not ceremony: "opened one day, decided the next" must
never be ambiguous between *weighed* and *ignored*, because once a
reader cannot tell the difference, every window in the record is worth
less - including the ones that will matter when someone is objecting
to something real.

## Step 5: Land the change (if approved)

1. **Merge the solution** into the public record - the governing document
   now says the new thing.
2. **Record it** in `amendment-log.md`:

   ```
   ## Amendment #N: [title]
   - Approved: [date]
   - Pollution(s): [links]
   - Solution: [link]
   - Approved by: [Founder-Led Phase: Founder | Federated Phase: steward consensus | Assembly Phase: vote]
   - Window: [opened] → [closed]
   - Effective: [usually immediately]
   ```

3. **File with the Serbian registry** (bylaws changes only) - quarterly or
   as needed, with translation; filing confirmations kept in `filings/`.
4. **Announce** - the monthly report lists all landed amendments; major
   ones get a standalone announcement.

**The durable-record rule:** discussion lives in the forum and may be
lost; outcomes live in the repository and may not. If the forum vanished
tomorrow, every landed amendment, rationale, and verdict survives in git.

---

## What can be amended

**Charter & roadmap:** almost anything - values, timelines, processes.

**Bylaws:** almost anything, but changes to these need Serbian legal review
before filing:

- Governance phases (Founder-Led, Federated, Assembly)
- Membership criteria
- Decision-making rules
- Dissolution clause
- Financial distribution policy

**Tooling bindings:** via [tooling.md](tooling.md) - same pipeline, one-line
landing.

**What CANNOT change:** the five core principles. A future Funarchy that
disagrees with them should fork, not amend.

---

## Decider's checklist

Before approving a solution:

- [ ] **Is the pollution real?** A problem someone observed, not a fix in
      a costume?
- [ ] **Does the solution meet the pollution's acceptance criteria?**
- [ ] **Does it align with the five principles?** Openness,
      Non-exploitation, Sovereignty, Permissionlessness, Co-benefit
- [ ] **What breaks?** Existing decisions, processes, or practices that
      contradict it?
- [ ] **Is the timing right?**
- [ ] **Is the language clear?** Would a new member understand it?
- [ ] **Do we have consensus (Federated and Assembly Phases)?** Genuine
      agreement, not a decision forced on dissenters?

---

## Amendment frequency & governance health

- **Founder-Led Phase:** expect 5-10 amendments (establishing first processes)
- **Federated Phase:** expect 3-5 amendments/quarter (refining domain structures)
- **Assembly Phase:** expect 2-4 amendments/quarter (community-driven improvements)

**Red flags:**

- No pollutions for 6+ months - either nothing hurts (unlikely) or people
  don't feel empowered to report; investigate the latter.
- More than 15 amendments/quarter - governance is churning, or changes are
  too large for single amendments.
- Pollutions that read like prescriptions - the problem-first discipline
  is eroding; push back at the report step, kindly.

---

## Amendment history

[Maintained in `amendment-log.md`]
