# agent.md

## 🤖 Federel Agent Roles and Responsibilities

Agents are the autonomous or semi-autonomous software components that make Federel work. Every user, whether an individual, an organization, or a domain owner, interacts with Federel through an agent.

Federel defines agents as software entities capable of:
- Crawling and summarizing content
- Storing knowledge locally
- Evaluating and submitting content
- Responding to user feedback and intent

An agent may function as both an **observer** and a **publisher**, depending on the user’s role and whether the visited or owned domain matches their **KPID**.

### Agent Modes:
- **Observer Mode**: When browsing content not owned by the user
- **Publisher Mode**: When visiting or crawling a domain the user controls (via KPID verification)

---

## 🧭 Observer Behaviour

When a user visits a website that they do not own or control (i.e., the domain does **not** match a verified KPID), the agent behaves in **Observer Mode**.

### ✅ Behaviors:
- Crawl or receive content as the user browses
- Distill pages into local knowledge chunks (AI summarization)
- Store knowledge locally (not shared publicly)
- Accept and store user input, e.g.:
  - Thumbs up/down
  - Notes or comments
  - Reports of spam or misinformation
- Optionally share anonymized feedback into the federated feedback layer
- Query the user’s private or federated knowledge pool

### ❌ Restrictions:
- Cannot publish knowledge into the public pool

---

## 🔐 Publisher Behaviour

When the agent interacts with a domain that the user **owns** and has verified via KPID (Knowledge Publisher ID), it enters **Publisher Mode**.

### ✅ Behaviors:
- Crawl the owned domain (or accept manual input)
- Distill and summarize content
- Sign knowledge chunks with KPID
- Publish knowledge into the shared, verifiable public pool
- Refresh or retract knowledge by re-crawling or updating the DNS record
- Optionally respond to feedback from the federated network

### 🔄 Publishing Flow:
1. Crawl → Summarize → Embed
2. Check for valid DNS KPID
3. Sign + submit to public pool

---

## 🗳️ Feedback and Social Signals

Any agent can:
- Submit **feedback objects** about a page or domain (e.g., spam, low quality, misaligned intent)
- Track and learn from user interaction patterns (e.g., bounce rates, reading time)

In the future, agents may use **AI-based heuristics** to:
- Automatically flag pages with poor engagement (e.g., short dwell time after search)
- Correlate feedback with intent, query relevance, and prior user signals

Only agents operating in **Publisher Mode** can:
- Re-crawl and update knowledge
- Adjust their own content or retract it

Agents may weigh feedback differently — this is up to their local configuration.

---

## 🔐 Trust Enforcement

Publishing is allowed **only** if the domain in question:
- Has a valid KPID TXT record
- Matches the source URL of the knowledge

This ensures:
- No one can publish fake content about another site
- Only the real owner takes responsibility for what's shared

---

## 📚 Summary

Agents are the core of Federel’s decentralized architecture. They:
- Provide summarization, verification, and local storage
- Allow user-level filtering and contribution
- Respect publishing authority via DNS and KPID

This separation of roles enables a trustworthy, human-centered, and federated model for Internet search.

