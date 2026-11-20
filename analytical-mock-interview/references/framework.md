# Execution / Analytical Framework

The ordered structure for an analytical (execution / product analysis / metrics) case.
Seven steps. Each step lists what the candidate must produce and the sub-questions used to
pressure-test them.

Trade-off questions ("should we build A or B", "we're considering removing X") are a different
question type and are **not** covered by this framework. If a case is a trade-off, say so and
run it separately.

---

## 1. WHY?

The candidate must establish what the product is for before measuring anything.

- How does the product align with the company's mission?
- What is the product's own mission statement?
- What problem is the product solving?
- Is the product **new or mature**? New products focus on adoption; mature products focus on
  engagement. This answer should visibly shape the metric set in step 4.

**Pressure-test:** light touch here. Check that motivation is anchored to the company mission and
that new-vs-mature was actually decided. Don't cross-examine competitors or risk — that belongs
to a product sense case, not this one.

---

## 2. WHO?

The signal is that the candidate saw the **whole ecosystem**, not that they measured all of it.

- Identify the full ecosystem, naming both sides even if only one will be measured.
- Classify the shape:
  - **Two user groups** — marketplace, creator/consumer, buyer/seller
  - **User + system** — AI products, search, ranking. The second side's metrics are quality, not
    engagement
  - **User + third party** — advertisers, developers. The second side pays or builds rather than
    consumes
- The candidate should ask the interviewer to confirm scope:
  *"Who's on each side — two user groups, or a user and the system serving them?"*
- If scoping to one side, they must say which, why, and what they would still watch on the other.

**Pressure-test:** a candidate who scopes to one side without naming the other has missed the
ecosystem. A marketplace metric set that ignores supply health looks complete and isn't. Ask:
"what would you watch on the side you're not measuring?"

---

## 3. Define "success" for each side

This step produces the raw material for step 4. **No metrics are named yet.**

- For each side of the ecosystem: list the **actions** that user takes.
- For each action: what **value** does it deliver to them?
- For a system side, success is a threshold rather than an action — e.g. "returns an accurate
  answer the user doesn't have to re-prompt."

**Pressure-test:** if the candidate starts naming metrics here, pull them back — the metrics in
step 4 must be measurements of the actions listed here, not pulled off a generic list. If their
action list is thin, step 4 will be generic, so push for depth now.

---

## 4. Metrics table (4-10 metrics)

A matrix, not a list. Rows are metric type; columns are each side of the ecosystem.

|                 | Side A | Side B |
|-----------------|--------|--------|
| **Adoption**    |        |        |
| **Engagement**  |        |        |
| **Retention**   |        |        |

- **Adoption** — number of people using the product (daily / weekly / monthly)
- **Engagement** — requires a **defined bar**: what action must a user complete to count as
  engaged? Expressed as % of users completing that action, or average level of actions per user.
  Never a raw count with no bar.
- **Retention** — what % of users who used the product last period used it again this period?

**N/A is valid, conditionally.** When a side is a *system*, adoption and retention don't apply —
a system doesn't adopt or retain. That column carries quality metrics instead (accuracy,
hallucination rate, latency, relevancy). This only applies when a side is genuinely a system; do
not let a candidate mark N/A to avoid work on a human side.

Three metric types across two sides is six cells, which is why the range is 4-10: minus any N/A,
plus room for a second metric where one number doesn't cover the behavior.

**Pressure-test:** this is the heaviest step and where candidates get stuck. Check that every
metric traces back to an action from step 3, that the engagement bar is explicitly defined, and
that new-vs-mature from step 1 is reflected in which metrics they lead with.

---

## 5. Identify the North Star metric (NSM)

- State it.
- **Justify it** — how does everyone in the ecosystem win?
- Confirm how it **aligns with the goal and mission** of the product established in step 1.

**Pressure-test:** ask them to defend it against the runner-up. A NSM that only one side of the
ecosystem wins on isn't a North Star, it's a team metric.

---

## 6. Prioritize 3 metrics

From the table, pick three.

- Prioritize by **type of metric** (usually engagement) and **type of user** (normally the
  consumer side).

**Pressure-test:** ask why those three and not the others. Make them commit.

---

## 7. Counter-metrics to the North Star

- Identify what could go up while the North Star goes up, and signal that something has gone
  wrong.
- A good counter-metric catches the NSM being gamed, hollow, or won by cannibalizing something
  else of value.

**Pressure-test:** this is the step that separates strong candidates. If they offer a generic
guardrail, ask: "how specifically would my North Star rise while the product got worse?" The
answer to that question *is* the counter-metric.

---

## Timing (default 40-minute session)

| Section                  | Target |
|--------------------------|--------|
| Intro + case prompt      | 2 min  |
| 1. Why                   | 4 min  |
| 2. Who                   | 4 min  |
| 3. Define success        | 6 min  |
| 4. Metrics table         | 10 min |
| 5. North Star            | 5 min  |
| 6. Prioritize 3          | 4 min  |
| 7. Counter-metrics       | 5 min  |
| **Total**                | 40 min |

Scale proportionally for a different session length.
