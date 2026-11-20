# Analytical Case Walkthrough

Written by Jessica Higgs.

A Claude skill that walks you step by step through answering an **analytical case** — the metrics
round used for PM roles at most top tech companies. Different companies call it execution,
product analysis, or analytical thinking, but it's the same question: *how would you measure
success of this product?*

It's good preparation for big tech PM loops, where the analytical round is a standard part of the
process.

Claude takes you through the case one step at a time. It says what each step needs, lets you
answer it, then checks your answer and tells you what's missing before moving on. The metrics
table builds up in front of you as you go, and at the end you get the finished case back in one
piece.

## What it holds you to

- A group of people is not a metric — a metric is a count or percentage of people doing something
- Adoption is a number, and you have to justify the cadence you picked
- Every engagement metric needs a defined bar, and one metric per side isn't enough
- Both sides of the ecosystem get measured, not just the obvious one
- Your North Star has to work for everyone in the ecosystem, not one side
- Counter-metrics name a real mechanism, not a generic guardrail

## What this skill is not for

- **Product sense / design cases** ("design a product for X") — use the product sense mock
  interview skill instead.
- **Trade-off cases** ("should we ship A or B") — a different question type with its own
  structure. The skill will tell you if your case is one of these.

## Installing

**Claude Code / Claude Agent SDK / Cowork:** drop the `analytical-mock-interview/` folder into
your skills directory (or install the packaged `.skill` file if you have one), then in a
conversation just say something like:

> Walk me through this: "How would you measure the success of YouTube Shorts?"

**No case handy?** Ask Claude for one — it'll generate a realistic case from a real company and
product area.

## License

MIT — see [LICENSE](LICENSE).
