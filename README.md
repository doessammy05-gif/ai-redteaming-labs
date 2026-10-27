# LLM Security & Red-Teaming Research 🛡️🤖

This repository serves as a portfolio of my research into the vulnerabilities of Large Language Models (LLMs) and Agentic Systems. My focus is on identifying "jailbreaks," prompt injection vectors, and data leakage in RAG (Retrieval-Augmented Generation) architectures.

## 🎯 Research Focus
- **Prompt Injection:** Direct and Indirect attacks to bypass system constraints.
- **Data Exfiltration:** Extracting system prompts or sensitive training data via iterative probing.
- **Agentic Abuse:** Testing tool-use boundaries and privilege escalation in AI Agents.
- **OWASP LLM Top 10:** Mapping findings to the industry-standard vulnerability framework.

## 📂 Case Studies
Detailed walkthroughs of simulated attacks can be found in the `/cases` directory:
- [Prompt Injection & Guardrail Bypass](./cases/prompt-injection.md)
- [RAG Vector Store Exfiltration](./cases/rag-exfiltration.md)

## 🛠️ Tooling
Included in `/tools` is a basic PoC scanner used to automate the detection of system prompt leakage.

---
*Disclaimer: All research conducted in controlled environments for educational and security improvement purposes.*