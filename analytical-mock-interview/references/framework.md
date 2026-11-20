# Execution / Analytical Framework

The ordered structure for an analytical (execution / product analysis / metrics) case.
Seven steps. Each step lists what the user must produce and the rules you check their answer
against before moving on.

Trade-off questions ("should we build A or B", "we're considering removing X") are a different
question type and are **not** covered by this framework.

---

## 1. WHY?

Establish what the product is for before measuring anything.

- How does the product align with the company's mission?
- What is the product's own mission statement?
- What problem is the product solving?
- Is the product **new or mature**? New products focus on adoption; mature products focus on
  engagement.

**Check:** did they actually decide new vs. mature? That answer determines what they lead with
in step 4, so it has to be made explicitly, not skipped.

---

## 2. WHO?

Identify the ecosystem, then classify its shape.

- Identify **both sides of the ecosystem**.
- Confirm the shape: **are both sides groups of people, or is one side a system or platform?**
- Shapes you'll see:
  - **Two groups of people** — marketplace, creator/consumer, buyer/seller
  - **People + a system or platform** — AI products, search, ranking. The system side carries
    quality metrics rather than engagement
  - **People + a third party** — advertisers, developers. That side pays or builds rather than
    consumes

**Check:** naming only one side is the most common miss. Both sides get measured by default,
and the next step defines success for each of them.

---

## 3. Define "success" for each side

This step produces the raw material for step 4. **No metrics are named yet.**

- For each side: list the **actions** that side takes.
- For each action: what **value** does it deliver to them?
- For a system or platform side, success is a threshold rather than an action — e.g. "returns an
  accurate answer the user doesn't have to re-prompt."

**Check:** if they start naming metrics here, pull them back. A thin action list produces a
generic metrics table, so push for depth now rather than later.

---

## 4. Metrics table (4-10 metrics)

A matrix, not a list. Rows are metric type; columns are each side of the ecosystem. **Every row
gets filled for both sides.**

|                | Side A | Side B |
|----------------|--------|--------|
| **Adoption**   |        |        |
| **Engagement** |        |        |
| **Retention**  |        |        |

**Adoption** — the **number** of people on each side who complete the core action at least once
per day, week or month. A count, not a percentage. The cadence must be justified: why weekly and
not monthly?

> e.g. *# of people who listen to at least one episode per week* · *# of podcasters who publish
> at least one episode per week*

**Engagement** — **multiple metrics per side**, each with a **defined bar**. What does a person
have to do to count as engaged? Expressed as a count, a percentage of people completing a
defined action, or an average per person.

> e.g. *% of people who listen to 4+ episodes a week* · *% of people who save an episode and come
> back to it* · *% of podcasters who publish 2+ episodes a month*

**Retention** — the **percentage** of people on each side who did it last period and came back to
do it this period.

> e.g. *% of podcasters who published last month and published again this month*

**Rules for this step, in the order people get them wrong:**

1. **A group of people is not a metric.** "Weekly active listeners" names a population. A metric
   is a count or percentage of people completing a defined action.
2. **Adoption is a number; retention is a percentage.** Engagement can be either, plus averages.
3. **One engagement metric per side is not enough.** A single number won't cover how people
   engage with a product.
4. **Both columns, every row.** N/A is valid only when a side is genuinely a system or platform —
   a system doesn't adopt or retain, so that column carries quality metrics instead (accuracy,
   hallucination rate, latency). Never let N/A be used to avoid work on a human side.
5. **Every metric traces back to an action from step 3.** If one doesn't, ask where it came from.

Three metric types across two sides is six cells, which is why the range is 4-10: minus any N/A,
plus room for the extra engagement metrics.

---

## 5. Identify the North Star metric (NSM)

- State it.
- **Justify it — how does everyone in the ecosystem win?**
- Confirm it aligns with the product's goal and mission from step 1.

**Check:** a North Star only one side benefits from is a team metric, not a North Star. Also
check it isn't a raw total that rises on user growth alone — if it is, ask whether a per-person
version says more.

---

## 6. Prioritize 3 metrics

From the table, pick three.

- Prioritize by **type of metric** (usually engagement) and **type of user** (usually the
  consumer side).

**Check:** make them say why those three and not the ones they dropped.

---

## 7. Counter-metrics to the North Star

- What rises while the product gets worse?
- A good counter-metric catches the North Star being gamed, hollow, or won by cannibalizing
  something else of value.

**Check:** a generic guardrail is a weak answer. Make them trace the mechanism — *"how
specifically would your North Star go up while this product got worse?"* The answer to that
question **is** the counter-metric.
