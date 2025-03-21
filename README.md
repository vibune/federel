# Federel

> 📘 **Name Origin**: The name **Federel** comes from **Federated Relevancy** — a system where decentralized agents share AI-distilled knowledge based on relevance and verified ownership, not traditional rankings.

**Federel** is a federated AI search protocol powered by decentralized agents, user intent, and verifiable domain-based knowledge sharing — with no central indexing, no ranking, and no ads.  
It is designed to be **spam-resistant**, **privacy-first**, and **community-governed** from day one.
[🧠 Project Concept →](docs/CONCEPT.md)

---

## ✨ What Makes Federel Different?

- 🧠 **Intent-Based Search** — Users find knowledge by asking, not by clicking ranked links.
- 🤖 **Local AI Agents** — You run your own crawler and summarizer.
- 🌐 **Federated Knowledge Pool** — Share only distilled knowledge, not raw content.
- 🔐 **Verified Publishing via DNS** — Only domain owners can contribute public data.
- ⚖️ **No Rankings. No SEO. No Ads.** — Just relevance, semantics, and community-driven discovery.

---

## 🧪 Project Status

Federel is in the early concept + prototype phase. The plan is to:
1. Publish the protocol vision and specs
2. Build a demo pipeline (`crawl → summarize → embed → query`)
3. Create the publishing + trust flow using DNS verification

---

## 📁 Repo Structure (Planned)

```txt
agents/         # Local crawlers and assistants
summarizer/     # LLM-powered summarization scripts
knowledge_pool/ # Embedding, vector search, and knowledge access
publisher/      # DNS + KPID identity verification and signing
docs/           # Protocol, trust, architecture
