# Project Airos

**Sovereign AI, in your hands.**  
Project Airos is an **open-source AI Agent OS** designed for client devices — phones, PCs, smart glasses, and future edge hardware.  
Our mission is to make **privacy-first, local + edge inference AI agents** accessible to everyone.

---

## ✨ Vision

AI is rapidly becoming the *operating layer* for daily life. But today’s ecosystems are closed, cloud-dependent, and vendor-controlled.  
**Airos** takes a different path:

- **Sovereign AI:** Your agent, your data, your memory.  
- **Local-first:** Inference on-device or at the edge, with cloud as an option.  
- **Portable memory:** Short-term + long-term user memory, stored under user control.  
- **Voice-first:** Combining GUI + VUI for natural multimodal interaction.  
- **Open-source:** Transparent, auditable, and community-driven.

---

## 🏗️ Architecture

Airos is built as a **hybrid stack**:

- **Frontend:** Voice, text, and GUI interfaces on phones, PCs, and smart devices.  
- **Core:** Multi-provider LLM orchestration via [MCP](https://github.com/modelcontextprotocol), Dora (Rust), vLLM, etc.  
- **ASR / TTS:** Whisper, FunASR, PrimeSpeech, and other pluggable backends.  
- **Memory:** Local vector DBs for contextual, portable user memory.  
- **Deployment:** Cloud + Edge + Device — user chooses the level of privacy and cost.  

---

## 🚀 Quickstart

Coming soon — in the meantime:

1. Clone this repo.  
2. Install dependencies (Docker / Node.js / Python).  
3. Run the local agent example.  
4. Connect to your LLM API provider (OpenAI, Anthropic, Qwen, LLaMA, etc.).  

Check [docs/](docs/) for early developer documentation.

---

## 🌐 Roadmap

- [ ] Voice-first client (ASR + TTS + chat loop).  
- [ ] Local memory service with vector DB.  
- [ ] Multi-provider LLM orchestration.  
- [ ] Smart glasses prototype integration.  
- [ ] Secure containerized deployment for schools & enterprises.  

See [issues](../../issues) for the latest milestones.

---

## 🤝 Community

We welcome contributions from researchers, developers, and educators:

- 📂 [GitHub Issues](../../issues) — file bugs, feature requests, and proposals.  
- 💬 Discussions (coming soon).  
- 📧 Contact: info@projectairos.org  

Please read our [Code of Conduct](CODE_OF_CONDUCT.md) before contributing.

---

# Sample Applications

While Project Airos is a general **AI Agent OS for client devices**, we highlight two flagship applications that demonstrate its potential:

---

## 🕶️ Smart Glasses (Inspired by Meta Aria & Google Astra)

**The Challenge:**  
Meta's *Project Aria* focused on AR sensor research.  
Google's *Project Astra* showcased real-time multimodal AI, but cloud-first and proprietary.  

**Airos Approach:**  
- **Local-first inference:** voice commands and wake word handled on-device.  
- **Photo capture + Vision Q&A:** take a picture and ask questions (“What does this sign mean?”).  
- **Voice-first interaction:** natural speech loop with cloud/edge LLMs.  
- **Privacy by design:** camera shutter indicator, mic/cam hardware switches, user-controlled memory.  
- **Open source stack:** Whisper/FunASR for ASR, PrimeSpeech TTS, LLMs via MCP/vLLM.  

Smart glasses become the **reference demo hardware** for Project Airos — showing what’s possible when privacy and openness are core principles.

---

## 🎓 AI for Education

**The Challenge:**  
Millions of students lack access to affordable, high-quality tutoring.  
Current AI solutions are cloud-only and raise concerns about equity and privacy.  

**Airos Approach:**  
- **Personalized AI tutor** with Socratic dialogue style, built on Airos agents.  
- **Portable student memory:** progress and misconceptions tracked locally, sharable with teachers if allowed.  
- **Hybrid deployment:** schools can run Airos on local servers (edge) to avoid data leakage.  
- **Open ecosystem:** supports open LLMs and ASR/TTS in multiple languages.  

Education becomes a **high-impact domain application** for Airos, proving how sovereign AI can deliver equitable and private learning support.

---

## Why These Matter

- **Smart glasses** = cutting-edge, wearable showcase of what local-first agents can do.  
- **Education AI** = socially impactful use case that resonates globally.  

Together, they show how **Airos can power both futuristic devices and practical daily learning.**

## 📜 License

MIT License. See [LICENSE](LICENSE) for details.

---

## 🙏 Acknowledgements

Built on the shoulders of open-source giants:
- [Whisper](https://github.com/openai/whisper), [FunASR](https://github.com/alibaba-damo-academy/FunASR)  
- [vLLM](https://github.com/vllm-project/vllm), [Model Context Protocol](https://modelcontextprotocol.io/)  
- [Dora](https://github.com/dora-rs/dora) and more.

---

**Project Airos**: building an **open, sovereign AI Agent OS** for the next generation of devices.


