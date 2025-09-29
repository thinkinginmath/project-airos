# Project Airos Website Specification

## Overview
The Project Airos website is the public-facing home for an **open-source AI Agent OS** designed for client devices (phones, PCs, smart glasses, and future edge devices). The site will:
- Communicate the **vision**: privacy-first, local + edge inference, sovereign AI.
- Provide **resources** for developers, researchers, and contributors.
- Act as a **hub** for community, docs, and code.
- Showcase **flagship demo applications** (Smart Glasses, AI for Education).

---

## Structure

### 1. Landing Page
- **Hero section**:  
  - Project name + tagline (e.g., *“Airos: Sovereign AI, in your hands”*).  
  - Short description: open-source AI Agent OS for client-side devices.  
  - Call-to-action buttons: *Get Started*, *Join Community*, *GitHub*.  
- **Key Features**:  
  - Privacy-first, local + edge inference.  
  - Voice-first UI (ASR + TTS).  
  - Portable memory (short + long term).  
  - Open-source stack (LLMs, ASR, TTS, orchestration).  
- **Vision Statement**:  
  - How Airos differs from Meta Aria / Google Astra.  
  - Sovereign AI principle.  
- **Flagship Demos**: Smart Glasses + AI for Education (with links to detail pages).

### 2. About
- The problem with current AI ecosystems (cloud-only, vendor lock-in, privacy risks).  
- Our solution: open, community-driven, local-first.  
- Roadmap of the project.  

### 3. Technology
- Architecture diagram: Cloud + Edge + Device hybrid.  
- Modules:  
  - ASR (FunASR, Whisper)  
  - TTS (PrimeSpeech, etc.)  
  - LLM Orchestration (MCP, vLLM, Dora)  
  - Memory layer (local vector DB).  
- Supported devices: smartphones, PCs, smart glasses.  

### 4. Applications
- **Smart Glasses Agent**  
  - Inspired by Meta Aria & Google Astra but open + privacy-first.  
  - Voice-first interaction (ASR/TTS).  
  - Vision Q&A (photo capture → ask question).  
  - Local-first with privacy controls (shutter, LED, user-owned memory).  
- **AI for Education Tutor**  
  - Personalized, Socratic-style tutoring.  
  - Hybrid deployment (on-device for students, edge for schools).  
  - Local/portable memory for progress tracking.  
  - Designed for underserved communities with privacy and equity.  

### 5. Community
- Links to GitHub repo.  
- How to contribute (issues, PRs, discussions).  
- Code of Conduct.  
- Mailing list / Discord / Slack (to decide).  

### 6. Documentation
- Quickstart (install on phone/PC).  
- Running Airos with Docker.  
- Using Airos with LLM APIs (OpenAI Realtime, Qwen, LLaMA).  
- Extending modules (add new ASR, TTS, LLM backends).  
- Use cases: Smart Glasses & Education demos.

### 7. Blog / Updates
- Release announcements.  
- Tutorials.  
- Partner contributions.  
- Conference talks (e.g., GOSIM Hangzhou 2025).  

### 8. Contact
- Team intro.  
- Email contact.  
- Press/media kit.  

---

## Technical Requirements

- **Framework**: Next.js or Astro (static-friendly + supports Markdown docs).  
- **Styling**: TailwindCSS or CSS modules for flexibility.  
- **Docs**: Use Markdown-based system (MDX or Docusaurus-style).  
- **Hosting**: GitHub Pages / Vercel / Netlify for CI/CD.  
- **SEO**: Basic metadata (open graph, keywords, sitemap).  

---

## Domain & Branding

- Preferred: **airos.org** (community identity)  
- Alternatives: airos.ai, airos.io, projectairos.com  
- Branding: clean, modern typography, privacy/security color palette (deep blue, green, white).  

---

## Initial Pages to Implement

- `/` → Landing page  
- `/about` → Vision & background  
- `/tech` → Technology overview  
- `/applications` → Smart Glasses + Education Tutor use cases  
- `/docs` → Quickstart + Developer Docs  
- `/community` → Contribution guidelines  
- `/blog` → News & updates  
- `/contact` → Contact form  

---

## Future Extensions

- API playground for voice chat demos (WebRTC/WebSocket).  
- Interactive diagram of local + edge + cloud workflow.  
- Showcase of partner projects and use cases.  

