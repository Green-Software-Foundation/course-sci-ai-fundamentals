# Course Outline: SCI for AI Fundamentals

**Tagline:** Learn the methodology that turns AI sustainability from a goal into a metric

**Duration:** ~50 minutes of video content across 10 modules

**Course URL:** [grnsft.org/sci-ai-fundamentals-course](https://grnsft.org/sci-ai-fundamentals-course)

---

## About This Course

Most carbon metrics tell you how bad things are. The SCI was designed to tell you what to do about it. This course introduces the Software Carbon Intensity for AI specification: a new standard built from the ground up to make AI's carbon footprint transparent, comparable, and actionable.

The SCI isn't a comprehensive carbon accounting tool. It was designed with a specific purpose: to guarantee that if you make your software more energy efficient, more hardware efficient, or more carbon aware, your score goes down. Not by accident. By design.

You'll start with the philosophy that makes the SCI different from every other carbon metric, then work through the equation, the data, and the decisions, before arriving at practical guidance you can apply to your own organisation.

## Who This Course Is For

Software practitioners, sustainability professionals, and IT leaders who want to go beyond awareness and actually measure and reduce the carbon emissions of AI systems.

**Prerequisites:** Foundational knowledge of digital sustainability concepts, general familiarity with software systems and infrastructure, and broad awareness of AI's environmental impact. New to green software? Consider the [Green Software Practitioner course](https://grnsft.org/mov-plat-gs-practitioner) first.

## Learning Outcomes

By the end of this course, you will be able to:

- Explain why traditional carbon metrics fail to drive action in software teams
- Calculate SCI scores using the core equation and its components
- Distinguish between Provider and Consumer responsibilities in AI systems
- Select appropriate functional units for your AI measurement needs
- Design measurement strategies that align accountability with agency
- Make informed decisions about measurement approaches based on available data

---

## Module Structure

### [Module 00 — Introduction](modules/00-introduction/)

Learn the newest SCI specification measuring the carbon impact of Artificial Intelligence. This module sets out the purpose of the SCI for AI, what makes it different from other carbon metrics, and what you'll be able to do by the end of the course.

---

### [Module 01 — Philosophy of Measurement](modules/01-philosophy-of-measurement/)

Discover why most carbon metrics tell you how bad things are but not what to do about it. We introduce the two boundaries every good metric needs and reveal the core design principle behind the SCI: that where your inclusion boundary and agency boundary overlap is exactly where the right actions live.

**Lessons:**
1. Boundaries That Must Align
2. Why Rates Beat Totals
3. Designed to Drive Change

**In this module:**
- Why misaligned boundaries create metrics that frustrate rather than motivate
- How rates drive action in ways that totals never can
- The three specific actions the SCI was engineered to reward
- Why the SCI guarantees your score improves when you do the right things

---

### [Module 02 — The SCI Equation](modules/02-the-sci-equation/)

Break down the equation at the heart of the SCI specification: (O + M) per R. You'll see exactly how each component works, where the carbon comes from, and how the functional unit transforms a raw emissions total into a meaningful, comparable rate.

**Lessons:**
1. Core Equation: O, M & R
2. Deliberate Exclusions

**In this module:**
- How operational emissions (O) are calculated from energy and carbon intensity
- How embodied emissions (M) are fairly allocated across shared hardware
- How the functional unit (R) makes your score comparable and actionable
- Why offsets and renewable energy credits are deliberately excluded from the SCI

---

### [Module 03 — Quantify Your Emissions](modules/03-quantify-your-emissions/)

You know what to measure. Now learn how to get the data. We walk through the quantification hierarchy the SCI relies on, from direct measurement at the top to cost-based estimation as a last resort, and help you understand when each approach is appropriate.

**In this module:**
- Why direct measurement is always the preferred starting point
- How to use models when you can't measure energy consumption directly
- When cost-based estimation is acceptable and what its limitations are
- Why consistency in your methodology matters more than perfect precision

---

### [Module 04 — Is SCI for AI Right for You?](modules/04-is-sci-for-ai-right-for-you/)

Not every product that uses AI is an AI product. Here you'll quickly determine whether the SCI for AI specification applies to your situation, or whether a different domain-specific specification is the better fit.

**In this module:**
- What makes something an AI product versus a product that uses AI
- The functional unit test that clarifies which specification to apply
- How SCI for AI relates to the standard SCI and other domain-specific variants
- Concrete examples of products that are, and aren't, in scope

---

### [Module 05 — Why AI Needs Special Treatment](modules/05-why-ai-needs-special-treatment/)

Training a model can emit thousands of tonnes of carbon before a single user sends a single prompt. That creates a unique agency problem, and it's why a single combined metric for AI simply doesn't work. Find out what makes AI different and why solving it requires a fresh approach.

**In this module:**
- Why training and inference have fundamentally different agency profiles
- What happens when a metric holds people accountable for things they can't control
- How the two-boundary principle from Module 01 breaks down with a combined AI metric
- Why separating the scores is the only way to drive action in both areas

---

### [Module 06 — Persona-Based Approach](modules/06-persona-based-approach/)

The solution to the AI agency problem is elegant: design the metric around the person who can act on it. We introduce the Provider and Consumer personas, map the AI lifecycle to each, and show with real examples why keeping the scores separate is what makes them useful.

**In this module:**
- Who Providers and Consumers are, and what each controls
- How the AI lifecycle stages map to each persona's sphere of agency
- Why combining training and inference in one score masks the improvements each team makes
- How Provider SCI and Consumer SCI work as complementary, not competing, metrics

---

### [Module 07 — Calculation & Disclosure](modules/07-calculation-and-disclosure/)

Who calculates what, and when? You'll get a clear, practical framework based on what you've built, whether that's a foundation model, an inference service, a RAG application, or something in between.

**In this module:**
- The dependency chain from foundation model providers to application builders
- Which scores to calculate based on your role in the AI value chain
- How to handle emissions from external APIs when providers do and don't disclose their SCI
- Why Consumer SCI is a shared responsibility across the entire stack

---

### [Module 08 — Choosing Your Functional Unit](modules/08-choosing-your-functional-unit/)

The functional unit makes or breaks your SCI score. Choose the wrong one and you can't set targets, track progress, or compare results meaningfully. We give you clear, principled guidance on which unit to use depending on whether you're a Provider or a Consumer.

**In this module:**
- Why Consumer functional units should align with how AI services are priced
- How cost-carbon alignment reduces cognitive load and enables real trade-offs
- Why Provider functional units should align with neural scaling laws
- How each Provider unit — per FLOP, per training token, per parameter — rewards a different efficiency strategy

---

### [Module 09 — Applying SCI for AI](modules/09-applying-sci-for-ai/)

Everything comes together here. You'll get a practical decision framework for applying SCI for AI in your organisation, from working out which scores you need to getting leadership on board with why this matters.

**In this module:**
- A simple framework for deciding which scores to calculate based on what you built
- How to source the data you need for both Provider and Consumer SCI
- How to make the case for SCI for AI adoption to technical and non-technical stakeholders
- The core principle that ties everything together: align the metric with the person who can act

---

## Assessment

After completing all modules, take the [12-question assessment](assessment/quiz.md). Score 75% or above to earn the **SCI for AI Fundamentals** digital badge.

**Credential portal:** [badges.greensoftware.foundation](https://badges.greensoftware.foundation/)

---

## Next Steps

- **Read the specification:** [github.com/Green-Software-Foundation/sci-ai](https://github.com/Green-Software-Foundation/sci-ai)
- **Explore green software patterns for AI:** [patterns.greensoftware.foundation/catalog/ai](https://patterns.greensoftware.foundation/catalog/ai)
- **Read the parent SCI specification:** [sci.greensoftware.foundation](https://sci.greensoftware.foundation)
- **Get involved:** [greensoftware.foundation](https://greensoftware.foundation)
