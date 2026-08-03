# llm wiki

**A curated, versioned knowledge base that lives in the repository - topic
pages with schemas, links, and automated correctness checks (evals) that
agents navigate along explicit links instead of similarity search - and
humans read and maintain too.**

## What it is

A set of markdown topic pages inside the project repository, held to a
schema: every page declares its type, sources, and links; indexes wire
pages into a navigable graph; agent skills - predefined procedures an
agent can run - exist for ingesting new knowledge, querying, finding
gaps, and adversarially reviewing pages against their sources. An agent starting a task reads the index, follows two or three
links, and has the project's actual conventions and architecture in
context - the same pages its human teammates read and maintain through
normal review.

## Why it's needed

An agent without a knowledge base re-derives your project from scratch
every session - reading code, guessing conventions, burning tokens to
recover what the team already knows. Worse, what it recovers is private
to that one session and that one person's agent: knowledge stays in heads
and chat logs. The wiki turns team knowledge into a shared, versioned,
inspectable artifact - one source of truth that every teammate and every
agent reads, and that improves through pull requests like everything
else. Your domain expertise becomes something the whole team - and the
whole team's agents - can use, with your name on the commit.

## Why not X

**Notion / Confluence** - built for humans, not repositories. Both ship
official agent integrations now, but the deeper gaps remain: no schema,
no eval discipline, content in a rented silo, and nothing connecting a
page to the code it describes. Use them if your knowledge never touches
a repository.

**RAG over a vector database** - retrieval by statistical similarity:
fragments without structure, no accountability for what the agent
"knows," silent index drift, and infrastructure to run. The wiki is
curation instead of retrieval - fewer tokens, auditable context, no
embedding pipeline. Use RAG when the corpus is huge and nobody owns it;
use a wiki when the knowledge is yours.

**A plain docs/ folder** - the starting point, and where docs go to rot.
No schema, no link discipline, no gap detection, no review-against-source.
The llm wiki is a docs folder with a maintenance discipline strong enough
that agents can safely spend tokens trusting it.

## Works with

Ships inside every [Funarchy Space](03-space.md) workspace; updated as
solutions land through [RPPS](04-rpps.md); the first thing any agent reads
before touching a task.

## Status

In production at Funexpected - the skillset and schema run daily against
a real product codebase. Open-sourcing is pending agreement with the
current maintainers; if that does not work out, it will be rewritten from
scratch. Target: **Q4 2026**.
