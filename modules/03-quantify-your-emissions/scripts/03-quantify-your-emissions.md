# Script: Quantify Your Emissions

**Module:** 03 — Quantify Your Emissions
**Course:** SCI for AI Fundamentals
**Duration:** 3-4 min

---

## Introduction

So we've established what the SCI measures and why. Now let's talk about where the data actually comes from.

There's a hierarchy here, and it matters.

**[VISUAL: Vertical stack showing Measurement → Models → Cost]**

At the top, we have direct measurement. That's the preferred approach.

In the middle, we have calculation using models. That's a good approach when measurement isn't possible.

At the bottom, we have cost-based estimation. That's the last resort.

---

## Direct Measurement

Direct measurement means actually counting energy consumption, emissions, and functional units.

You might have hardware meters on your server racks. You might have telemetry from your infrastructure that reports power consumption. You might have logs that let you count exactly how many requests you served.

For example: your server rack has a power meter. It shows you consumed 500 kilowatt hours last month. Your logs show you served 10 million requests. So your energy per request is 0.05 watt hours.

That's direct measurement. If you can do it, do it. It's the most accurate.

**When to use direct measurement:**

- You have access to hardware-level telemetry
- Your cloud provider exposes energy data
- You have physical meters on your infrastructure

---

## Calculation with Models

But often you can't measure directly. Maybe your cloud provider doesn't expose energy data. Maybe you're in a shared, virtualised environment where you can't see the physical hardware. Maybe your supply chain just hasn't disclosed enough information.

In these cases, you use observations you *can* get and apply models that convert them into impacts.

**Observations** are things you can measure directly:

- CPU utilisation
- Memory usage
- Network transfer
- API call counts
- Page views

**Models** convert those observations into impacts:

- "CPU at 50% utilisation on this chip type uses approximately X watts"
- "X watts in this region equals Y grams of CO2"

This is what the Impact Framework does: take observations, apply models, produce impact estimates. Everything is transparent and auditable.

**When to use calculation:**

- You can't measure energy directly
- Your supply chain hasn't disclosed enough data
- You're in a shared or virtualised environment

The key is to document your models and assumptions. Be consistent over time.

---

## Cost-Based Estimation

At the bottom of the hierarchy, we have cost.

Cost has one advantage: you will always have a cost number. Energy data can be hard to get. Server counts can be obscured. But cost? Your provider will always tell you what you owe them.

So if you absolutely cannot get better data, cost can be used as a last resort. But know its limitations.

And what do I mean by cost based estimation, it's still a model, some sort of $ =~ Carbon Emission Factor. You can get them from various sources, heck, you can divide a companies SCOPE 1,2 an 3 by their revenue and estimate it. But if you can use one of the others, it will provide mode useful data which inform better actions.
