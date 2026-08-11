# Experience & Work History

## Columbia University — DAPLab
**Undergraduate Researcher | Creatures in the TV**  
*January 2026 – May 2026 | New York City, NY*

**Focus:** Computer vision pipeline development and scene-graph generation from RGB images

**Key Responsibilities:**
- **Owned the computer-vision track**, converting single RGB images into metric depth, instance masks, semantic labels, relations, and depth-backed 2D/3D scene graphs
- **Vision Model Integration:** Deployed cutting-edge models locally with no paid APIs:
  - Depth Anything V2 for monocular depth estimation
  - GroundingDINO for open-vocabulary object detection
  - SAM2 for instance segmentation
  - Florence-2 for semantic understanding
  - RAM++ for region attribute modeling
  
- **Geometry Hardening:** Implemented robust preprocessing pipelines:
  - Adaptive erosion for per-mask geometry refinement
  - Sigma clipping for outlier handling
  - Mode-based depth estimation for robustness
  - Paired statistics (with/without-erosion) to expose preprocessing sensitivity

- **Geometric Reasoning:** Prototyped advanced scene representations:
  - Depth-clustered regions for spatial partitioning
  - Mask hierarchies for relationship understanding
  - Traversability cost fields for navigation reasoning
  - Ranked path hypotheses with QA artifacts for validation

- **Performance Optimization:** Hardened inference across multiple backends:
  - Shared device routing for CUDA, CPU, and Apple MPS
  - Depth caching to reduce redundant computation
  - Inter-stage model unloading to manage memory
  - Significantly reduced VRAM pressure and runtime failures

**Technical Stack:** Python, PyTorch, Vision Transformers (Depth Anything, GroundingDINO, SAM2, Florence-2, RAM++), CUDA, Apple MPS, GPU optimization, scene graph representation

**Key Learnings:**
- Production-grade computer vision pipeline design
- Multi-backend optimization and cross-platform performance
- Robust preprocessing for geometric data
- Failure mode analysis and documentation
- Local deployment strategies for cutting-edge models

**What it demonstrates:**
- Vision model orchestration and integration
- GPU/CPU/MPS performance optimization
- Rigorous engineering and preprocessing discipline
- Spatial reasoning and scene understanding
- Handling of edge cases (occlusion, support surfaces, motion naturalness)

---

## Oracle — Solutions Engineering Intern

**Focus:** AI-assisted workflows for enterprise HCM systems

**Key Responsibilities:**
- Built AI-assisted workflows for Oracle Fusion HCM Fast Formula creation, debugging, and explanation
- Worked across HCM Extracts, PL/SQL, Redwood UX, and regression testing
- Delivered client adoption demos showing practical value of AI enhancements
- Supported enterprise service-request triage:
  - Reproduced issues from customer reports
  - Validated fixes and coordinated with development teams
  - Understood enterprise HCM implementation constraints and customer needs

**Technical Stack:** Oracle Fusion, PL/SQL, Fast Formula, HCM systems, Redwood UX, testing automation

**Key Learnings:**
- Enterprise software complexity and customer support workflows
- How AI can enhance developer productivity in domain-specific systems
- Importance of validation and regression testing at scale
- Translating customer problems into actionable engineering work

---

## Columbia Build Lab / Sachi Health — Fullstack Software Engineer

**Focus:** RAG pipelines and AI-assisted clinical data workflows

**Key Responsibilities:**
- Engineered RAG/data pipelines that parsed unstructured clinical-trial documents into structured data:
  - Eligibility criteria extraction
  - Intervention and outcome normalization
  - Structured recommendation data generation
- Built React Native/TypeScript visualization screens for MVP testers
- Researched HIPAA-aware recommendation logic and compliance workflows
- Designed qualitative evaluation workflows for AI-assisted clinical matching

**Technical Stack:** Python, RAG frameworks, React Native, TypeScript, clinical data standards, LLM integration

**Key Learnings:**
- Healthcare domain knowledge and HIPAA compliance requirements
- How to structure unstructured data for ML systems
- RAG system design and knowledge base optimization
- Qualitative evaluation methods for AI systems
- Working with domain experts and regulatory constraints
- Balancing technical solutions with real healthcare workflows

---

## Columbia University — Undergraduate Research in Visual Computing

**Project:** Creatures in the TV (CITV) - Early Research Phase

**Focus:** Scene-aware visual computing for inserting animated agents into video/art scenes

**Key Responsibilities:**
- Built scene-understanding pipelines for visual comprehension
- Implemented mask-based segmentation and depth estimation workflows
- Developed semantic labeling and scene graph construction
- Explored motion-path constraints and interaction design
- Optimized performance across GPU/CPU/MPS platforms

**Technical Stack:** Python, OpenCV, Vision Transformers, CUDA, GPU optimization, scene representation

**Key Learnings:**
- Research methodology and experimental design
- GPU optimization and real-time system constraints
- Visual understanding and computer vision pipelines
- How to balance theoretical research with practical implementation
- Comfort with ambiguous research problems and iterative refinement

---

## Additional Involvement

### Teams & Communities
- **ColorStack Member** — technical community for Black and Latinx technologists
- **PwC / Paragon One Remote Extern** — consulting-style research and problem framing
- **Goldman Sachs Virtual Insight Series** — financial services exposure

### Product Engineering
- **Rhythmic** (team project) — contributed to music-oriented product with focus on team delivery and testing

---

## Skills Developed Across Roles

| Category | Skills | Evidence |
|----------|--------|----------|
| **Backend** | System design, API development, data pipelines, RAG systems | Pocketii, Sachi Health, Oracle |
| **Frontend** | React, React Native, TypeScript, UX thinking | Roam, Sachi Health, Rhythmic |
| **ML/AI** | LLM workflows, vision models, fine-tuning, evaluation | MistralMoE, CITV, Roam, Image Captioning |
| **Data** | Pipeline design, unstructured-to-structured transformation | Sachi Health, Pocketii |
| **Cloud & DevOps** | Docker, Google Cloud, CI/CD, environment management | Roam, Pocketii |
| **Computer Vision** | Multi-model orchestration, depth estimation, segmentation, optimization | DAPLab/CITV |
| **Domain Knowledge** | Healthcare (HIPAA), Enterprise (HCM), Finance, Graphics, Vision | Oracle, Sachi Health, Pocketii, CITV |
| **Team Collaboration** | Code review, sprint planning, cross-functional coordination | Rhythmic, team internships |

---

## What I'm Looking For Next

Roles where I can:
- Build technical systems that connect messy real-world inputs to useful products
- Work on infrastructure, research prototypes, or AI products
- Collaborate with talented teams across engineering, product, and design
- Take on problems that require both technical depth and product judgment
- Continue growing in backend systems, AI/ML, computer vision, and platform engineering
