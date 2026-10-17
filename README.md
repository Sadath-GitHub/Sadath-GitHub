<h1 align="center">Mohammed Sadath Khan</h1>
<p align="center">
  <b>Backend & distributed systems engineer</b> · payments, fintech, GenAI<br>
  5+ years at Flipkart & Yubi · MS CS @ UALR (4.0 GPA)
</p>

<p align="center">
  <a href="https://mohammedsadathkhan-portfolio.netlify.app/"><img src="https://img.shields.io/badge/Portfolio-000?style=for-the-badge&logo=safari&logoColor=white"></a>
  <a href="https://www.linkedin.com/in/mohammed-sadath-khan-328188137/"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a>
  <a href="https://leetcode.com/u/Mohammed_Sadath_Khan/"><img src="https://img.shields.io/badge/LeetCode-FFA116?style=for-the-badge&logo=leetcode&logoColor=black"></a>
  <a href="mailto:mohammedsadathkhan123@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white"></a>
</p>

---

## Impact, in numbers

| | What I built | Where |
|---|---|---|
| 💸 **$5M / year saved** | Wallet write-off flow to reconcile unrecoverable payment amounts | Flipkart |
| 🛒 **$1B in sales handled** | Migrated payment services from VMs to Kubernetes and load-tested for Big Billion Days | Flipkart |
| 📈 **+$50K / month revenue** | Temporal + Kafka framework for resilient bulk-file processing | Yubi |
| 🔔 **500K+ pushes / month** | Firebase-based push notification framework (mobile + web) | Yubi |
| 📉 **-25% infra cost** | Led Golang → Java migration of a notification service, removed AWS Lambda | Yubi |

---

## How I think about systems

**Resilient bulk processing** (the pattern behind the Temporal framework)

```mermaid
flowchart LR
    A[Kafka message] --> B[Temporal workflow]
    B --> C[Worker builds output file]
    C --> D{Per-row tasks}
    D -->|configurable| E[Row task 1..n]
    E --> F[Output file]
    B -. retries/durability.-> C
```

**Real-time vendor failover**

```mermaid
flowchart LR
    R[Request] --> S[Redis sorted set: vendors ranked by live failure rate]
    S --> V[Top-ranked vendor]
    V -->|success / failure metric| S
    S -. durable state .-> P[(PostgreSQL)]
```

*(Conceptual diagrams of patterns I've designed, not proprietary code.)*

---

## Things I build on my own

- 🎬 **[AdSlot AI](LINK)**: FastAPI + Whisper + Claude API that analyzes video transcripts and recommends optimal ad-break timestamps. Deployed.
- 🛡️ **[Incident-Based Risk Assessment](LINK)**: LangGraph + RAG pipeline that compares code changes against historical incidents in a vector DB, flags risky deploys, auto-approves safe ones.
- 🔐 **[PrivacyGuard](LINK)**: Python/FastAPI on Kubernetes. Pulls from search, social, and breach sources (HaveIBeenPwned) and uses LLMs to generate weighted PII exposure reports.
- ⚙️ **[MarketGen](LINK)**: n8n + Supabase marketing automation that generates on-brand images, blogs, and videos with LLMs.

---

## Stack

<details open>
<summary><b>Core</b></summary>

`Java` `Go` `Python` `SQL` · `Spring Boot` `FastAPI` · `Kafka` `Temporal` `Redis` · `PostgreSQL` `MongoDB`
</details>

<details>
<summary><b>Infra & quality</b></summary>

`AWS` `Docker` `Kubernetes` `Jenkins` `Grafana` · `JUnit` · load & performance testing
</details>

<details>
<summary><b>GenAI</b></summary>

`LangGraph` `LangChain` `RAG` `Pinecone` `Claude API` `n8n`
</details>

---

## Right now

🎓 Finishing my MS in CS at UALR (May 2027)
🔭 Building GenAI tooling and distributed systems projects
💼 Open to full-time SWE / Lead roles, backend and distributed systems
