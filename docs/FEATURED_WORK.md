# Featured Work

A closer look at the projects I've put the most time into — spanning AI-powered products, computer vision research, and applied ML.

---

## Roam

**Timeline:** 2025 – Present
**Stack:** Swift, AVAssetImageGenerator, Vision LLMs, FastAPI, PostgreSQL, Google Maps API

AI-powered travel and social-planning app that converts short-form video inspiration (think: a friend's travel reel) into structured planning data.

- Built iOS video/reel ingestion with frame extraction and confidence-scored location/activity extraction
- Resolved extracted locations against the Google Maps API for real places, not just guesses
- FastAPI + PostgreSQL backend for recommendations, shared maps, and calendar-aware planning

**Links:** [GitHub](https://github.com/omondistanley/roam-mvp) · [Live](https://roam-alpha.web.app/) · [TestFlight](https://testflight.apple.com/join/CHpUX4F4)

---

## Pocketii

**Timeline:** 2024 – 2026
**Stack:** Python, FastAPI, PostgreSQL, Redis, Docker, JWT, background jobs

Production-grade personal finance platform — expense tracking, budgets, investment monitoring, and AI-powered financial insights, with an emphasis on reliable transaction data.

- Authenticated bank integrations (Plaid, Teller, TrueLayer) with idempotent ingestion and provider failover so a flaky feed doesn't corrupt a user's ledger
- Background job processing for spending-anomaly detection and expense forecasting
- Shared household finances, savings goals (including round-up micro-savings), and recurring-transaction management
- Deployed with a live production app and a sandboxed interactive demo (no account needed, resets every 15 minutes)

**Links:** [GitHub](https://github.com/omondistanley/pocketii) · [Live App](https://pocketii.fly.dev/landing) · [Interactive Demo](https://pocketii.onrender.com)

---

## Creatures in the TV (CITV)

**Timeline:** 2026 — Columbia University, DAPLab
**Stack:** Python, PyTorch, SAM2, GroundingDINO, Florence-2, RAM++, Depth Anything V2, CUDA/MPS

Research pipeline for context-aware creature insertion: converts a single RGB image into metric depth, instance masks, semantic labels, spatial relations, and a depth-backed 2D/3D scene graph — entirely local, no paid APIs.

- Orchestrated multiple vision models (depth, detection, segmentation, semantic labeling) into one pipeline with shared device routing across CUDA/CPU/Apple MPS
- Built geometry-hardening steps — adaptive mask erosion, sigma clipping, mode-based depth estimation — to make per-object 3D estimates robust to noisy masks
- Prototyped depth-clustered regions, mask hierarchies, and traversability cost fields to support ranked path hypotheses for animated agents moving naturally through a scene

**Links:** [GitHub](https://github.com/omondistanley/citv)

---

## Knowledge Distillation for Scalable Mixture-of-Experts (MistralMoE)

**Timeline:** 2025 - 2026
**Stack:** Python, PyTorch, Transformers, PEFT/LoRA, Weights & Biases

Research framework converting **Mistral-7B** into sparse Mixture-of-Experts architectures via sparse upcycling and knowledge distillation, benchmarked on MMLU across 10+ architectural variants.

- **Key finding:** sparse upcycling alone cuts FLOPs by ~65.6% (8,796G → 3,024G) while exactly preserving dense MMLU accuracy — with zero training
- Standard fine-tuning then pushed MoE to 69.70% MMLU (+4.97% over the 66.40% dense baseline)
- Counter-intuitive result: knowledge distillation from the dense teacher *degrades* MoE accuracy in most variants, unless the architecture explicitly protects expert diversity (router jitter, distributed expert placement) against the teacher's pull toward non-MoE behavior

**Links:** [GitHub](https://github.com/omondistanley/MistralMoE) · [Paper](https://github.com/omondistanley/MistralMoE/blob/master/MoE%20Final%20Paper.pdf)

---

## Neural Volume Rendering

**Timeline:** 2026
**Stack:** Python, PyTorch, NeRFs, differentiable rendering, 3D reconstruction

Graphics/ML case study in neural scene representation — differentiable volume rendering, camera-ray geometry, and transfer-learning workflows for 3D reconstruction, sitting alongside CITV in my broader visual-computing work.

**Links:** [GitHub](https://github.com/omondistanley/Neural-Volume-Rendering)

---

## Image Captioning with LSTM

**Timeline:** 2025
**Stack:** Python, PyTorch, TorchVision, ResNet-18, LSTM

Conditioned LSTM language model that generates natural-language captions for Flickr8k images by combining pretrained ResNet-18 visual features with a sequence model trained on human-written captions.

- Implemented greedy, sampling, and beam-search decoders for caption generation
- Trained with padding/masking on variable-length caption sequences

**Links:** [GitHub](https://github.com/omondistanley/Image-captioning-using-LSTM)

---

## 2048 AI Solver

**Timeline:** 2025
**Stack:** Python, search, expectiminimax, alpha-beta pruning

AI decision engine for 2048 using iterative-deepening expectiminimax with probabilistic tile modeling and a heuristic evaluation function over empty tiles, monotonicity, smoothness, corner placement, and merge potential.

**Links:** [GitHub](https://github.com/omondistanley/2048-Puzzle-AI-Agent-Solver) · [Live](https://2048-puzzle-ai-agent-solver.fly.dev/)

---

## Other Notable Repos

- **[anchorpoint](https://github.com/omondistanley/anchorpoint)** — Monorepo for a mobile-first building help desk: Expo (React Native + TypeScript) client, FastAPI + PostgreSQL + Redis API, SLA-escalation background workers, and a public situational-summary feed.
- **[generative-camera-dolly](https://github.com/omondistanley/generative-camera-dolly)** — Video preprocessing pipeline for generative/graphics work: frame extraction, COLMAP camera-pose estimation, optical flow, MiDaS depth estimation, and semantic segmentation (Mask2Former/DeepLabV3).
- **Rhythmic** — Team project on a music-oriented product, focused on team delivery and testing as part of a larger engineering team.

---

**See also:** [About](./ABOUT.md) · [Experience](./EXPERIENCE.md) · [Tech Stack](./TECH_STACK.md) · [Programs & Training](./PROGRAMS_AND_TRAINING.md)
