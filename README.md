# Hey, I'm Rahul 👋

**AI/ML Engineer & Full-Stack Developer.** I build production applications, AI/ML products and research-oriented projects.

### How I work
I code in two modes, depending on what the project needs.

**🔧 Hand-written, when reliability is a must.**
I design the system, build the pipelines and write the code myself: clean, optimized and robust (competitive programming habits help). I like creative fixes for real problems, like cutting concert-pass QR scanning at Aura 2026 from 8s to 1s.
See it in [GitGriffin](https://github.com/Rahul-Samedavar/GitGriffin), [HTF3-Backend](https://github.com/Rahul-Samedavar/HTF3-Backend), [Prior-Guided Fusion](https://github.com/Rahul-Samedavar/ultralytics), [Adept](https://github.com/Rahul-Samedavar/Adept) and Aura (private repo).

**⚡ AI-assisted, when shipping fast is the priority.**
I use AI as a coding tool, but I still plan the system, design the pipelines, review the code, and debug or simplify it where needed. I own what I ship.


[LinkedIn](https://www.linkedin.com/in/rahul-samedavar-aa3237293) · [Email](mailto:rahulsamedavar@gmail.com) · [Hugging Face](https://huggingface.co/Rahul-Samedavar) · [DevPost](https://devpost.com/rahulsamedavar)

---

## 💼 Experience

**Data Scientist Intern, Bajaj Finserv Health** *(Jul 2026 – now)*
- Working on AI-assisted document processing and data handling, involving text processing, NER, NLP, LLMs and VLMs and Backend Dev.

**Project Lead & Backend Developer, Hack To Future 3.0** *(Apr – May 2026)*
- Ran a 24-hour national hackathon (with TCS); owned system design and deployment.
- Deployed the Node.js/PostgreSQL backend on DigitalOcean behind Nginx, with JWT auth and rate limiting.
- Designed a round-robin email OTP system handling **4,500 OTPs/day at zero cost**.

**App Developer, Aura 2026 (official tech fest, 14,000+ users)** *(Jan – Mar 2026)*
- Shipped 4 production apps: participants, admin, PR and secure entry management.
Engineered a custom QR optimization for encrypted concert passes, taking average scan time from 8s to 1s (8x faster) and keeping entry lines moving at a live concert (Mohit Chauhan) instead of crowding at the gate.
---

## 🚀 Things I've Built

### [Prior-Guided Fusion](https://github.com/Rahul-Samedavar/ultralytics) · a new YOLO architecture, built into Ultralytics
🏆 Runner-Up, Crackathon 2026 (IIT Bombay)

An original detection architecture: it fuses a handcrafted texture-anomaly prior (Gabor filters, multiscale residuals, edge suppression) into YOLO's learned features through a **learnable gate**, so the network decides how much to trust the prior at each location.

Instead of keeping it as a research script, I extended the open-source **Ultralytics** codebase to support it. I forked the framework and added custom neural-network modules and YAML model-parsing logic, so the architecture is a native, configurable model that trains with the framework's own tooling. I also built lossless pretrained-weight transfer from standard YOLO, so only the new layers start from scratch. Tested on crack detection. [Details →](https://github.com/Rahul-Samedavar/ultralytics/blob/main/docs/prior-guided-fusion/README.md)
*Python · PyTorch · Ultralytics · YOLOv8/v12*

### [ShastraDocs v2](https://github.com/Rahul-Samedavar/ShastraDocs2) · RAG over multiple documents
🏆 Hackrx 6.0 preliminary round

A RAG platform for questions over 8+ document formats. Each query is **decomposed into sub-questions**, every sub-question is retrieved independently with **hybrid search** (BM25 + semantic), and the results are **reranked** before answering.

Queries that need more than the documents go to a **one-shot agent** with web search and crawling tools.

Behind it sits a **unified LLM gateway** that routes each request to the right provider, with managed API keys, rate limits and per-provider capabilities, so the system degrades gracefully instead of failing on a rate limit.
*Python · FastAPI · LLMs*

### [Taskion](https://github.com/Rahul-Samedavar/Taskion) · a web agent built from scratch
🏆 Built for the Hackrx 6.0 finale: 2nd Runner-Up

An autonomous agent that takes a goal in plain language and carries it out by controlling and interacting with a real browser. It runs an Observe → Think → Act loop with an iteration depth limit to prevent infinite loops.

Everything is built from scratch: **no Exteranl MCP and no agentic libraries**. tool calling , agentic loop, context management,  everything was implemented from scratch.
*Python · Selenium · Gemini· Pydantic*

### [GitGriffin](https://github.com/Rahul-Samedavar/GitGriffin) · spam moderation for GitHub repos
A desktop app that cleans spam out of GitHub Discussions, Issues and Pull Requests. A **Naive Bayes classifier trained on 100,000+ GitHub comments** flags spam, and the app can hide or delete it, remove spam threads, and block spammers, using the GitHub GraphQL API and multi-threaded moderation (about 7K comments/hour per repo).

It also **learns from you**: unhiding a comment counts as a false positive and hiding a missed one counts as a false negative, and those corrections incrementally fine-tune the model to your repo.
*Python · Naive Bayes · GitHub GraphQL API · GitHub OAuth*

### [Hack To Future 3.0 Backend](https://github.com/Rahul-Samedavar/HTF3-Backend) · backend for a 650+ user national hackathon
Built and deployed solo: JWT auth, rate limiting, and **reliable PostgreSQL transactions** that kept registrations and event data consistent under heavy load. Its email OTP system is triggered through **Google Apps Script** and round-robins across multiple **.edu email accounts**, delivering **4,500 OTPs/day at zero cost**. Ran on a DigitalOcean droplet behind Nginx.
*Node.js · Express · PostgreSQL · Nginx · DigitalOcean* · [Frontend →](https://hacktofuture3.git.edu/)

**More:** [Fasal-Mitra](https://github.com/Rahul-Samedavar/Fasal-Mitra) · [Brain Tumor Detection from MRI](https://github.com/Rahul-Samedavar/Brain-Tumor-Detector-From-MRI-Scan) (research) · [CodeCanvas](https://github.com/Rahul-Samedavar/CodeCanvas) (hobby) and other repos..

---

## 🏆 Hackathon Podiums (8)

### 🥇 Winner
- **RooCode Community Hackathon (hosted via MLH, global): Best AI Hack.**
- **HackFusion 25, AGMR College of Engineering, Hubli: 1st Place.**
- **Hackfinity 2025, Tontadarya College of Engineering, Dharwad: 1st Place.**

### 🥈 Runner-Up
- **Crackathon 2026, IIT Bombay (deep-learning hackathon).** Built **Prior-Guided Fusion** for crack detection with custom YOLO architectures.

### 🥉 2nd Runner-Up
- **Convolve 4.0, Pan-IIT Hackathon, IIT Guwahati.**
- **Hackrx 6.0, Bajaj Finserv Health, finale at RVCE Bangalore.** Built **Taskion**, an autonomous web agent, for the finale. **ShastraDocs v2** (enterprise RAG) took us through the preliminary round.
- **FantomCode 2K25, RVITM.** Built **GitGriffin**, a multi-agent spam-moderation system for GitHub.
- **IEEE Clash of Code.**

*I started with ACM Nexus (college-level), where I took 1st in my first hackathon.*

---

## 🛠️ Tech Stack

- **Languages:** Python, JavaScript, Java, SQL
- **AI/ML:** PyTorch, TensorFlow, Hugging Face, LangChain, LangGraph, OpenAI & Gemini APIs, RAG, agents, NLP, computer vision (YOLO / Ultralytics)
- **Backend & infra:** FastAPI, Flask, Node.js/Express, PostgreSQL, MongoDB, Elasticsearch, Nginx, Docker, GitHub Actions, DigitalOcean
- **Frontend/mobile:** React, Expo

---

*Happy to talk about LLM systems, RAG, or building models on top of existing frameworks.*



