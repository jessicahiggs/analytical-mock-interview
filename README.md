# Analytical Case Walkthrough

Written by [jessicahiggs](https://github.com/jessicahiggs).

A Claude skill that walks you step by step through answering an **analytical case** — the metrics
round used for PM roles at most top tech companies. Different companies call it execution,
product analysis, or analytical thinking, but it's the same question: *how would you measure
success of this product?*

Claude takes you through the case one step at a time. It says what each step needs, lets you
answer it, then checks your answer and tells you what's missing before moving on. The metrics
table builds up in front of you as you go, and at the end you get the finished case back in one
piece.

## What it looks like

A short excerpt (illustrative):

```text
Claude: Next: who's in the ecosystem? And tell me whether both sides
are groups of people, or whether one side is a system or a platform.

You: Listeners and podcasters. Both are people.

Claude: Good — so both columns get filled later.

Before any metrics, define what success looks like for each side. What
does each one actually do, and what do they get out of it?

You: Podcasters record and publish episodes, build a following so people
don't miss the next one, and eventually land sponsors. Listeners find
shows that match their interests, save them for later, listen, and share
episodes with friends.

Claude: Hold onto that list — the metrics come straight out of it.

Now adoption. This is a count: the number of people on each side who do
the core action at least once per period. Both sides, and tell me why
you picked the period you picked.

You: Number of people who listen to at least one episode a week, and
number of podcasters who publish at least one episode a week.

Claude: Both sides, both counts. Why weekly?

You: Episodes mostly drop weekly, so that's the natural cycle for
someone to come back.

Claude: That's the justification I wanted. On to engagement — and this
is where it gets harder, because you need more than one per side.

You: Weekly active listeners.

Claude: That's a group of people, not a metric. A metric is a count or
a percentage of people doing something specific. What does a listener
have to actually do for you to call them engaged?

  ... [continues through the full table, the North Star,
      prioritization, and counter-metrics] ...
```

At the end it prints the finished case back in one piece — purpose, ecosystem, the completed
table, the North Star and its justification, the three prioritized metrics, and the
counter-metrics — plus a short read on how your reasoning went. No scores or grades.

## What this skill is not for

- **Product sense / design cases** ("design a product for X") — use
  [product-sense-mock-interview](https://github.com/jessicahiggs/product-sense-mock-interview)
  instead.
- **Trade-off cases** ("should we ship A or B") — a different question type with its own
  structure. The skill will tell you if your case is one of these.

## Installing

**Claude Code / Claude Agent SDK / Cowork:** drop the `analytical-mock-interview/` folder into
your skills directory (or install the packaged `.skill` file if you have one), then in a
conversation just say something like:

> Walk me through this: "How would you measure the success of YouTube Shorts?"

**No case handy?** Ask Claude for one — it'll generate a realistic case from a real company and
product area. You can also aim it: name a company, product area, or seniority ("a staff-level
case for a fintech app") and it'll tailor the prompt to what you're preparing for.

## License

MIT — see [LICENSE](LICENSE).
