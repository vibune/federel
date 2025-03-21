
# Contributing to Federel

First off, thank you for your interest in Federel!  
This project is in early development, and every contribution — ideas, code, feedback, or bug reports — helps move it forward.

---

## 💡 What We're Building

Federel is a federated AI search protocol that enables:
- Decentralized knowledge discovery
- Private local agents
- Verified, accountable content contribution via domain ownership
- A spam-resistant, privacy-first alternative to traditional search

---

## ✅ How to Contribute

We welcome contributions in several forms:

### 📄 Documentation
- Fix typos, clarify concepts, or improve explanations in the `/docs/` folder
- Propose new specs for trust, summarization, or federation protocols

### 💻 Code
- Add or improve tools in `agents/`, `summarizer/`, `publisher/`, or `knowledge_pool/`
- Prototype agent workflows or integrate LLM APIs (OpenAI, Hugging Face, etc.)

### 🧠 Ideas / Discussions
- Use [Discussions](https://github.com/vibune/federel/discussions) to share thoughts
- Open issues for architectural questions, ethical concerns, or governance models

---

## 🖊️ Developer Certificate of Origin (DCO)

All commits must be signed off using the `Signed-off-by:` line to acknowledge you are submitting under the Apache 2.0 License.

To sign off on a commit, use the `-s` flag:

```bash
git commit -s -m "Your commit message"
```

This adds a line like:

```
Signed-off-by: Your Name <your.email@example.com>
```

If you're contributing via the GitHub web interface, include this line manually in your commit message.

---

## 🧪 Code Style & Tools

Please follow these basic guidelines when contributing code:

- ✅ Use **Python 3.10+**
- ✅ Format your code with [`black`](https://black.readthedocs.io/en/stable/)
- ✅ Lint using [`flake8`](https://flake8.pycqa.org/)
- ✅ Include **docstrings** for all public functions and classes
- ✅ Write clear, concise comments for logic that isn’t immediately obvious

---

## 🚀 Getting Started

To set up your local development environment:

```bash
# 1. Clone the repository
git clone https://github.com/vibune/federel.git
cd federel

# 2. Create and activate a virtual environment
python -m venv .venv
source .venv/bin/activate  # On Windows, use: .venv\Scripts\activate

# 3. Install development dependencies
pip install -r requirements.txt
```

> ✅ Ensure you're using **Python 3.10** or newer.

You're now ready to start building and testing locally.  
Feel free to open issues or discussions as you explore!

---

🙏 **Thanks**

Federel is an experiment in rethinking how humans — and their AIs — find and share knowledge.  
We’re glad you’re part of it.

— The Federel Team
