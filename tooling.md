# Tooling Registry

The governance documents (01–03 and the bylaws, 07) speak in
tool-neutral terms. This living document is the one place that binds
those terms to concrete tools. Swapping a tool means changing one line
here and recording the change in `amendment-log.md` - nothing in the
charter or bylaws moves.

| Term in governance docs | Current binding |
|---|---|
| **The public record** | This git repository (canonical remote: github.com/funarchy; mirrors: to be added) |
| **The public forum** | GitHub Issues on the canonical remote |
| **The treasury** | See [04-treasury-wallet.md](04-treasury-wallet.md) and `treasury-address.md` |
| **Recorded agreement** (on a solution) | A 👍 reaction, an "Agreed" comment, or a PR approval on the solution's pull request |
| **Cooperator** (recognized standing, [03-amendment-process.md](03-amendment-process.md) Step 3) | Member of the `funarchy` GitHub organization, with membership set public so the "Member" badge shows on their comments |

The org member list is display, not record: the authoritative register
of cooperators is the admission decisions in `decisions.md` (the
durable-record rule). If a cooperator keeps their org membership
private, no badge shows - their standing is unchanged, and a reader
verifies it against the decision log rather than the forum.

## Why this indirection

The public *record* is the repository itself - versioned, forkable, and
mirrorable by anyone with `git clone`. It does not depend on any hosting
company. GitHub is one mirror plus a discussion layer, chosen for reach,
not required by design. Sovereignty demands that no platform can halt
Funarchy's governance by suspending an account.

## The durable-record rule

Forums are ephemeral; the record is durable. Every governance outcome -
approved amendments, decisions, treasury reports - lands in the repository
(`amendment-log.md`, `decisions.md`, `treasury-reports/`). Discussion may
live in the forum, but if the forum vanished tomorrow, no governance state
would be lost - only conversation history.

## Migrating a binding

1. Report a pollution describing what is polluted about the current tool
   (lock-in, censorship risk, cost, friction).
2. Propose the replacement as a solution; include the migration plan for
   any open discussions.
3. Decide per the current phase rules ([03-amendment-process.md](03-amendment-process.md)).
4. Update the table above and record the change in `amendment-log.md`.
