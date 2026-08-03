# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this repository is

The governance and product documentation for **Funarchy**, a workers' cooperative being founded by jkbo. It is pure Markdown — there is no build system, linter, or test suite. The repository itself is "the public record": versioned, forkable governance state. GitHub Issues on the canonical remote is "the public forum."

## Document architecture

Three tiers of documents with different rules:

1. **Numbered governance docs (`01`–`07`)** — charter, bylaws, roadmap, amendment process, treasury wallet, onboarding, carved-domains examples. Numbers are reading/dependency order. The charter (`01-charter.md`) and `products/` are reviewed line by line and the author stands behind every sentence; `02`–`07` are drafts still in progress. `07-carved-domains.md` is illustrative and explicitly non-binding: fictional worked examples, not plans — if it ever disagrees with charter/bylaws/roadmap, those govern.
2. **`products/` (`01`–`07` + README)** — seven products forming a stack (each layer proves the one below). Numbers are reading order; each page assumes the reader has read all lower-numbered pages, and every dependency has a smaller number — preserve that invariant when editing.
3. **Living records (unnumbered)** — `tooling.md`, `treasury-reports/`, and files created at trigger events: `amendment-log.md` (first amendment), `decisions.md` (launch), `treasury-address.md` (wallet setup). These are appended to, not read in sequence. Don't create the trigger-event files preemptively.

**Precedence:** if documents disagree, the charter governs. The five core principles in the charter (Openness, Non-Exploitation, Sovereignty, Permissionlessness, Co-Benefit) cannot be amended — a Funarchy with different values forks instead.

## Key conventions

- **Tool-neutral language in governance docs.** Documents `01`–`04` say "the public forum" and "the public record," never "GitHub" or "git repository." The one place that binds terms to concrete tools is `tooling.md`. Don't leak tool names into the governance docs.
- **Problem-first vocabulary.** A **pollution** is a problem described as a problem (never a prescribed fix); a **solution** is a concrete proposal (for governance: the exact new text, as a diff). The boundary rule: *changes a rule → pollution; applies a rule → decision (recorded in `decisions.md`)*. This distinction is load-bearing throughout the documents — keep it exact.
- **Domain vocabulary.** Domains are **carved, not pre-designed** — never introduce a pre-made domain list. The **founding domains** are technology (the Founder) and operations (the Partner); new domains are *carved* from that map via the amendment process (qualitative test: sustained real work, more than one person, someone already taking and holding responsibility whom the others accept). The first carve is delegation; the **second carve starts the Federated Phase** — phase transitions are events, not dates (dates in the docs are estimates). Keep the carve/founding-domain wording exact across docs.
- **Steward, never "lead."** Responsibility > leadership: the role-holder of a domain is its **steward** — named for responsibility already held, recognized after the fact, revocable. Don't reintroduce "lead/leader" for roles ("Founder-Led Phase" as a phase name is the deliberate exception — it describes decision authority, not a role).
- **Changing governing documents** (charter, bylaws, roadmap, standing processes) goes through the pollution → solution pipeline in `04-amendment-process.md` and lands in `amendment-log.md`. Editorial fixes to draft docs are normal work; substantive changes to reviewed docs are amendments.
- **The durable-record rule.** Governance outcomes (amendments, decisions, treasury reports) must land in repository files, never only in forum discussion.
- **Honesty over polish.** Status tables state exactly what exists today, including risks (e.g. the llm wiki IP caveat). Don't inflate statuses or soften stated risks when editing.
- **Prose style.** Most documents hard-wrap prose at ~72 characters — match the wrapping style of the file being edited. Cross-references are relative Markdown links.

## Issue templates

`.github/ISSUE_TEMPLATE/pollution.yml` mirrors the required pollution fields from `04-amendment-process.md` (What's polluted / Who it affects / Cost of not fixing / Acceptance criteria + optional solution sketch). If the amendment process's required fields change, update the template to match.
