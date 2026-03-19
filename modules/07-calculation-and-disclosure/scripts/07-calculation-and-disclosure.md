# Script: Calculation & Disclosure

**Module:** 07 — Calculation & Disclosure
**Course:** SCI for AI Fundamentals
**Duration:** 2-3 min

---

Now, an important clarification. The terms 'Consumer' and 'Provider' describe the lifecycle stage, not who uses the score.

Provider SCI measures the efficiency of training — the build stages. Consumer SCI measures the efficiency of runtime operations — inference.

Both scores are calculated and disclosed by whoever builds that thing.

So if you're a major AI company — say you've trained a foundation model and you're offering it as an API — you would calculate and disclose both scores. A Provider SCI for how efficiently you trained the model. A Consumer SCI for how efficiently your inference infrastructure runs.

Now, a company building on top of your API would look at your disclosed Consumer SCI, add their own infrastructure emissions, and calculate their own Consumer SCI. They wouldn't have a Provider SCI because they didn't train a model.

And end users — the people actually using these products — don't calculate anything. They're just users.

**[VISUAL: Dependency tree showing Foundation Model Company → App Builder → End User, with which scores each calculates]**

Let me give you a few scenarios:

If you trained a model and you're providing inference services, you calculate and disclose both a Provider SCI and a Consumer SCI.

If you took someone else's model — maybe open source — and built your own inference infrastructure, you disclose a Consumer SCI only. You didn't do the training.

If you built a RAG solution or wrapper that calls an external API, you calculate a Consumer SCI. It includes your infrastructure plus the attributed emissions from your API calls. If the provider you're calling discloses their Consumer SCI, you can use that. If not, you estimate using models or fall back to cost.

If you're a research lab that trains models but doesn't run production inference, you might only have a Provider SCI.

The principle is: disclose what's relevant to what you built.

One more important point. The Consumer SCI isn't just valuable to downstream users. It's valuable to providers too.

If you're a provider running inference infrastructure, improving that infrastructure reduces your Consumer SCI. That benefits your customers. It's a shared responsibility — the provider can make the infrastructure more efficient, and downstream users can make their usage more efficient. Both actions reduce the Consumer SCI.
