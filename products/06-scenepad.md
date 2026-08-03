# scenepad

**The TypeScript implementation of PMS, plus a React Native toolkit and
an agent skillset - together turning Funarchy Space into a
general-purpose engine for apps and games.**

## What it is

Three layers in one open monorepo. The runtime implements
[PMS](05-pms.md) on an entity-component-system core: channels, systems with
declared ownership, presentations. The toolkit provides the interactive
building blocks - scenes, draggables, shared transforms - rebuilt
PMS-native for React Native, running on web and mobile from one codebase.
The skillset teaches agents the build loop: spec-first, test-first,
regenerate-don't-patch. Development started inside Funexpected's math
product, where these mechanics ship to real learners.

## Why it's needed

An engine for the agent age has four requirements the old engines never
faced:

- everything is plain code and diffable - agents and git must see every
  change
- units are regenerable from their contracts - fast iteration is the
  entire point
- tests derive from specs - the agent's work must be checkable without
  trusting the agent
- the whole loop is cheap enough in tokens that a small team - or a
  teacher, or a teenager - can afford to build seriously

scenepad is that engine, and it is what makes
[Funarchy Space](03-space.md) more than a dev environment - in two ways.

Shipping real apps and games is one: a team enters Space and builds
end-to-end together, with each person's skills contributing and agents
doing the work in between.

Extending Space itself for your own needs is the other. An organization
describes the tool it needs in plain words and grows it inside its own
Space: a local store's tool that audits missed goods and reorders them
from a configured supplier by email - in one click, or automatically.
Software for exactly one organization, owned by that organization, too
small and too specific for any vendor to ever build - which is most of
the software the world is missing.

## Why not X

**Unity** - an editor-first world whose truth lives in asset databases
and scene files that agents and git cannot meaningfully read, built
around a single person at an editor. Unbeatable for heavy 3D; wrong
shape for cooperative, agent-assisted, code-first creation.

**Godot** - open-source, text-based scenes, genuinely git-friendly:
credit where it is due. It is still designed around one person at an
editor, and its scene tree carries no ownership contracts - agent
iteration gets no safety rails. Use it (or Unity) when the game is
seriously 3D.

**Phaser / PixiJS** - rendering libraries, honest ones. They draw
sprites and leave the architecture to you, which means every project
reinvents state discipline - and agents inherit the mess. scenepad's
value is precisely the discipline.

**Raw React Native** - the platform scenepad stands on, unopinionated
about state and interaction by design. Without a pattern, each app grows
its own; with PMS, every scenepad app speaks the same contract language
agents already know.

## Works with

Implements [PMS](05-pms.md); developed and used inside
[Funarchy Space](03-space.md); [Type Space](07-type-space.md) is its first
full product.

## Status

Extraction into a standalone open-source monorepo has started: the PMS
runtime, the React Native toolkit, and a browser-runnable flagship demo,
built test-first against the spec. Target: **Q4 2026 - Q1 2027**.
