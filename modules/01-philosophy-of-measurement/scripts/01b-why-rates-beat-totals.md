# Script: Why Rates Beat Totals

**Module:** 01 — Philosophy of Measurement
**Lesson:** 01b
**Course:** SCI for AI Fundamentals
**Duration:** ~2-3 min (part of 7-8 min module)

---

## Part B: Why Rates, Not Totals?

This brings us to a fundamental question: why is the SCI a rate and not a total?

Many people expect a carbon metric to be a total. "How much CO2 did my software emit?" That feels like the natural question.

But totals are problematic for driving action. Let me show you why.

**[VISUAL: GPT emissions table appearing]**

Here are the training emissions for three versions of GPT:

| Version | Total Emissions |
| :---- | :---- |
| GPT-2 | ~50 tonnes CO2e |
| GPT-3 | ~1,200 tonnes CO2e |
| GPT-4 | ~20,000 tonnes CO2e |

If you just look at totals, the story is simple: everything is getting worse. GPT-4 emitted 400 times more carbon than GPT-2.

But that's not the whole picture. These models are also dramatically more capable. GPT-4 has roughly 600 times more parameters than GPT-2.

Now look at the same data normalised per billion parameters:

| Version | Emissions per Billion Parameters |
| :---- | :---- |
| GPT-2 | ~33.3 tonnes CO2e |
| GPT-3 | ~6.86 tonnes CO2e |
| GPT-4 | ~20 tonnes CO2e |

This tells a completely different story.

GPT-3 was about five times more efficient than GPT-2 per parameter. That's a massive improvement in efficiency.

GPT-4 regressed somewhat from GPT-3, but it's still significantly more efficient than GPT-2.

And critically, now you can set a meaningful target. If you're the team about to train GPT-5, you can say: "Let's beat 6.86 tonnes per billion parameters." That's specific. That's actionable. That's something engineers can work toward.

With totals, what target would you set? "Emit less than GPT-4"? But you know GPT-5 will be bigger and more capable. Totals give you no path forward.

**[VISUAL: Data center analogy]**

This isn't a new concept. Data centers have understood this for years.

Data centers are getting bigger every year. Total energy consumption keeps rising. But nobody says data centers are failing because of that.

Instead, we track PUE: Power Usage Effectiveness. It measures how efficiently a data center uses power. And PUE has generally improved over time, even as total energy has grown.

Nobody would give a data center operator a target of "use less total energy" when demand is doubling. You give them an efficiency target. Same logic applies to AI. Same logic applies to software.

**[VISUAL: Two graphs — total energy rising, PUE improving]**

So the SCI is a rate, not a total. Carbon per functional unit. That's what makes it comparable and actionable.

And here's an important philosophical point: the SCI is not about calculating the exact carbon emissions of a piece of software. It's about directional truth. Can you track whether you're getting better or worse? Can you set a target and measure progress toward it?

If your methodology is consistent, if your boundary is well-defined, then even if the absolute number isn't perfectly accurate, you can still drive improvement. That's what matters.
