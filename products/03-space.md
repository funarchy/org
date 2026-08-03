# Funarchy Space

**A self-hosted, agent-native cooperative development environment - the
place where a team and its agents share workspaces, sessions, and reviews
on hardware you own.**

## What it is

A web-based development environment a whole team enters together -
reachable from a browser today, with standalone thin-client and local
container-wrapped forms planned.
Every branch gets an instant copy-on-write workspace; every agent session
is bound to a workspace and visible to the team; work moves between
people and agents through explicit handoffs; reviews happen where the
work happened. It runs on an ordinary Linux machine - a rented Hetzner
server, a home server, a machine in your school - and the team owns
every byte of it. For teams that want one click instead of running
servers, the cooperative hosts it as a service.

## Why it's needed

Development environments were designed for individuals; agent tooling
made that worse, selling each developer a private cockpit and a fleet of
agents - the one-person orchestra. But real teams cooperate: they hand
work to each other in the middle of a task, review each other's sessions,
share one knowledge base, and need to see what agents did and who asked
them to. Space is built around that - shared visibility of sessions,
handoff as a built-in operation, workspaces cheap enough that parallel
human+agent work rarely queues. And it is self-hostable because sovereignty is not a
feature: a team whose entire working environment can be repriced or
revoked by a platform does not own its own cooperation.

## Why not X

**GitHub Codespaces / Gitpod / Coder** - closed products rented per
seat: you cannot read the code that runs your environment, cannot host
it yourself, and cannot leave with your workflows intact. To be fair,
hosted Space is also a paid service - the difference is that it is the
same open product: whatever we host for you, you can take tomorrow and
run yourself, with your data, history, and workflows. Use the closed
clouds if zero-maintenance matters more to you than the option to
leave.

**Local VS Code + an agent plugin** - the one-person orchestra by
design. No shared sessions, no handoffs, no team-visible agent history;
cooperation happens by pasting things into chat. Fine for solo work;
it simply is not a place a team inhabits.

**Devcontainers / Nix environments** - reproducible machines, and a good
piece of the puzzle. But a reproducible machine is not a shared place:
no sessions, no workflow, no cooperation layer.

**Unity / Godot** - complete creation environments, but single-player
ones: one person at one editor, with teamwork pushed out to version
control, asset locks, and meetings. No shared sessions, no handoffs, no
team-visible agent work - what agent tooling exists is bolted onto the
editor, not the team. Space with [scenepad](06-scenepad.md) inside it
covers the same ground for code-first apps and games, as a place a team
inhabits together; for heavy 3D they remain the right tools (the honest
engine-level comparison is on the [scenepad page](06-scenepad.md)).

## Works with

[RPPS](04-rpps.md) is its workflow layer; the [llm wiki](01-llm-wiki.md) ships
in every workspace; [scenepad](06-scenepad.md) apps are developed inside it,
turning Space into an app engine.

## Status

In daily production use at Funexpected as the internal development
environment (under its working name). Rename to Funarchy Space,
extraction, and open-sourcing target **Sep-Oct 2026**. Hosted
one-click instances are the cooperative's first product revenue stream
([financial model](../README.md)).
