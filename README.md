# Aidan Eckfeldt

**CS + Math @ Penn State** · I build internal tooling that other teams actually run on.

[LinkedIn](https://linkedin.com/in/aidaneckfeldt) · [Email](mailto:aidan@eckfeldt.com) · Manhattan / State College

---

Most of my work sits at the boundary between a model and a real business process: talking to the people who do the work, finding where the friction actually is, and shipping something into their workflow that holds up under real data. Right now that means AI tooling for clinical and operational teams at NYU Langone Health, and a multi-tenant analytics platform I build end to end as technical co-founder.

I care about correctness you can prove rather than correctness you hope for — schema-constrained model output, deterministic services around the LLM, and gates that reject bad generations before a user ever sees them.

---

## Currently

**NYU Langone Health** — AI/Automation Intern, MCIT · *Manhattan, NY · Summer 2026*
Building and deploying AI tooling for clinical and operational teams inside the hospital system. Previously (Summer 2025) on the Campus Transformation IT PMO team, where I:
- Surveyed 30 project managers and shadowed their workflows to find where AI could remove repetitive work
- Identified procurement intake as the highest-impact target — PMs were hand-assembling forms from documentation, vendor quotes, and agreements, producing slow and inconsistent submissions to Finance and Legal
- Mapped the intake process end to end with Finance and Legal, then built a guardrailed LLM workflow that extracts and standardizes procurement data into a structured package for PM review, cutting prep from days to minutes

**THON Technology** — Technology Captain · *Penn State · May 2025 – Feb 2027*
Cloud and systems infrastructure for the world's largest student-run philanthropy.
- Traced ~10 minute CI builds on one-line commits to full image rebuilds on every push in a legacy, high-turnover codebase; added Docker layer caching and cut build times roughly in half
- Audited AWS (EC2, S3, container images) to decommission unused resources and cut monthly compute spend ahead of THON Weekend
- Own cloud and security operations across AWS, CI/CD, and IAM for year-round production systems
- Engineered full-stack features for the public THON Store (Django, Vue, Wagtail) handling 15,000+ annual orders for a community of 50,000+

---

## Selected Work

### Mandate — Multi-tenant AI analytics platform
*TypeScript · Fastify · React · Supabase · BullMQ · Redis · Anthropic SDK*
**Technical Co-Founder** · 2026 · *private*

- Architected the full stack: a TypeScript/Fastify backend on Supabase with row-level security and JWT-tested data isolation per client organization
- Designed an **LLM-narrates-never-calculates** architecture that enforces correctness mechanically — a PII-stripping boundary so client data never reaches the model, a closed prompt schema, and a 10-check gate that rejects hallucinated output
- Built tested deterministic services for scoring, segmentation, and confidence-tier ranking, plus a queued memo-generation pipeline on BullMQ and Redis

### uPR — iOS strength analytics
*React · TypeScript · Capacitor*
**Creator** · 2025 · **[Live on the App Store](https://apps.apple.com/app/id0000000000)**

- Shipped solo to the App Store: workout logging, trend tracking, and predictive performance insights
- Built a predictive analytics engine with real-time PR detection and estimated 1RM calculation on top of a structured workout/set/rep/load data model designed for long-term consistency
- Mobile-first UI tuned for fast entry mid-workout, with Recharts dashboards for post-session analysis

### MyCord — TCP chat client in C
*C · POSIX sockets · pthreads*
**Creator** · 2025

- Implemented a custom binary protocol (LOGIN, MESSAGE_SEND, MESSAGE_RECV, SYSTEM, DISCONNECT) over packed structs with fixed 1064-byte framing
- Multithreaded architecture separating async message receipt from local input, with graceful shutdown on SIGINT/SIGTERM/EOF and automatic logout dispatch
- Buffered read logic tolerant of partial packets, `EINTR`, and socket edge cases — no crashes across thousands of messages

### Phil or No Phil — Prediction market
*Next.js 14 · TypeScript · Prisma · PostgreSQL · Vercel*
**Creator** · 2025 · *[live](https://philornophil.com)*

- Built a working prediction market for friends: auth, market creation, YES/NO shares, dynamic pricing, admin resolution
- Took it idea to production solo — Prisma Postgres, env config, Vercel deploy, custom domain

---

## Also

**Nittany AI Machine Learning Bootcamp** · Jan – Apr 2026
Selected from 200+ applicants. Built end-to-end PyTorch pipelines across regression, classification, neural networks, RAG, and fine-tuning; shipped fraud detection, digit recognition, and an LLM retrieval system. Competed in the Nittany AI Challenge.

**Learning Assistant, Calculus** · Penn State
Led small-group sessions and office hours for undergraduate calculus.

---

## Tools

**Languages** Python · TypeScript · C · Java · SQL
**Backend & Data** Fastify · Django REST · Supabase/Postgres · Prisma · Redis · BullMQ · REST APIs
**Frontend** React · Vue · Next.js · Capacitor
**Infra** AWS (ECS, ECR, EC2, S3, CloudFront) · Docker · CI/CD · IAM
**AI/ML** PyTorch · Hugging Face · Anthropic SDK · RAG · fine-tuning · evaluation

Currently working on: Go, and getting more comfortable in systems-level territory beyond C.

---

## Education

**Pennsylvania State University**, College of Engineering — *December 2027*
B.S. Computer Science · Minors in Artificial Intelligence and Mathematics · GPA 3.6
MLK Jr. Scholarship Recipient · Dean's List

---

If you're working on deployed AI systems, healthcare infrastructure, or internal tooling that people depend on, I'd be glad to talk — **aidan@eckfeldt.com**
