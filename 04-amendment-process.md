# Amendment Process: How Funarchy Evolves

Funarchy governs its own evolution with the same problem-first method its
products implement: **pollutions and solutions**. This document defines the
method self-containedly and applies it to governance.

Amendments touch three governing documents:

1. **Charter** ([01-charter.md](01-charter.md)) - values, principles, decision-making
2. **Bylaws** ([02-bylaws.md](02-bylaws.md)) - the legal encoding, filed with the Serbian registry
3. **Roadmap** ([03-roadmap.md](03-roadmap.md)) - timeline, milestones, success criteria

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
- How long: 2 weeks minimum (longer for major changes; the proposer may
  extend).
- Who: anyone. No voting yet - clarify, surface consequences, suggest
  amendments to the amendment, or file a competing solution.

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
solution itself.

## Step 5: Land the change (if approved)

1. **Merge the solution** into the public record - the governing document
   now says the new thing.
2. **Record it** in `amendment-log.md`:

   ```
   ## Amendment #N: [title]
   - Approved: [date]
   - Pollution(s): [links]
   - Solution: [link]
   - Approved by: [Founder-Led Phase: Founder | Federated Phase: leads | Assembly Phase: vote]
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
