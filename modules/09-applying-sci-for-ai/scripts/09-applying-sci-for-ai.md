# Script: Applying SCI for AI

**Module:** 09 — Applying SCI for AI
**Course:** SCI for AI Fundamentals
**Duration:** 3-4 min

---

Let's bring this all together with practical guidance.

## What Scores Do You Calculate?

Here's the simple framework:

Did you train a model or do significant fine-tuning? Calculate and disclose a Provider SCI.

Are you running inference infrastructure or building an application that delivers AI to users? Calculate and disclose a Consumer SCI.

Did you do both? Disclose both.

Most AI companies will disclose both scores. The foundation model providers — they train models AND run inference. Both scores. A startup that fine-tunes an open model and serves it — probably both scores. A company building a RAG application on someone else's API — Consumer SCI only.

## Where Does Your Data Come From?

For your Provider SCI, you're measuring your own training infrastructure. You have access to that data. Use measurement where you can, models where you can't.

For your Consumer SCI, it depends on your situation.

If you run your own inference infrastructure, measure it directly. Your servers, your energy, your hardware.

If you're calling someone else's API, you need to account for those emissions too. In the ideal case, your provider discloses their Consumer SCI, and you can use that figure directly. If they don't, you estimate — using models if you can, falling back to cost-based estimation if you have to.

Your Consumer SCI is your infrastructure plus the attributed emissions from the services you call. Add them together.

## Reminder: Is SCI for AI Right for You?

Remember the test from Module 1. SCI for AI is for AI products — where the functional unit is AI-native.

If your product uses AI internally but the value to users isn't AI itself, you probably want a different specification. An e-commerce site with AI recommendations? Your functional unit is probably 'per purchase.' That's SCI for Web territory, not SCI for AI.

If AI IS your product — an inference API, a chatbot, an image generator, an AI-powered document processor — then SCI for AI applies.

## For Leadership

If you're evaluating whether to adopt SCI for AI, here's the framework:

Do you train models? Provider SCI gives your ML teams actionable efficiency targets. Track training efficiency across model versions. Set improvement targets.

Do you run inference? Consumer SCI incentivises your infrastructure teams to make inference more efficient. When they improve it, the score goes down, and that benefits everyone downstream.

Do you build AI applications? Consumer SCI helps you measure and optimise your usage patterns, and make informed choices about which services to use.

Assign the right scores to the right teams. Provider SCI to whoever owns training. Consumer SCI to whoever owns runtime operations. Don't blur the lines.

## Closing

The SCI for AI doesn't just measure emissions. It's designed to reduce them.

Two boundaries must align: the inclusion boundary and the agency boundary. Where they overlap is where the right actions live.

Provider SCI and Consumer SCI exist because training and inference have different agency profiles. Separate them, and each team gets a metric they can actually move.

Disclose what's relevant to what you built. If you trained it, disclose Provider SCI. If you run inference, disclose Consumer SCI. If you're building on someone else's API, calculate Consumer SCI and push your providers to disclose theirs.

Thank you.
