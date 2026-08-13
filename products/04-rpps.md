# RPPS

**Pollutions & Solutions running inside Funarchy Space - typed problem
reports, owned solutions, bound tasks, and explicit handoffs, wired into
git and enforced by tooling.**

## What it is

The software implementation of the [Pollutions & Solutions](02-pollutions-n-solutions.md)
methodology. Pollutions are typed issues with required problem-first
fields, guarded by automation that rejects anything else. A solution is a
pull request with a brief public proposal, exactly one accountable owner,
rotating assignees moving through explicit handoffs, and zero or more
task rows bound to it - tasks never float free. Agents participate at
every step: they report pollutions with diagnostics attached, draft
solution proposals, and execute tasks - while ownership and the decision
stay human and visible. It runs on the team's forum and record (GitHub
today) and is designed to be moved off it completely.

## Why it's needed

A methodology without enforcement decays into informal guesswork -
issues drift back into prescriptions, ownership blurs, tasks lose their
owners. RPPS makes the discipline mechanical, and that matters most once
agents join the team: an agent can open ten plausible changes an hour.
The pipeline forces every change to answer a stated human problem, with
a named human owner - so the team steers instead of drowning in review.

## Why not X

**Raw GitHub Issues + Projects** - untyped issues that arrive as
prescriptions, no ownership discipline, boards that describe work without
governing it. RPPS is the missing discipline layer on top - and unlike
your issue history, it is designed so that if you ever leave GitHub, you
take all of it with you.

**Jira** - process at its maximum: workflows about workflows. It earns
its enterprise keep - audit trails, compliance, coordination at
300-person scale - but at cooperative scale that machinery substitutes
for cooperation instead of carrying it, and agents arrive bolted on as
ticket-writers.

**Linear** - genuinely well-crafted, and closed, rented, and
solution-shaped: a beautiful list of what someone decided to do, with the
problems left in people's heads.

## Works with

Native to [Funarchy Space](03-space.md); implements
[Pollutions & Solutions](02-pollutions-n-solutions.md); what solutions learn
flows into the [llm wiki](01-llm-wiki.md). Funarchy's own
[governance](../03-amendment-process.md) runs on the same
pipeline.

## Status

In production at Funexpected as Space's workflow layer (under its working
name). Renamed and open-sourced right after Space, target **Oct 2026**.
