# Analytical Mock Interview Partner

Written by [jessicahiggs](https://github.com/jessicahiggs).

A Claude skill that runs a live, timed mock **analytical interview** — the metrics round used for
PM roles at most top tech companies. Different companies call it execution, product analysis, or
analytical thinking, but it's the same question: *how would you measure success of this product?*

Claude plays a realistic interviewer: it presents a case, makes you define every bar, and
challenges your North Star against its runner-up — without spoon-feeding you the structure. It
tracks real elapsed time per section against target pacing, and closes with detailed narrative
feedback (no scores or grades — just specific, quotable critique).

## What it looks like

You bring a case (or ask for one), and Claude runs the session as a real interviewer would —
probing, pushing back, and holding you to your choices. A short excerpt (illustrative):

```text
Interviewer: Let's do a case. "How would you measure the success of a
podcast feature inside a video streaming app?" Before any numbers — what
is this product for?

You: It's there to grow engagement and give people a reason to open the
app more often.

Interviewer: That's the goal of every feature. Is this product new or
mature? Because that changes what you'd measure first.

You: New — so I'd lead with adoption rather than depth of engagement.

Interviewer: Good. Who are we measuring?

You: Listeners, and the creators publishing the shows.

Interviewer: You've given me a two-sided ecosystem. Are you measuring both,
or scoping to one?

You: I'd scope to listeners, but I'd still watch creator retention — if
publishers churn, the catalog thins out and listener metrics follow.

Interviewer: Fine. Give me your engagement metric.

You: Weekly active listeners.

Interviewer: That's an adoption metric wearing a different hat. What does
a user have to actually do for you to call them engaged?

  ... [case continues through the metrics table, the North Star,
      and counter-metrics] ...
```

When the case ends, it drops the interviewer persona and gives you an honest read:

```text
Pacing — that took about 29 minutes.

Where it was strong — you caught the new-vs-mature distinction unprompted
and let it shape which metrics you led with. You also volunteered what
you'd watch on the side you weren't measuring, which most candidates skip.

Where it was thin — your metrics didn't trace back to the user value you
established earlier. You listed what's conventional rather than deriving
it from what listeners actually do, which is why "weekly active listeners"
came out with no bar attached.

Highest-leverage fix — your counter-metric was a generic guardrail. Name
the mechanism: how specifically would your North Star rise while the
product got worse? Answer that and the counter-metric writes itself.
```

No scores or grades — just specific, quotable feedback tied to what you actually said.

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

> Mock interview me on this: "How would you measure the success of YouTube Shorts?"

**No case handy?** Ask Claude to give you one — it'll generate a realistic case from a real
company and product area. You can also aim it: name a company, product area, or seniority
("a staff-level case for a fintech app") and it'll tailor the prompt to what you're preparing for.

**How long it takes:** a full case runs about 25–40 minutes, plus a couple of minutes of feedback
at the end — close to a real interview round, so you can practice under realistic pacing.

## License

MIT — see [LICENSE](LICENSE).
