# Script: Why AI Needs Special Treatment

**Module:** 05 — Why AI Needs Special Treatment
**Course:** SCI for AI Fundamentals
**Duration:** 3-4 min

---

AI introduces a unique problem. It's an agency problem.

---

## The AI Challenge

AI systems have this unusual characteristic: they require massive upfront emissions before anyone uses them.

Training a large language model can emit thousands of tonnes of CO2. And all of that happens before a single user sends a single prompt.

It's like embodied emissions, but for the model itself rather than the hardware.

Now, here's where it gets interesting. AI systems have two very different activities:

**Training** is resource-intensive. It might happen once, or periodically for retraining. And it's controlled by whoever builds and manages the model.

**Inference** is per-request. It happens continuously as people use the model. And it's controlled by whoever is using the model.

**[VISUAL: Timeline showing Training as a big burst, then Deployment, then Inference as an ongoing stream]**

These two activities have completely different agency profiles.

| Activity | Who has agency? | What can they do? |
| :---- | :---- | :---- |
| Training | Model builder | Choose efficient hardware, optimise algorithms, pick cleaner regions |
| Inference | Model user | Write better prompts, cache responses, batch requests, choose which model |

Whoever builds and manages the model has the most agency to reduce training emissions.

Whoever uses the model has the most agency to reduce inference emissions.

---

## The Agency Problem

So here's the question: if I'm using an AI API, what can I do about training emissions?

Nothing. I didn't train it. I can't go back in time and make them train it more efficiently.

But I *can* control how efficiently I use it. I can write better prompts that use fewer tokens. I can cache responses. I can batch requests. I can choose which model to call for which task.

A single SCI score that combines training and inference would hold me accountable for things I can't control. That violates our core principle: the inclusion boundary should sit within the agency boundary.

**[VISUAL: The two circles from Module 1, but now showing misalignment between a combined AI metric and a user's agency]**

Remember those two boundaries from Module 1?

If we set the inclusion boundary as "Training plus Inference" but the user's agency boundary only covers Inference, they don't overlap properly.

The metric can't drive action because the user can't act on half of what's being measured.

---

## The Solution

So rather than one metric that tries to do everything, we align the metric with the persona who can act.

We split it. Providers get a metric that covers what they control. Consumers get a metric that covers what they control.

**[VISUAL: Two separate diagrams showing proper alignment for each persona]**

That's the foundation of SCI for AI.
