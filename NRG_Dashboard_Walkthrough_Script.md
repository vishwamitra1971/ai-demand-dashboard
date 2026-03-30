# AI Demand Dashboard — Presenter Script
### NRG Internal Walkthrough · Q1 2026
**Estimated runtime: 20–25 minutes**
*Italics = what's on screen. [Pause] = hold for questions/reaction.*

---

## SECTION 1 — Opening (2 min)
*Screen: Password gate → enter → dashboard header loads*

---

"Before I walk you through the mechanics, let me tell you why we built this.

NRG is making 10-to-25-year infrastructure commitments in a technology that is moving on an 18-month cycle. The standard approach — reading analyst reports, tracking NVIDIA earnings, watching hyperscaler capex announcements — gives you a rear-view mirror picture. By the time consensus forms around a demand view, you've either already committed or you've missed the window.

What this dashboard tries to do is something different. It asks: **what are the leading signals, sourced directly from primary data, that would tell you *before* consensus which direction AI energy demand is heading by 2030?**

We track 12 indicators, organized into three categories — Technology Efficiency, Market Behavior, and Adoption Patterns. But more importantly, we've built a scenario framework on top of those indicators so that every data point is interpreted in context. The numbers don't just sit there. They map to a thesis about what the world looks like in 2030 and what NRG should do about it.

Let me start at the top."

---

## SECTION 2 — The Scenario Framework (6 min)
*Screen: Scroll to the three scenario cards*

---

"There are three plausible worlds we could be in by 2030.

**Scenario A — 'Efficiency Wins' — currently 15% probability.**

*[Point to the Scenario A card, blue border]*

The thesis here is that AI hardware and software are getting so efficient so fast that demand plateaus. Think of it this way: if every generation of NVIDIA chips does twice the work at the same power draw, and every software optimization halves the compute needed for the same task, you can theoretically get 10× more AI capability from the same amount of electricity. If adoption doesn't keep pace — if people don't find 10× more things to do with AI — total energy demand actually flattens or falls.

The 2030 endpoint in this scenario is 500 to 600 terawatt-hours of US data center demand. For context, that's roughly double where we are today but it grows at a decelerating 15% CAGR. For NRG, this is the scenario where contracts face early termination pressure and some of the Phase 3 build program needs to stop.

**Scenario C — 'Jevons Dominates' — also currently 15% probability.**

*[Point to Scenario C card, red border — note the pulsing alert badge]*

The polar opposite. Efficiency gains are real, but every time AI gets cheaper, people find dramatically more things to do with it. AI agents proliferate, autonomous systems create persistent baseload demand, every application embeds AI inference. The rebound effect is explosive — over 200% — meaning every efficiency gain generates more than double the new demand.

The 2030 endpoint here is 1,100 to 1,500 terawatt-hours. That is roughly 25 to 30 percent of current total US electricity generation. For NRG, this is the scenario where scarcity pricing on generation is viable, $100+ per megawatt-hour contracts make sense, and the constraint on growth is physical — grid capacity, permitting, gas supply — not demand.

**Scenario B — 'Balanced Growth' — 70% probability. Our base case.**

*[Point to Scenario B card, green border, 'Base Case' badge]*

The moderate path. Efficiency and adoption grow in parallel. The rebound effect is real but not explosive — roughly 100 to 130 percent — meaning every efficiency gain is roughly absorbed by proportional new demand. Energy demand grows 20% per year through 2028, then decelerates to 10 to 15% through 2030.

The 2030 endpoint is 750 to 900 terawatt-hours, with our base model at 820. This is the scenario where NRG's phased buildout executes on schedule, contracted pipeline delivers, and market share — not market size — is what determines winners.

[Pause]

Now here's something I want you to notice before we go any further."

*[Point to the trigger count section on all three cards]*

"All three scenarios have their trigger thresholds simultaneously met.

Scenario A needs 2 or more triggers firing. It has 2 of 6. Scenario C needs 3 or more. It has 4 of 7.

This is not a dashboard error. This is actually the most important single insight from the data: **we are living in a moment of genuine bifurcation.** Efficiency signals are pointing toward A. Demand signals are pointing toward C. And Scenario B is what you get when both are true at the same time and roughly cancel each other out.

The question I want you to hold as we go through the data is: which set of signals is accelerating faster? That answer determines whether we should be accelerating Phase 3 builds or pumping the brakes."

