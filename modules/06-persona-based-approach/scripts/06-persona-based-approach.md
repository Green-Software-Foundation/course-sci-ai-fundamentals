# Script: Persona-Based Approach

**Module:** 06 — Persona-Based Approach
**Course:** SCI for AI Fundamentals
**Duration:** 4-5 min

---

## The Core Insight

Here's the design principle we followed:

Ignore the software boundary first. Decide the persona you want to target. Understand their realm of agency. Then design a metric with a boundary that sits within that realm.

Do it in that order.

---

## Two Personas

For AI, we identified two primary personas:

**Providers** are anyone who builds or sells AI. They have agency over how the model is created and trained.

**Consumers** are anyone who uses or buys AI. They have agency over how the model is used at runtime.

These aren't necessarily different companies. A single organisation might be both a Provider and a Consumer. But they're different roles with different agency, so they need different metrics.

---

## The AI Lifecycle

To map this properly, we needed to define the AI lifecycle. We aligned with ISO definitions and identified these stages:

**[VISUAL: Horizontal flow of lifecycle stages]**

**Inception** is where you define the problem, assess whether AI is the right solution, engage stakeholders, and establish constraints.

**Design and Development** covers data collection, preprocessing, synthetic data generation, model selection, feature engineering, training, evaluation, and benchmarking.

**Deployment** involves integrating the model into larger systems, connecting with external applications, and testing before going live.

**Operation and Monitoring** is the runtime phase: inference, orchestration, monitoring performance, maintenance, and ongoing optimisation.

**End of Life** is decommissioning the model when it's no longer needed.

---

## Mapping Lifecycle to Personas

Now we map these stages to the personas based on agency.

**[VISUAL: Lifecycle with a dividing line showing Provider vs Consumer domains]**

**Providers control:**

- Inception
- Design and Development
- Deployment
- End of Life

**Consumers control:**

- Operation and Monitoring

The dividing line is clear. Before the model goes into production, the Provider has agency. Once it's running, the Consumer has agency over how it's used.

Each persona is accountable only for the stages where they have agency.

---

## Why This Works — A Concrete Example

Let me show you why this separation matters with a concrete example.

Historically, training used to be the dominant source of emissions in AI systems. But that's changed. For popular models that are used at scale, inference now far, far surpasses training in total emissions.

Imagine you're the team responsible for training. You do an absolutely incredible job. You optimise your algorithms. You use efficient hardware. You reduce training emissions by 40%.

But your metric includes both training and inference. And the product team just launched a major marketing campaign. Usage doubles. Inference emissions explode.

Your 40% improvement in training? It's completely lost in the noise. The metric goes up despite your excellent work. You stop being incentivised to optimise training because it doesn't seem to matter.

**[VISUAL: Training improvements getting swamped by inference growth]**

Now flip it around. You're on the product team. You've done incredible work optimising runtime operations. Better caching. Smarter batching. Efficient prompt design. You've cut inference emissions per request by 30%.

But the training team just did a major retraining run with a new architecture. It was expensive. It took weeks of GPU time.

Their one-time training cost ruins your metric for the quarter. Your sustained optimisation work is invisible.

**[VISUAL: Runtime improvements getting wiped out by a training spike]**

This is exactly the problem we talked about in Module 1. When multiple teams are responsible for a metric, nobody is responsible for the metric.

By separating Provider SCI and Consumer SCI, each team has a metric they can own. The training team can focus on what they're good at: making training efficient. The product team can focus on what they're good at: making runtime operations efficient.

Both teams can set targets. Both teams can show progress. Both teams are accountable for things they actually control.

---

## Each Persona Gets Their Own SCI

Both personas use the same core equation:

```
SCI = (O + M) per R
```

But the specifics are different:

**Different software boundaries.** Providers include training infrastructure. Consumers include inference infrastructure.

**Different functional units.** Providers might use "per parameter" or "per training token." Consumers might use "per inference" or "per output token."

**Different actors held accountable.** The Provider SCI is owned by the team that builds the model. The Consumer SCI is owned by the team that uses it.

**[VISUAL: Two SCI score cards side by side]**

Same equation, different applications, different accountability.
