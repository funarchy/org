# PMS

**An architecture pattern that makes agent-driven development cheap:
small isolated units with declared ownership, so testing, rewriting, and
iterating cost minimal tokens - and parallel work never collides.**

## What it is

A pattern for structuring interactive applications. State flows through
**channels**; **systems** react to frames, changes, and messages, and
declare up front exactly what they write, send, spawn, and destroy;
**presentations** compose systems into user-facing units. Those
declarations form an ownership map: two units that would touch the same
state are visible from their declarations, before anything runs. Every unit is
small enough to hold in one context window, specified enough to test
against its contract, and cheap enough to regenerate whole rather than
patch.

## Why it's needed

Pre-agent architectures optimize for what humans do: read code
top-to-bottom, avoid repetition, build clever abstractions. Agents work
differently - the cost of any change is proportional to the context
needed to make it safely, paid in tokens every single time. A global
store means every change needs whole-app understanding, forever. PMS
inverts the economics: contracts carry the safety, so a unit can be
tested, rewritten, or regenerated from its declaration alone. And the
ownership map is the cooperation-first commitment at the architecture
level - several people, each with their own agents, work on the same app
in parallel, and the pattern makes any collision between their changes
detectable from the declarations alone.

## Why not X

**Redux / MobX / global stores** - one shared state tree where any code
can reach anything; correctness lives in convention and review. A
well-sliced store helps, but nothing *declares* ownership - so an agent
change still typically needs app-wide context, and the token bill
compounds with codebase size.

**Classic ECS** - the right granularity (that is why PMS builds on it)
but no contracts: any system can touch any component, so nothing is
statically checkable and parallel work still collides. PMS is ECS plus
declared ownership.

**Microservices / micro-frontends** - isolation bought at deployment
cost: network boundaries, versioned APIs, operational sprawl. PMS
isolates *inside* one application - no network boundary, no deployment
cost.

**"Just prompt harder"** - the default the agent economy sells you:
re-derive the invariants in every session and pay tokens for what a
contract states for free. This is exactly the workflow that token-billed
incentives predict - and the one PMS exists to refuse.

## Works with

[scenepad](06-scenepad.md) is the reference implementation; apps built with
it are developed in [Funarchy Space](03-space.md), where agents apply the
pattern through its skillset.

## Status

Specification written (pattern + reasoning documents); the reference
implementation (an ECS-based TypeScript runtime) is in progress. Target:
**Q4 2026**.