[Pause — take questions on the scenario framework before continuing]

---

## SECTION 3 — The Jevons Rebound Rate (4 min)
*Screen: Scroll down to the gold-bordered Jevons panel*

---

"This panel is the analytical center of the entire dashboard. I want to spend a few minutes here because it answers the question I just asked.

William Stanley Jevons observed in 1865 that as steam engines became more fuel-efficient, Britain's total coal consumption went up, not down. Cheaper energy enabled more uses of energy than anyone anticipated. That dynamic — efficiency gains stimulating demand faster than they suppress it — is called the Jevons rebound effect.

The Jevons rebound rate is the single number that determines which of our three scenarios wins.

*[Point to the large '~115%' metric]*

A rebound rate below 50% means efficiency is winning — Scenario A. 100 to 130% means they're roughly in balance — Scenario B. Above 200% means adoption is exploding past efficiency — Scenario C.

We are currently tracking at approximately 115% in the energy frame. Let me explain what that means concretely.

*[Point to the Energy Frame box on the right]*

AI hardware efficiency is improving roughly 30 to 40 percent per year — that's the H100 to B200 to Rubin trajectory on NVIDIA's roadmap. Simultaneously, total US data center electricity consumption is growing about 25 to 30 percent per year according to the EIA and Lawrence Berkeley National Laboratory. When you divide those two numbers, you get a rebound rate slightly above 100 percent.

In plain English: every watt we save through better hardware is being consumed by increased adoption — and then a little more on top. We are not saving electricity from smarter chips. We are using every bit of it plus some.

*[Point to the Token Frame box]*

Now look at the token frame. In pure computing terms — tokens processed versus price per token — the rebound is closer to 300 percent. Every time inference gets cheaper, people use it far more than proportionally. This is why the Scenario C demand signals are firing so loudly even though hardware is genuinely getting more efficient.

The energy frame is what matters for NRG because we sell electrons, not tokens. And in the energy frame, we're at 115% — firmly in Scenario B territory, but with a slow upward drift that is worth watching.

*[Point to the 12-month trend chart — now with zoomed axis]*

You can see that drift here. The axis is zoomed to 45 to 155 percent so you can actually see the month-to-month movement. The shaded green band is the Scenario B sweet spot — 100 to 130 percent. The rebound rate has been inside that band all year but has been gradually creeping upward. It touched 126 in February before pulling back to 115 in March.

**The probability of any scenario shifting meaningfully starts here. If this line exits the green band and stays outside it for two or more quarters, that is the signal to revisit the scenario probabilities.**"

[Pause — take questions on Jevons before continuing]

---

## SECTION 4 — Technology Efficiency Indicators (3 min)
*Screen: Scroll to the Technology Efficiency section*

---

"These four indicators measure the supply side of the Jevons equation — how fast efficiency is improving and whether that efficiency is being captured at the edge or requiring centralized compute.

*[T1: GPU Performance-per-Watt]*

The hardware trajectory is real and steep. We went from 1.6 teraflops per watt on the A100 in 2020 to 9.0 on the B200 in 2025 — roughly a 30 to 40 percent per year improvement rate. The Rubin generation expected in 2026 is projected to push this further. This indicator is borderline A/B — efficiency is strong but not yet so dominant that it's suppressing net demand.

*[T2: Training Cost Benchmarks]*

This one is counterintuitive and worth pausing on. Frontier training costs are going UP, not down — we're estimating Grok 4 at $500 million for a single training run, up 2.4x year over year. This signals Scenario C at the frontier. But commodity inference costs are collapsing. The key insight: don't confuse frontier R&D costs with deployment costs. They're moving in opposite directions.

*[T3: Inference API Pricing]*

This is one of the most dramatic data series in the dashboard. GPT-4 equivalent inference has fallen 280 times in price since November 2022 — from roughly $60 per million tokens to $0.40 today. The Scenario A trigger for this indicator requires that price decline without proportional volume growth. The evidence shows volume IS growing proportionally. This is pure Jevons — the price collapse is enabling a volume explosion, not a demand plateau.

*[T4: Edge AI Device Volumes]*

370 million GenAI-capable smartphones shipped in 2025. The Scenario A trigger for edge AI is 100 million units — we're at 3.7 times that threshold. The caveat, which is on the card, is critical: these devices only matter for Scenario A if they're actually substituting for cloud inference. Right now the evidence suggests they're additive — people use their AI phone *and* call cloud APIs. Until substitution is demonstrated, this trigger is technically firing but analytically soft."

