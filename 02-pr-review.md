# Mid-Week PR Review

← [Back to Learning Framework](./README.md)

**When:** Wednesday, 9:00 AM – 11:00 AM  
**Artifact:** PR opened and closed same day

---

## What it's for

The Wednesday PR review is a focused practice session for the mechanics of professional code review. You open a pull request, a peer reviews it with written comments, you discuss it live, and it's closed the same morning. That's it.

This is separate from the Friday peer review. The goal here isn't to reflect on the week's module — it's to practice reading unfamiliar code carefully, writing specific and constructive feedback, and being able to defend your own decisions in writing.

---

## Setup: the shared sandbox repo

Everyone works inside one shared GitHub repository under the LEVEL3 organisation. Your folder lives at `participants/[name]/week-X/`. Your weekly work goes in a feature branch, and your PR is opened from that branch into `main`.

This is how real teams work: shared codebase, peer review, visible history. Mentors can see all PRs in one place without needing access to individual repos.

---

## How big should the PR be?

Small to medium — roughly **150–300 lines changed** (additions and deletions combined). One clear intent. If it can't be described in a single sentence, it's too big.

**Example:** a data transformation step that reads raw CSV sales data, normalises column types and date formats, handles missing values with a documented strategy, and outputs a clean Parquet file. That might be a new `transform.py`, changes to a pipeline config, and a basic test. Enough to have a real conversation about structure, edge case handling, naming, and design decisions — without overwhelming the reviewer.

---

## Wednesday timeline

| Time | Activity |
|---|---|
| **9:00 AM** | Author opens PR with the completed description template |
| **9:00 – 10:00 AM** | Reviewer reads the code independently and leaves written comments (aim for at least 3–5 meaningful ones) |
| **10:00 – 11:00 AM** | Author and reviewer sit together, walk through each comment, discuss and resolve |
| **By 11:00 AM** | PR is merged or closed with a short written summary. Done. |

---

## PR description template

Every PR needs these four things filled in before the review starts:

- **What does this PR do?** (1–3 sentences)
- **Why did you approach it this way?** (your reasoning, not just what you did)
- **What are you unsure about?** (be honest — this helps your reviewer focus)
- **How to test it?**

---

## Reviewer checklist

Your written comments should cover some of the following. Not all of them — but each one should be specific and actionable:

- Does the code actually do what the description says?
- Is there a simpler way to get the same result?
- Are functions and variables named clearly?
- Is anything repeated that could be extracted or reused?
- Are edge cases or errors handled?
- What's one thing you'd do differently, and why?

> **The rule that makes prep non-optional:** If you wrote a comment, you have to be able to explain it out loud. That means you can't skim and rubber-stamp — you have to read carefully enough to actually have an opinion.

---

*LEVEL3 · Arkadia Heilbronn gGmbH · level3@arkadia.hn · level3.hn*
