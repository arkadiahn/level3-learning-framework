# Mid-Week PR Review

← [Back to Learning Framework](./README.md)

**When:** Friday 12th June, 14:30 AM – 16:00 AM  
**Artifact:** PR opened and closed same day

---

## What it's for

The PR review is a focused **practice session for the mechanics of professional code review**. You open a pull request, a peer reviews it with written comments, you discuss it live, and it's closed the same afternoon. That's it.

The goal here is to practice reading unfamiliar code carefully, writing specific and constructive feedback, and being able to defend your own decisions in writing.

---

## Setup: the shared sandbox repo

Everyone receive a buggy code from one shared GitHub repository under the LEVEL3 organisation. Your work is to open your branch, find a bug, fix it, and open a PR from that branch into `main`. Then we will have 2 rounds code review to close those PRs.

This is how real teams work: shared codebase, peer review, visible history.

---

## PR description template

Every PR needs these four things filled in before the review starts:

- **What does this PR do?** (1–3 sentences)
- **Why did you approach it this way?** (your reasoning, not just what you did)
- **What are you unsure about?** (be honest — this helps your reviewer focus)
- **How to test it?**

---

## How big should the PR be?

Keep it small — under **25 lines changed** (additions and deletions combined). One clear intent. If it can't be described in a single sentence, it's too big.

**Example:** a data transformation step that reads raw CSV sales data, normalises column types and date formats, handles missing values with a documented strategy, and outputs a clean Parquet file. That might be a new `transform.py`, changes to a pipeline config, and a basic test. Enough to have a real conversation about structure, edge case handling, naming, and design decisions — without overwhelming the reviewer.

---

## Wednesday timeline

| Time | Activity |
| --- | --- |
| **14:30 - 15:00** | Find bugs and open PR |
| **15:00 – 15:30** | Reviewer reads the code independently and leaves written comments (aim for at least 2 meaningful ones) |
| **15:30 – 15:45** | Round 1 - Author and reviewer sit together, walk through each comment, discuss and resolve |
| **15:45 – 16:00** | Round 2 - Author and reviewer sit together, walk through each comment, discuss and resolve |
| **By 16:00** | PR is merged or closed with a short written summary. Done. |

---

## Reviewer checklist

Your written comments should cover some of the following. Not all of them — but each one should be specific and actionable:

- Does the code actually do what the description says?
- Is there a simpler way to get the same result?
- Are functions and variables named clearly?
- Is anything repeated that could be extracted or reused?
- Are edge cases or errors handled?
- What's one thing you'd do differently, and why?

> **The rule that makes prep non-optional:** Every comment you write must be specific enough that you can explain it verbally during the discussion. No vague feedback like "looks good" or "fix this" — each comment needs a clear point you can defend. That means you can't skim and rubber-stamp — you have to read carefully enough to actually have an opinion.

---

*LEVEL3 · Arkadia Heilbronn gGmbH · <level3@arkadia.hn> · level3.hn*
