# Script: Core Equation: O, M & R

**Module:** 02 — The SCI Equation
**Lesson:** 02a
**Course:** SCI for AI Fundamentals
**Duration:** ~4-5 min (part of 5-6 min module)

---

## The Core Equation

The SCI equation is elegantly simple. Here it is:

```
SCI = C per R
```

That's it. The SCI is a rate. It's the amount of carbon per unit of work. Lower is better. And reaching zero is impossible.

That last part is important. This isn't a metric where you can "solve" it and be done. There's always room for improvement. It's a continuous journey.

Now, let's expand that equation:

```
SCI = (O + M) per R
```

**O** is operational emissions. That's the carbon emitted from running your software.

**M** is embodied emissions. That's the carbon associated with the hardware your software runs on.

**R** is the functional unit. It's how you measure "one unit of work" for your software.

Let me break down each component.

---

## Operational Emissions (O)

Operational emissions are calculated as:

```
O = E × I
```

**E** is the energy your software consumes, measured in kilowatt hours.

**I** is the carbon intensity of the electricity, measured in grams of CO2 equivalent per kilowatt hour.

~~**[VISUAL: E × I shown as two dials]**~~

This is where two of our three target actions show up.

**Energy efficiency** means reducing E. Write more efficient code. Optimise your database queries. Right-size your infrastructure. When E goes down, O goes down, and your SCI goes down.

**Carbon awareness** means reducing I. Run your workloads when the grid is cleaner. That might mean running batch jobs at night when there's more wind power. Or it might mean running workloads in regions with cleaner grids. When I goes down, O goes down, and your SCI goes down.

**[VISUAL: World map showing different carbon intensities by region]**

**[VISUAL: Clock showing carbon intensity changing through the day]**

---

## Embodied Emissions (M)

Now let's talk about embodied emissions. This is the carbon that was emitted to manufacture the hardware your software runs on.

Here's the challenge: servers are shared. Your software doesn't get its own dedicated hardware. It shares with other workloads, other applications, maybe other companies entirely if you're in the cloud.

So you need a way to allocate a fair share of the total embodied emissions to your piece of software. That's what the M equation does:

```
M = TE × (TiR/EL) × (RR/ToR)
```

Let me walk through each part.

**TE** is the Total Embodied Emissions of the hardware. This comes from lifecycle assessment data.

**TiR** is Time Reserved. How long did you use the hardware?

**EL** is Expected Lifespan. How long is this hardware expected to last?

**RR** is Resources Reserved. What share of the hardware did you use?

**ToR** is Total Resources. What's the total capacity of the hardware?

Let me give you a concrete example.

**[VISUAL: Calculation appearing step by step]**

Say you have a server with 1000 kilograms of embodied carbon and an expected lifespan of 4 years.

Your software reserved that server for 1 hour and used 25% of the available resources.

Your share of embodied emissions is:

1000 kilograms, multiplied by 1 hour divided by 4 years worth of hours, multiplied by 25%.

That works out to about 7.1 grams.

That's your fair share of the embodied carbon for that hour of compute.

**[VISUAL: Server with a "slice" being carved out]**

This is where **hardware efficiency** shows up. Use fewer servers, and RR goes down. Use servers for less time, and TiR goes down. Extend hardware lifespan, and EL goes up, which reduces the fraction.

Any of these improvements reduces M, which reduces your SCI.

---

## The Functional Unit (R)

The functional unit is what turns a total into a rate. It's how you define "one unit of work" for your software.

The choice of R should reflect how your software scales:

- Per user
- Per API call
- Per transaction
- Per minute of video streamed
- Per ML training run

The functional unit is what makes the SCI comparable and actionable. It's what lets you set targets and track progress even as your software grows.

**[VISUAL: Different R options as cards]**

A few key principles:

Keep R consistent when comparing over time. If you change your functional unit, you're not comparing apples to apples anymore.

Keep R consistent across components you're summing together. If you're calculating the SCI of a whole system, all the components need to use the same R.

And always disclose your choice of R when you report your SCI score. Otherwise, people can't properly interpret what the number means.
