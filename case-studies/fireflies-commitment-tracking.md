# Fireflies.ai · From Meeting Notes to Closed Commitments

### A promise made in a meeting is captured, but owned by no one.

> **TL;DR:** Fireflies captures commitments from meetings well, but only **28%** are resolved within 14 days; the brief's target is **45%**. Research across 31 people, 17 phone interviews and a test meeting with 10 planted commitments showed that **extraction works; ownership doesn't.** Nobody is ever asked *"is this yours?"* The proposal: **claim once, then Fireflies follows the work.** A one-tap *Mine* creates the owner and an already-assigned ticket, status syncs two-way across Jira, Asana and Slack, and an AI closure engine checks the next meeting for anything still open. I built a working prototype and tested it with 5 users.

| | |
|---|---|
| **Type** | AI product case study: research, problem framing, PRD, prototype, GTM, metrics and risks |
| **Company** | Fireflies.ai (AI meeting assistant) |
| **Goal** | 14-day commitment resolution **28% → 45%** in six months |
| **Deliverables** | 21-slide deck · [working prototype](#working-prototype-one-tap-creates-the-owner-and-the-ticket) · [AI closure engine](#the-ai-piece-a-closure-engine-so-the-next-meeting-closes-whats-still-open) · [product teardown](#the-teardown-following-one-promise-from-spoken-to-day-14) · 8 full documents, PRD included |
| **Methods** | Survey · phone interviews · planted-commitment teardown · competitive scan of 8 AI tools · RICE · OKRs · risk matrix · cohort rollout |
| **Skills shown** | AI product strategy · AI for product management · user research · competitive analysis · problem framing · prioritisation · PRD · prototyping · metrics and OKRs · stakeholder mapping · GTM · business modelling · risk management |

| 31 | 17 | 10 | 8 | 15 | 5 | 14 |
|---|---|---|---|---|---|---|
| people surveyed | phone interviews | planted commitments | AI tools compared | ideas scored | prototype testers | sync scenarios tested |

---

## 1. The problem

I said *"I'll fix the payment bug by Wednesday."* Fireflies captured it perfectly and sent it to everyone in the recap. **Nobody was asked "is this yours?"** Sent to everyone, it belongs to no one.

| Today | Target |
|---|---|
| **28%** resolved within 14 days | **45%** in six months |

**Resolved** means done, reassigned, or deliberately dropped. Silently ignored or raised again doesn't count.

---

## 2. Research: six methods, covering both sides of a promise

- **31 surveyed** via LinkedIn (128 reached, a 24% response rate)
- **17 phone interviews**
- **10 planted commitments** in a test meeting, followed through Fireflies, Slack and Jira
- **8 AI meeting tools + 5 everyday methods** compared
- **4 stakeholder roles** mapped: user, manager, admin and buyer
- **5 hypotheses** tested

### Findings: promises live in private notes, and slip by being re-dated rather than dropped

- **Notebooks beat trackers 17 to 10** as the place people note action items, so most promises never reach a tool.
- **People report closing 79%** (42 of 53 promises), and 21 of 31 say promises "usually get done." Yet the person waiting often can't see it.
- **Surveys say "I'd tell them." Real stories show re-dating.** In interviews, 6 of 17 moved a promise to a later date; none described saying "I am not doing this."
- **Visibility is acceptable:** 25 of 30 were neutral or comfortable with a manager seeing pending promises.

> *"Ticket got breached as it was not tracked anywhere in the meeting."* P7, manager
>
> *"Clients often promise to give the details … many at times, they forget."* P13, assistant project manager

### The teardown: following one promise from spoken to day 14

| When | What happens | Where it's lost |
|---|---|---|
| Within the hour | Recap email and Slack summary go to everyone | **1.** Nobody is asked "is this yours?" |
| Same day | Jira tickets created, with noise and duplicates | **2.** Every ticket arrives unassigned |
| Same day | Owner notes it privately | **3.** The person waiting can't see it |
| Days 2–13 | Done, moved or forgotten | **4.** A new date or a drop has nowhere to go |
| Day 14 | Done in Jira, still open in Fireflies | **5.** Closure doesn't travel, so it isn't counted |

**Extraction works:** Fireflies caught 7 of the 8 open commitments. What breaks is everything after it.

### Competition: some tools ask for acceptance; none carries closure across tools

| | Owner says yes | Travels across tools | Drop is a real ending |
|---|---|---|---|
| Fireflies today | ❌ Nobody is asked | ❌ One-way push to Jira | ❌ Tick or delete only |
| Zoom, Microsoft Teams | 🟡 Zoom yes, Teams partly | 🟡 Inside their own suite | ❌ |
| Jira, Asana | ✅ As assignee | ❌ Own tool only | 🟡 "Won't Do" |
| Slack, standups | 🟡 Informally | ❌ | ❌ |
| **Fireflies with this proposal** | ✅ **Mine, on any platform** | ✅ **Jira, Asana, Slack, two-way** | ✅ **One of three endings** |

Fireflies already sits across Zoom, Teams and Meet, so it is best placed to carry one status everywhere.

---

## 3. The primary barrier: no moment of acceptance

Forgotten, quietly re-dated, repeated, unassigned, out of sync: **these are all symptoms.** The one cause is that nobody is asked "is this yours?", so there's no one to close it and no one for Fireflies to ask.

**The tension:** the person who promised wants autonomy, and the person waiting wants visibility. So **ownership is chosen, never assigned,** and only seen at team level.

---

## 4. How 28% becomes 45%: acceptance does the work

Out of every 100 commitments heard in a meeting:

| | Share | Close rate | Closed |
|---|---|---|---|
| Accepted by an owner | 55 | 60% | **33** |
| Not accepted | 45 | today's 28% | **12.6** |
| **Total** | | | **45.6%** ✅ vs the 45% target |

- **75% ceiling:** in the test meeting, the owner was present for 6 of 8 open commitments.
- **33% floor:** even if accepted promises closed at the best case of 79%, acceptance must reach 17 ÷ (79 − 28) = **33%.**
- **55% accepted** is the midpoint of the floor and the ceiling. **60% close** is the rate then needed to hit 45%.
- **Split by team type:** teams with tools reach 50.2% and teams without reach 39.0%, so the blend is 44.0%. Adding "Open from last time" lifts the no-tool teams, and the blend reaches **45.4%.**

---

## 5. Prioritisation: why these two

RICE across 15 ideas, with every reach number taken from the research.

| Idea | Score | Decision |
|---|---|---|
| **1 · Claim it where you see it** | **36.0** (1st) | ✅ **Chosen.** Nothing closes without an owner, and today nobody is asked |
| Three endings on the commitment | 29.3 | Ships alongside, for the 17 of 31 with no tracker or Slack |
| Slack message updates in place | 23.2 | Part of the same sync |
| "Before you go" card | 22.5 | Later. It asks for action when attention is lowest (50% confidence) |
| Acceptance by action | 22.5 | Later, to widen the claim step |
| **2 · Status follows the work** | **21.6** (6th) | ✅ **Chosen.** The only closing idea that asks nothing extra of the owner |

**Judgement over the ranking:** RICE scores ideas on their own; I chose the two that **together** fix the cause: no owner, and closure that doesn't travel.

**Trade-offs made explicit:**
- **Accountability vs autonomy:** ownership is chosen, never assigned. I give up coverage (an unclaimed item stays unowned) to keep consent.
- **Automation vs control:** ask at the start (whose is it?), automate at the end (copy a status the owner already set).

---

## 6. The solution: claim once, then Fireflies follows the work

`1 · Spoken and extracted (as today)` → **`2 · Claim: Mine or Not mine, in Fireflies, Slack or email`** → `3 · Ticket created, already assigned` → **`4 · End anywhere: Done, Hand off or Drop`** → `5 · Counted: every tool agrees`

- **How ownership is set:** nothing is yours until you tap *Mine*. *Not mine* returns it to the room. Fireflies never assigns anyone.
- **How a drop is handled:** a drop counts as resolved, and "Won't Do" in Jira means dropped. A new date keeps it open; it isn't an ending.
- **When Fireflies acts alone and when it asks:** it acts alone only to copy a status a person already set. It asks whose it is, and whether it's real.

### Working prototype: one tap creates the owner and the ticket

Four tabs: the Fireflies meeting page, the Slack thread (each owner asked once, with the message updating in place), a recap email for someone with no account, and Jira (tickets arrive already assigned). **Tested with 5 people across roles; every flow worked.**
### The AI piece: a closure engine, so the next meeting closes what's still open

- **AI at the next meeting:** *"The fix went out on Tuesday"* is matched to last week's open commitment. Only matches at **0.70 confidence or above** reach the owner, as one question: *Confirm* or *Not this*.
- **Sync engine:** linked ticket ID, events both ways, its own echoes ignored, latest change wins, status group not name, and a periodic check for lost events.
- **14 scenarios tested, all as designed. It never closes anything without the owner.**
---

## 7. Metrics: North Star, OKRs and guardrails

**North Star:** commitments resolved by day 14 ÷ all commitments extracted. **28% → 45%.** Reopened ones don't count, and "Not a commitment" stays in the total.

| Key result | Target |
|---|---|
| Clear owner within 24 hours | **55%** (gate: 33% in cohort 1) |
| Accepted commitments resolved | **60%** |
| Median time to resolution | **7 days or fewer** |
| Status agreement with linked tickets | **99%** |
| Resolutions that arrive by sync | **Half or more** |

**Guardrails:** "Needs an owner" under 25% · comfort with team-level visibility at 83% or more · raised again under 10% · no more than 1 extra message per person per week versus matched teams · **commitment text never sent to analytics.** 17 events specified.

---

## 8. Rollout: 26 weeks, build included; each cohort earns the next

| Weeks | Stage | Gate to continue |
|---|---|---|
| 1–7 | Build, then our own teams (25 person-weeks, 4 engineers) | 99% status agreement; no added scheduled message |
| 8–13 | Cohort 1: 50 teams, plus 50 matched teams | Acceptance **≥ 33%** (the floor) |
| 14–18 | Cohort 2: 500 teams, incl. 100 with no tools | Resolution **≥ 38%** |
| 19–22 | Cohort 3: all connected paid teams | Resolution **45%** |
| 23–26 | Cohort 4: everyone else | Acceptance above 33% |

**Pause if** messages per person per week rise more than 1 above matched teams, or "Not a commitment" passes 25%.

---

## 9. Business impact: per 1,000 paid seats, 65 extra seats and $7,800 a year

| Case | Seats | Revenue a year | Uplift |
|---|---|---|---|
| Low | 24 | $2,880 | +2.4% |
| **Plan** | **65** | **$7,800** | **+6.5%** |
| High | 150 | $18,000 | +15% |

- **Retention, 40 seats:** small-business software keeps 70–82 of every 100 dollars; I assume this keeps about 4 more points.
- **Expansion, 25 seats:** 4 people per team without a seat × 55% tap *Mine* × 30% create an account × 15% pay = 0.10 seats per team × 250 teams.

---

## 10. Risks: the biggest one is not technical

| Risk | Score (likelihood × impact) | Mitigation |
|---|---|---|
| **Teams with no tools don't close** (17 of 31 people) | **9** | Three endings, plus "Open from last time" at the next meeting |
| People don't claim | 6 | 50 teams first; the 33% gate decides before scaling |
| Wrong or noisy extraction | 6 | Nothing is yours until you tap; "Not a commitment" removes it |

> **Fireflies holds the promise. The tracker holds the plan.** We won't build a task board, individual dashboards, automatic assignment or reminder chains.

---

## 11. The ask

**Build claim and sync for 50 teams, and let the 33% gate decide.**

- **Asking for:** 7 weeks and 4 engineers for *Mine* / *Not mine*, three endings, and the Jira, Asana and Slack sync.
- **Known by week 13:** whether real teams accept at least 33% of commitments, against matched teams without the feature.
- **Not yet proven:** real-use acceptance. Evidence so far: 31 surveyed, 17 interviewed, 5 prototype users.

---

📄 The full deck, supporting artifacts pack and 8 documents (research, problem framing, prioritisation, PRD, growth and business impact, metrics, risks, closure engine) are available on request.

⬅️ [Back to portfolio](../README.md)