---

## SECTION 5 — Market Behavior Indicators (3 min)
*Screen: Scroll to the Market Behavior section*

---

"These four indicators measure revealed preference — what the people who are writing the largest infrastructure checks in the world are actually doing. This is harder to fake than surveys or projections.

*[M1: Hyperscaler Capex Growth]*

Microsoft, Google, Amazon, and Meta combined are spending over $600 billion in 2026 — a 36 percent increase year over year. The Scenario C trigger is above 35 percent. We're through it. These are not speculative commitments. This is cash leaving accounts and going into concrete and silicon. The companies that have the best internal demand forecasts in the world are betting on Scenario C conditions persisting. That's a meaningful signal.

*[M2: GPU Lease Rates]*

H100 spot lease rates have fallen from roughly $3.50 per hour at peak to about $2.25 today. The Scenario A trigger is a breach below $2.00. We're 25 cents away. This softening is a direct result of Blackwell supply coming online — more supply, slightly lower prices. Watch this number over the next two quarters. If it breaks through $2.00, that's the clearest early warning sign that supply is catching up to or exceeding demand.

*[M3: Interconnection Queue Depths]*

226 gigawatts in the ERCOT large-load queue. The Scenario C trigger is 15 gigawatts in Texas alone. We are 15 times past that threshold. I want to be careful here — queue is not the same as built capacity. Historically about 65 percent of queued projects are withdrawn before they're built. But even at a 65 percent withdrawal rate, that's roughly 79 gigawatts of actual data center load coming to ERCOT. That's a number that should focus minds in this room.

*[M4: Data Center Vacancy Rates]*

1.4 percent vacancy across primary markets. Northern Virginia is at 0.5 percent. The Scenario B confirmation range is 3 to 8 percent. We are well below the floor of the B range. 92 percent of new supply under construction is already pre-committed. This is a physical scarcity signal — not speculative demand, not queue, actual committed absorption of space that hasn't been built yet."

---

## SECTION 6 — Adoption Patterns Indicators (3 min)
*Screen: Scroll to the Adoption Patterns section*

---

"The final category measures whether the demand signals in the market layer are translating into actual business adoption — and whether the institutional environment is enabling or constraining it.

*[A1: GPU Shipments]*

NVIDIA data center revenue of $194 billion in fiscal 2026, up 68 percent year over year. The Scenario C trigger is above 50 percent sustained through 2027. We're through it today. The watch question is whether this growth rate can hold for two more years. Every historical technology buildout cycle has eventually decelerated. The question is when, not if.

*[A2: Enterprise AI ROI Surveys]*

This is one of the more nuanced indicators. 78 percent of enterprises are using AI in some form, but only 39 percent report a measurable EBIT impact. The Scenario B confirmation range is 25 to 35 percent with EBIT impact — we're at the top of B, approaching the Scenario C trigger of 40 percent. The gap between 78 percent adoption and 39 percent with EBIT impact represents a massive pipeline of enterprises that are using AI but haven't yet figured out how to monetize it. When that gap closes, it will generate a second wave of inference demand.

*[A3: AI Patent Filings]*

275,000 PCT filings in 2025, up 0.7 percent. No hard scenario triggers here — we use this as a leading indicator of R&D investment. Sustained growth signals AI research investment remains high. China leading with 73,000 filings, US second at 52,000. The geopolitical dimension of this chart is itself a Scenario C input — neither country is going to voluntarily constrain compute development.

*[A4: Regulatory Proposals]*

The US regulatory environment is moderately Scenario C supportive — the Biden executive order was rescinded, the AI Action Plan is deregulatory, and there's no federal energy consumption constraint on data centers in sight. The EU is the counterweight — the Digital Omnibus is creating some delay in AI Act implementation, but Europe remains the jurisdiction most likely to impose DC energy constraints. **Neither jurisdiction has yet enacted the energy consumption cap that would be the definitive Scenario A trigger.** Until that happens, regulation is not a binding constraint."

[Pause — take questions on indicators]

---

## SECTION 7 — So What: NRG Decision Framework (3 min)
*Screen: Scroll back up to the scenario framework*

---

"Let me pull this together into what it means for NRG.

**Today's read: Scenario B at 70% is the right base case — but the C tail risk is louder than it was a year ago.**

