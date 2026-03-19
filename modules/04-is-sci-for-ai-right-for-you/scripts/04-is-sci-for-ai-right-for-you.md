# Script: Is SCI for AI Right for You?

**Module:** 04 — Is SCI for AI Right for You?
**Course:** SCI for AI Fundamentals
**Duration:** 1-2 min

---

The SCI works beautifully for most software. You define your boundary, pick your functional unit, measure or calculate your emissions, and you're off.

But AI introduces unique challenges. And before we get into them, let me be clear about what SCI for AI is for.

SCI for AI is a domain-specific specification. It's for people building AI products — products where the thing you're delivering IS AI. Where the functional unit is inherently AI-native: per token, per inference, per image generated, per second of video.

It's not for products that happen to use AI as an implementation detail.

Here's the test: if you're building an e-commerce site that uses AI for product recommendations, but your product's value to customers is 'buying things' — your functional unit is probably 'per purchase' or 'per user session.' That's not an AI product in this sense. The AI is just part of how you built it. For that, you'd use the standard SCI specification, or SCI for Web when that's available, or whatever domain-specific spec fits your product.

But if you're building an inference API, a chatbot platform, an image generation service, a RAG application — something where AI IS the product — then SCI for AI is for you.
