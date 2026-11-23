# Porter · First-Trip Conversion

### Porter asks you to pick the truck before it asks what you are moving.

> **TL;DR:** Porter's first-trip completion is 41%; the brief asked for 58% in six months. Research across 42 users, two live bookings walked screen by screen, and 30 complaints showed that **labour expectations, not the vehicle, decide whether a first trip succeeds.** The fix is to ask what you're moving first, price the whole trip (including who carries it) up front, and give a trip in trouble a way to recover instead of only a cancellation form. Most of it is **relocating things Porter already owns, not building new ones.**

| | |
|---|---|
| **Type** | Product teardown, research, solution, PRD, GTM and metrics |
| **Company** | Porter (intra-city logistics) |
| **Goal** | First-trip completion **41% → 58%** in six months |
| **Deliverables** | [🎥 video walkthrough](https://www.loom.com/share/a3b9888cce0c4a06bc410b8eb469dc0a) · 17-slide deck · [prototype](#prototype) with 24 design notes · PRD, research, GTM, metrics and risks documents |
| **Methods** | User survey and calls · live-app teardown · complaint analysis · RICE · North Star and guardrails |
| **Skills shown** | User research · product teardown · problem framing · solution design · prioritisation · PRD · prototyping · metrics and guardrails · GTM and sequencing · hypothesis testing · presenting (video walkthrough) |

### 🎥 Video walkthrough

<a href="https://www.loom.com/share/a3b9888cce0c4a06bc410b8eb469dc0a"><img src="https://img.shields.io/badge/▶%20Watch%20the%20walkthrough-Loom-625DF5?style=for-the-badge&logo=loom&logoColor=white" alt="Watch the walkthrough on Loom"/></a>

<sub>Correction at 3:29: 88% had a clean first trip when labour went as expected, 56% when it broke.</sub>

---

## 1. The brief

**North Star:** first-time individual users who enter pickup and drop, reach the vehicle-selection screen, and complete a trip within 7 days.

| Today | Target | What it means |
|---|---|---|
| **41%** | **58%** in 6 months | **17 in every 59** of today's non-completers must complete instead (28.8%) |

The brief names four ways a first trip is lost: **abandonment, cancellation, rebooking, and going back to an offline option.**

---

## 2. The problem: too early, and no way back

- **Too early:** the vehicle, price and labour are all committed *before* the answers that should inform them arrive.
- **No way back:** a live trip has two controls, and both end at the same nine-reason cancellation form.

The brief calls it judgment a first-timer has not built yet. In the product, it is **the order of the questions.**

| The question a first-timer has | When Porter answers it |
|---|---|
| What does my load weigh? | After the vehicle is chosen |
| Which vehicle takes it? | Never. It shows a number and leaves the maths to you |
| Who carries each item? | Never, anywhere in the app |
| What does the price cover? | After the fare is set |
| Is any of it restricted? | After the vehicle is chosen |
| What if it goes wrong? | Nine reasons, one cancellation form |

---

## 3. Research: three sources

| | |
|---|---|
| **42 user responses** | 23 of them followed by a phone call, across five cities |
| **2 bookings walked** | Screen by screen on the live app, 16 figures |
| **30 complaints read** | Plus Porter's published terms and the offline alternatives |

The teardown is first-party: anyone who opens Porter today sees the same thing. The survey explains *why*, and Porter's own event data would supply the rates.

---

## 4. The key finding: labour decides the first trip

| Labour expectation | Clean first trip |
|---|---|
| ✅ Went as expected (n = 25) | **88%** |
| ❌ Broke (n = 9) | **56%** |

- Only **1 person in 42** raised the vehicle as the issue. **None of the 30 complaints** mention it.
- **5 of the 6** who entered the funnel without a clean trip had a labour expectation or mismatch.
- Every offline alternative prices labour explicitly, at **₹400–800 per person.** Porter alone says nothing about it.

### Why it happens: the vehicle is asked for first

`Stage 4: vehicle chosen and priced` → `Stage 5: goods declared, weight pre-filled` → `Review: terms appear, fare already set`

It starts on the home screen, where the tiles are *Trucks, 2 Wheeler and Packers & Movers*: two vehicle classes and a service. A 2 Wheeler then opens a 19-category freight list, and House Shifting opens a room picker. **What you're moving can't inform the vehicle choice, because the vehicle choice decides which question you get asked about it.**

### Porter already owns the fix

| What a first-timer needs | Where Porter already has it | On-demand? |
|---|---|---|
| A room-by-room item picker | The House Shifting wizard | No |
| A vehicle that comes with labour | Mini truck with 2 labour, within city | No |
| A class rated for a household | Tata Ace, 750 kg, on porter.in | No |
| A weight that tests the load | The goods step captures one | Only after the vehicle |
| A catalogue of its own failures | Nine cancellation reasons | Only as exits |

**That's why the plan is cheap: four of the six booking-side changes move things that already exist rather than build new ones.**

---

## 5. The solution: one on each side of booking

### 1 · Before booking: six changes, no new screen
Porter asks **what you're moving first**, then answers it: the class your weight allows, who carries it, whether stairs are covered, and the whole price.

| # | What changes | Evidence |
|---|---|---|
| S6 | Home screen asks what you're moving; goods come before the vehicle | Today the vehicle decides which goods list you see |
| S4 | Every card says: you load and unload, stairs not included | 27 of 42 assumed loading was covered |
| S11 | Load Assist on the card, priced, with its limits | 7 of 42 bought labour elsewhere |
| S17 | Which floor, and is there a lift? | 20 of 42 assumed stairs were covered |
| S5 | The three charges that can change the fare | 8 of 30 complaints |
| S1 | Each class marked against the declared weight | The 2 Wheeler is rated for 20 kg |

S4, S11 and S17 arrive as **one configuration**, not three labels.

### 2 · After booking: a ladder, not a cancellation form

| Today | After |
|---|---|
| Nine reasons, all leading to the same cancellation form | A person in one tap, before any reason is picked |
| The support bot answers "driver unreachable" with a route to cancelling | The call is placed for you |
| | Still no answer? It asks: assign another driver, or hold two minutes |
| | The fare is held throughout |
| | Load Assist that was paid for but not provided is refunded |

Only one option should end a trip: **"changed my mind."** Every other path leads to a completed trip.

> In the brief's own words, Porter gets easier when it helps a first-timer *correctly configure the trip* and *trust the service can actually complete the job*. One solution for each. Neither reaches 58% alone.

### Prototype
1. **What are you moving:** parcel or household goods, then Porter's own list and which floor
2. **Select vehicle:** the class your weight allows, who carries it, and the whole price
3. **Something's wrong:** a person in one tap, then a ladder of steps through to the completed trip
---

## 6. Does it answer the brief?

| Failure mode | Why it happens today | What answers it |
|---|---|---|
| **Abandonment** | Vehicle, price and labour committed before the answers arrive | Goods first, then the whole trip priced |
| **Cancellation** | Nine failure reasons, one cancellation form | A ladder: call, ask, fare held |
| **Rebooking** | A vehicle too small, discovered at the kerb | Weight checked before booking |
| **Back to offline** | The tempo quote prices two people and stairs; Porter never said it excludes both | Load Assist stated and priced |

---

## 7. Prioritisation: RICE across 15 ideas

*Reach per 1,000 users at the vehicle screen · Impact 0.5–3 · Confidence from the evidence · Effort in person-months · Score = R × I × C ÷ E*

| # | Idea | Reach | Impact | Conf. | Effort | Score | Ships |
|---|---|---|---|---|---|---|---|
| 1 | S5 · Terms on the vehicle screen | 1,000 | 2.0 | 0.85 | 0.5 | **3,400** | Wave 1 |
| 2 | S4 · State who lifts and carries | 643 | 2.0 | 0.95 | 1.0 | **1,222** | Wave 1 |
| 3 | S17 · Which floor, is there a lift | 476 | 1.5 | 0.70 | 0.5 | **1,000** | Wave 1 |
| 4 | S1 · Weight check before the vehicle | 1,000 | 2.0 | 0.75 | 2.0 | **750** | Wave 1, gated |
| 5 | S11 · Load Assist, priced, on the card | 643 | 2.0 | 0.85 | 2.0 | **547** | Wave 1 |
| 6 | S3 · Dimensions on every card | 1,000 | 1.0 | 0.25 | 0.5 | 500 | ❌ Cut |
| 13 | S8 · Help that resolves, not cancels | 300 | 3.0 | 0.85 | 5.0 | 153 | Wave 1, argued |

**Judgement over the formula:** S3 scores 500 and is **cut**, because S1 answers the same question. S8 scores only 153 and **ships**, because RICE prices reach and effort, never the cost of the alternative.

---

## 8. Metrics: one North Star, eight guardrails

**North Star:** first-time individual users who enter pickup and drop, reach the vehicle-selection screen, and complete a trip within 7 days. **41% today → 58% in six months.**

| Must not rise | Must not fall, or must stay at zero |
|---|---|
| Cancellation after assignment | Repeat booking within 90 days |
| Rebooking within 24 hours | Overload warnings overridden (under half) |
| Fare disputes per 1,000 trips | Load Assist bought and not delivered (zero) |
| Driver cancellation at pickup | |
| App open to booking confirmed | |

**30 events specified.** The holdback group gives the real rates at week 9 and the headline result at week 20.

---

## 9. Sequencing: three waves, each one gated

| Wave | What it does | Cost | Gate to start |
|---|---|---|---|
| **1: Complete the booking, rescue the trip** | Both solutions, shipped together | 20 person-months | Two queries in Porter's data. They decide its shape, not whether it ships |
| **2: Remove the guesswork that remains** | Free re-send on a wrong vehicle; saved draft | 8 person-months | Vehicle changed at pickup has not fallen |
| **3: Make the trip repeatable** | Porter remembers the configuration | 3 person-months | First-trip completion has moved |

**41% → 50%** after Wave 1 is a planning figure, replaced by a measured one at week 9. **If it moves under 5 points, Waves 2 and 3 are dropped.**

---

## 10. What would prove this wrong

Two queries in Porter's own data:

- **If vehicle changed at pickup is near zero:** the weight check isn't needed, which is why it's already gated. The goods step shrinks to the reordering change, which works on its own.
- **If service-failure cancellation reasons are rare:** the rescue path is expensive insurance and Solution 1 waits. Only Porter can see that reach number.

---

> **Porter does not need to build a first-trip experience. It needs to move the one it already has.**

📄 The full deck and supporting documents (research, evidence tracker, product teardown, journey map, PRD, GTM, metrics, risks) are available on request.

⬅️ [Back to portfolio](../README.md)
