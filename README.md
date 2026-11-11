#  Hi, I'm Tushank Raut

 **Software Developer | Systems & MLOps Engineer | Backend Specialist**

I build scalable microservices, event-driven architectures, and high-performance machine learning serving systems. Passionate about writing clean, optimized code and architecting resilient backend infrastructure.

---

## Technical Core

| | |
|---|---|
| **Languages** | Java · TypeScript · JavaScript · Python · C++ · SQL |
| **Backend** | Spring Boot · Node.js · FastAPI · REST · Kafka · BullMQ · Microservices · Pub/Sub |
| **Data** | PostgreSQL · MongoDB · DynamoDB · Redis · ChromaDB |
| **Cloud & Ops** | AWS (Lambda, SQS, S3, API Gateway) · Terraform · Docker · GitHub Actions · OpenTelemetry · k6 |
| **AI** | RAG · XGBoost · Groq · AWS Bedrock |
| **Foundations** | Data Structures & Algorithms · DBMS · Operating Systems · Computer Networks · Distributed Systems |

---

### What I work on
 
- **Correctness under failure** — exactly-once effects via idempotent writes and the outbox pattern; retries with exponential backoff; dead-letter queues so nothing is silently dropped.
- **Performance I can measure** — indexing, caching, query tuning, then a k6 load test to confirm the P95 actually moved.
- **Infrastructure as code** — Terraform-provisioned AWS serverless stacks, Dockerised services, GitHub Actions CI.
- **Applied LLM systems** — RAG pipelines and multi-provider routing with fallback, built with the same reliability habits as any other backend.

### Featured projects
 
####  [Distributed Commerce & Billing Platform](https://github.com/tushank99/Shopify-app)
`Java` `Spring Boot` `Kafka` `Node.js` `BullMQ` `PostgreSQL` `MongoDB` `Redis` `Docker` `k6` `OpenTelemetry`
 
A multi-service commerce backend with a ledger at its core.
 
- **Ledger service (Spring Boot):** consumes transaction events from Kafka via a Node.js **transactional outbox relay**. Idempotent PostgreSQL writes prevent duplicate postings; a **dead-letter topic** captures poison messages.
- **Job processing (FastAPI + Node.js + BullMQ):** 5 concurrent workers, 3 retries with exponential backoff, DLQ — failed jobs are retried, never lost.
- **Performance:** cut MongoDB query latency **68%** by reworking aggregation pipelines and text indexes; Redis sliding-window rate limiting and 24h caching; **P95 < 300 ms at 3,000 virtual users** (k6).
- **Operability:** OpenTelemetry tracing across Java, Node.js and Python services, Actuator health endpoints, unit + integration tests in CI, and failure drills.
####  [PolicyCraft — Internal Developer Platform](https://github.com/tushank99/REPLACE-WITH-POLICYCRAFT-REPO)
`Python` `AWS Lambda` `API Gateway` `DynamoDB` `SQS` `S3` `Terraform` `GitHub Actions`
 
A serverless platform that gives developers a ready environment in seconds and stops insecure code before it builds.
 
- Terraform-provisioned stack on Lambda, API Gateway, DynamoDB and SQS — environment setup went from **hours to under 30 s**.
- LLM code generation routed through Groq with **automatic failover to AWS Bedrock** (99.9% uptime).
- **AST-based policy checks** for Python, TypeScript and Go that block hardcoded secrets and insecure dependencies pre-build.
####  [TriageFlow — AI Patient Triage](https://github.com/tushank99/REPLACE-WITH-TRIAGEFLOW-REPO)
`Python` `FastAPI` `React` `TypeScript` `XGBoost` `ChromaDB` `Groq` `PostgreSQL`
 
Explainable Emergency Severity Index (ESI) recommendations in real time.
 
- Hybrid pipeline: **XGBoost** risk prediction + **ChromaDB RAG** over historical EHR cases + **LLM reasoning** for a human-readable rationale.
- RAG workflow improved triage throughput **30%**.
- PII anonymisation, clinician-override audit trail, and tested under a **3× patient-surge** simulation.

---

### Recognition
 
- **Flipkart GRiD 8.0** — Semi-finalist among 177,000+ participants
- **Amazon ML Summer School** — Selected for the final round among 165,000+ applicants
- **Hackfest '25, IIT (ISM) Dhanbad** — Runner-up

 


---



##  Connect With Me

-  **LinkedIn:** [/in/tushankraut](https://www.linkedin.com/in/tushankraut)
-  **Email:** [tushankr0020@gmail.com](mailto:tushankr0020@gmail.com)
