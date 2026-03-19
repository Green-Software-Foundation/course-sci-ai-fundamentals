# Course Quiz: SCI for AI Fundamentals

**Pass mark:** 75% (9 out of 12)

Correct answers are marked with ✓.

---

## Explain why traditional carbon metrics fail to drive action in software teams

**1. A software team spends a quarter making their application significantly more energy efficient. But their carbon metric doesn't improve. What is the most likely reason?**

- Their efficiency improvements weren't large enough to show up
- **The metric measures total emissions, so growth in users cancelled out their efficiency gains ✓**
- They should have focused on offsets instead

**2. Why is carbon per functional unit more useful to an engineering team than total carbon emissions?**

- **It reflects something the team has direct agency over, regardless of how much the product grows ✓**
- It's easier to calculate
- It satisfies regulatory reporting requirements

---

## Calculate SCI scores using the core equation and its components

**3. Your team improves database query efficiency, cutting energy consumption per request by 30%. What happens to your SCI score?**

- It stays the same because embodied emissions are unchanged
- It goes up because more efficient queries increase request volume
- **It goes down because operational emissions have decreased ✓**

**4. Your software consumes 10 kWh of energy in a region with a carbon intensity of 200g CO2e per kWh. What are your operational emissions?**

- 20g CO2e
- **2,000g CO2e ✓**
- 200g CO2e

---

## Distinguish between Provider and Consumer responsibilities in AI systems

**5. A company trains a foundation model and offers it as an API. Which scores should they calculate and disclose?**

- **Both Provider SCI for training and Consumer SCI for inference ✓**
- Consumer SCI only, since inference is the ongoing activity
- Provider SCI only, since training is where the significant emissions occur

**6. Your company has built a web-based learning platform that uses AI in the backend to personalise course recommendations. Which SCI score should you calculate?**

- Consumer SCI, because you're using an AI API
- Provider SCI, because you built the system that uses AI
- **Neither. This isn't an AI product. The value to users is course delivery, not AI. You'd apply SCI for Web rather than SCI for AI ✓**

---

## Design measurement strategies that align accountability with agency

**7. Your organisation both trains models and runs inference. Leadership wants one team to own the SCI programme. What do you recommend?**

- Assign ownership to the team with the highest emissions
- **Split ownership: the ML team owns Provider SCI, the infrastructure team owns Consumer SCI ✓**
- Centralise ownership with the sustainability team so reporting stays consistent

**8. You want to set a meaningful efficiency target for next year's model training. Which approach gives you the most actionable baseline?**

- Calculate total training emissions and aim to emit less next time
- Calculate training emissions as a percentage of total company emissions
- **Calculate emissions per FLOP, per training token, or per parameter and set a target to beat that rate ✓**

---

## Select appropriate functional units for your AI measurement needs

**9. You're running an LLM inference service. Your provider charges per token. What functional unit should your Consumer SCI use?**

- **Per token, to align your carbon metric with how the service is priced and consumed ✓**
- Per inference request, to capture the full cost of each interaction
- Per user session, to reflect the end user experience

**10. A Provider is focused on improving the quality and curation of their training data. Which functional unit best incentivises that work?**

- Per parameter
- **Per training token ✓**
- Per FLOP

---

## Make informed decisions about measurement approaches based on available data

**11. You're starting your first SCI measurement programme and can only access cost data right now. Should you wait until you have better data?**

- Yes, cost-based estimation isn't reliable enough to be worth reporting
- **No, start with cost data and improve your methodology over time as better data becomes available ✓**
- Only proceed if you can get at least model-based estimates first

**12. You can directly measure energy consumption for 10% of your infrastructure. The rest sits behind a cloud provider that doesn't expose energy data. What should you do?**

- Wait until you can measure everything directly before calculating a score
- Only report on the 10% you can measure directly
- **Measure the 10% directly and use model-based calculation to estimate the remaining 90%, combining both in your SCI ✓**
