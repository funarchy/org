---
description: Propose a solution — a draft PR answering one or more pollutions, per 03-amendment-process.md Step 2.
argument-hint: '[#pollution…] [prose with optional "todo:" bullets]'
---

Propose a **solution** — a pull request answering one or more open
pollutions, following [03-amendment-process.md](../../03-amendment-process.md)
Step 2: the diff is the exact new text, the body links the pollutions
it answers, plus a brief rationale (a screenful, arguable).

All mechanics are done directly with `git` and `gh` — there is no
standalone tool and no lock. Your job is the judgment: gather the
proposal, compose the title/body, pick the referenced pollutions,
resolve the branch decision — then run the mechanics and report.

## Step 0: Preflight — gh must exist

Run `command -v gh`. If it is **missing**, the command fails here:
ask via `AskUserQuestion` — "GitHub CLI (gh) is not installed; it is
required for this command. Install it now?" with options **Install
via Homebrew** (`brew install gh`, then tell the user to run
`gh auth login` in a terminal — it is interactive) and **Abort**.
On abort, stop; do not fall back to raw git pushes or the web UI.

If gh exists, run `gh auth status`; if unauthenticated, tell the
user to run `gh auth login` and stop.

## Implementation steps

1. **Gather the proposal**, in priority order: prose args → use them;
   no args → summarize _this conversation_ into a proposal; nothing
   to go on → stop and ask what the solution is.
2. **Pollutions are the link.**
   - Every `#N` in the args → a `Fixes #N` (fully answers) or
     `Part of #N` (partial narrowing) line in the body — ask which
     if unclear; #1-style long-lived pollutions are usually
     `Part of`.
   - When the prose describes a problem with no filed pollution,
     offer **once** via `AskUserQuestion`: "File this as a pollution
     first and reference it?" — on yes, open one with
     `gh issue create` using the required fields from
     [03-amendment-process.md](../../03-amendment-process.md) Step 1
     (What's polluted / Who it affects / Cost of not fixing /
     Acceptance criteria), label `type: pollution`, then use the
     resulting `#N`. A nudge, not a gate.
3. **Compose** a `title` (sentence-case, ≤ ~70 chars) and a `body`
   following [.github/PULL_REQUEST_TEMPLATE.md](../../.github/PULL_REQUEST_TEMPLATE.md).
   `todo:` bullets from the args become a `- [ ]` task list in the
   body. Write the body to a temp file.
4. **Choose the branch.** Read state with `git branch --show-current`
   and `gh pr list --head <branch> --json number`, then:

   | State                | Branch                                   |
   | -------------------- | ---------------------------------------- |
   | On `main`            | new `solution/<slug>` from main           |
   | On non-main, PR-less | ask user¹: current branch _or_ new slug   |
   | On non-main, PR-full | new `solution/<slug>` from main           |

   ¹ Ask via `AskUserQuestion`: "Create the PR for the current
   branch, or a new branch from main?" Suggest `solution/<slug>`
   from the title lowercased (non-alnum → `-`, filler dropped,
   ≤ ~5 words).

5. **Mechanics**, in order; stop and surface the error if any step
   fails — do not improvise around a failed push:

   ```
   git switch -c solution/<slug>   # only if a new branch is needed
   git add <files> && git commit   # only if changes are uncommitted
   git push -u origin <branch>
   gh pr create --draft --title "<TITLE>" --body-file <tmp> --base main
   ```

   The PR always opens as a **draft** — Step 3 of the amendment
   process gives discussion 2 weeks minimum before any decision.

6. **Report**: PR URL, branch, and the pollutions referenced.

## Don'ts

- Don't include AI-attribution lines in titles, bodies, or commits.
- Don't gate on a pollution reference — nudge once, then respect
  the answer.
- Don't mark the PR ready for review — discussion time is the
  proposer's and decider's call, not the command's.
- Don't invent a title/body the user didn't imply.
- Don't auto-stash; if the tree is dirty with unrelated changes,
  ask.
- Governance outcomes land in repository files, never only in the
  PR discussion (the durable-record rule).
