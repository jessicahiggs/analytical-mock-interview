# Analytical Mock Interview Partner

Written by Jessica Higgs.

A Claude skill that runs a live, timed mock **analytical interview** — the metrics round used for
PM roles at most top tech companies. Different companies call it execution, product analysis, or
analytical thinking, but it's the same question: *how would you measure success of this product?*

It's good preparation for big tech PM loops, where the analytical round is a standard part of the
process.

Claude plays a realistic interviewer: it presents a case, asks probing questions, makes you
define every bar, and challenges your North Star against its runner-up. You bring your own
approach — the skill doesn't hand you a structure, the same way a real interview doesn't.

It tracks real elapsed time against target pacing and closes with narrative feedback: what you
actually said, where it was thin, and the single highest-leverage thing to fix next time. No
scores, no grades.

## What it tests

- Whether your metrics trace back to real user value, or were named off a generic list
- Whether you defined the bar for every metric you proposed
- Whether your North Star works for the whole ecosystem, not just one side
- Whether your counter-metrics name a real mechanism, not a generic guardrail

## What this skill is not for

- **Product sense / design cases** ("design a product for X") — use the product sense mock
  interview skill instead.
- **Trade-off cases** ("should we ship A or B") — a different question type with its own
  structure. The skill will tell you if your case is one of these.

## Installing

**Claude Code / Claude Agent SDK / Cowork:** drop the `analytical-mock-interview/` folder into
your skills directory (or install the packaged `.skill` file if you have one), then in a
conversation just say something like:

> Mock interview me on this: "How would you measure the success of YouTube Shorts?"

**No case handy?** Ask Claude to give you one — it'll generate a realistic case from a real
company and product area.

## License

MIT — see [LICENSE](LICENSE).