The demand signals — capex, queues, vacancy, GPU shipments — are all tracking C-directional. The efficiency signals — inference pricing, hardware efficiency — are real but being fully consumed by Jevons rebound. The Jevons rate at 115% means the system is in dynamic equilibrium, not tipping toward either extreme. Execute the phased buildout, maintain return discipline at 12 to 15 percent unlevered IRR, hold 5-to-10-year contract duration — not 20 to 25.

**The three numbers that would change this view:**

One — **Jevons rebound rate exits the 100-to-130% band.** If it drops below 80% for two consecutive quarters, start shifting probability toward A and revisit Phase 3 go/no-go. If it climbs above 150%, start shifting toward C and consider accelerating.

Two — **H100/H200 lease rates breach $2.00 per hour.** That's 25 cents away today. A sustained break below $2.00 means supply is catching up to demand — the single clearest early warning of Scenario A emerging at the infrastructure layer.

Three — **Hyperscaler capex growth decelerates below 20% year over year for two consecutive quarters.** These are the best-informed buyers in the market. If they're pulling back, that's a demand signal that overrides everything else on this dashboard.

**Until one of those three things happens, the base case holds. Execute against it.**"

---

## Closing (30 sec)

"This dashboard updates with every earnings cycle, every EIA data release, and every time Artificial Analysis refreshes inference pricing — roughly monthly. The scenario probabilities shown are our current analytical view. They should move when the data moves — and this dashboard is designed to show you, in real time, when that's happening.

Any questions?"

---

*[End of walkthrough — estimated total time 22–25 minutes]*

---

## Quick Reference: Key Numbers to Know Cold

| Indicator | Current | Scenario Signal |
|---|---|---|
| Jevons rebound rate | ~115% | B (sweet spot) |
| H100/H200 spot rate | ~$2.25/hr | Approaching A trigger ($2.00) |
| Hyperscaler capex growth | +36% YoY | C trigger MET |
| DC vacancy rate | 1.4% | C signal (below B floor) |
| ERCOT large-load queue | 226 GW | C trigger MET (15× threshold) |
| GPU shipments (NVIDIA DC) | +68% YoY | C trigger MET |
| Inference API pricing | $0.40/M tokens | A signal on price / B on volume |
| Edge AI device volumes | 370M units | A trigger MET (soft — no substitution yet) |
| Enterprise AI EBIT impact | 39% | Top of B / approaching C trigger |

---

## Anticipated Tough Questions

**Q: If 4 of 7 Scenario C triggers are firing, why is the probability only 15%?**

"Because triggers firing today tell you about current momentum. The 15% probability reflects whether that momentum is sustained for four more years at the same rate. Sustaining 50%+ GPU shipment growth and 35%+ hyperscaler capex growth through 2027 has no historical precedent at this scale. Markets normalize. The question is when. We think 2028. If we're wrong and it persists, we'll see it in the Jevons chart first."

**Q: What's the provenance of the Jevons rebound rate — how reliable is that number?**

"The energy frame input — DC electricity growth from EIA and LBNL, hardware efficiency from NVIDIA datasheets — is high confidence. The token frame is a proxy based on OpenAI revenue divided by average price per token and carries ±30% uncertainty. We're transparent about that on the dashboard. The qualitative conclusion — full Jevons rebound, firmly in B territory — is robust to that uncertainty range. What matters for the watch is the trend direction, not the precise level."

**Q: The regulatory slide shows the US is deregulatory. Doesn't that tilt toward C?**

"Marginally, yes. But the binding constraint on Scenario C isn't regulation — it's physics. Getting to 1,100 to 1,500 terawatt-hours by 2030 requires roughly 25 to 30 percent of current total US electricity generation directed to data centers. The grid, transmission buildout, and permitting timelines create a physical ceiling that no executive order can remove. Deregulation increases the *probability* of attempting C, but the physical infrastructure timeline is what ultimately limits it."

**Q: Should NRG be building more aggressively given the C signals?**

"The 15% C probability still represents a meaningful tail risk, and some of what looks like C-preparedness — securing interconnection rights, pre-positioning gas supply, maintaining site optionality — has positive expected value even in Scenario B. What we're arguing against is locking in 20-to-25-year fixed contracts at current pricing on the assumption C is the base case. The option to accelerate later, if C signals strengthen, is more valuable than the upside of over-committing now."

---

*Document version: Q1 2026 | Confidential — NRG Internal Use Only*
