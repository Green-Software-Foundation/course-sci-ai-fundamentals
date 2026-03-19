# Script: Choosing Your Functional Unit

**Module:** 08 — Choosing Your Functional Unit
**Course:** SCI for AI Fundamentals
**Duration:** 4-5 min

---

## For Consumers: Align with Cost

Let's talk about how to choose the functional unit R for each persona.

For Consumers, our recommendation is simple: align your carbon functional unit with your cost functional unit.

The industry has already converged on how AI services are priced:

**[VISUAL: Table of AI system types and their pricing models]**

| AI System Type | Typical Pricing |
| :---- | :---- |
| LLMs | Per token |
| Video generation | Per second |
| Image generation | Per image |
| Agentic AI | Per workflow execution |
| Classical ML | Per inference |

Use the same unit for your SCI.

---

## Why Align with Cost?

There are four good reasons.

**First, less cognitive load.** If you're already thinking in tokens for cost, thinking in tokens for carbon is natural. You don't have to do mental gymnastics to compare.

**Second, it enables real trade-offs.** Look at this comparison:

| Service | Cost | SCI |
| :---- | :---- | :---- |
| A | $2 per million tokens | 300g per million tokens |
| B | $1.50 per million tokens | 500g per million tokens |

Now you can make a real decision. Service B is cheaper but has higher carbon intensity. Service A costs more but is cleaner. Which matters more for this use case?

**Third, it fits with FinOps.** Most organisations already have cost attribution figured out. They know which team spent how much on which AI services. If carbon uses the same functional unit, it can ride those same rails. The attribution is already done.

**Fourth, it's future-proof.** Whatever new AI system emerges next, it will have a pricing model. Follow that model for carbon, and you're automatically aligned.

---

## For Providers: Align with Neural Scaling Laws

For Providers, the recommendation is different: align with neural scaling laws.

Let me explain what that means.

Neural scaling laws are empirical relationships discovered by AI researchers. They describe how model performance improves as you scale up certain factors.

Specifically, these laws tell us that model accuracy is roughly proportional to three things:

- **Compute**, measured in FLOPs (floating point operations)
- **Dataset size**, measured in training tokens
- **Model size**, measured in parameters

**[VISUAL: Simple representation of scaling laws]**

These are the levers that AI researchers pull to improve capability. When they want a more capable model, they increase one or more of these factors.

Now, there are caveats here. Scaling laws aren't perfect. They have limitations. Different architectures scale differently. There's ongoing debate about exactly how these relationships work.

But despite those caveats, the working group felt this was still the best foundation for Provider functional units. Here's why:

If you're trying to measure the efficiency of AI training, you need to normalise by something that represents "capability gained." Otherwise, you're just measuring size, not efficiency.

The scaling law factors — FLOPs, training tokens, parameters — are the best proxies we have for capability. They're well-researched. They're widely understood. They're already tracked by AI teams.

So Provider functional units should align with one of these:

| Functional Unit | What it measures |
| :---- | :---- |
| Per FLOP | Carbon per unit of compute |
| Per Training Token | Carbon per unit of training data |
| Per Parameter | Carbon per unit of model size |

Each emphasises different efficiency strategies:

**Per FLOP** incentivises algorithmic improvements and hardware efficiency.

**Per Training Token** incentivises data quality and curation.

**Per Parameter** incentivises efficient model architectures.

Providers should choose the unit that best reflects their optimisation focus, and clearly disclose their choice and rationale.
