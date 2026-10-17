<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f2027,50:203a43,100:2c5364&height=200&section=header&text=Mohammed%20Sadath%20Khan&fontSize=42&fontColor=ffffff&fontAlignY=38&desc=Backend%20%26%20Distributed%20Systems%20Engineer&descSize=18&descAlignY=58" />

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=18&duration=3000&pause=1200&color=38BDF8&center=true&vCenter=true&width=700&lines=Payments+%C2%B7+Fintech+%C2%B7+GenAI;5%2B+years+at+Flipkart+%26+Yubi;Building+resilient+systems+at+scale;MS+CS+%40+UALR+%7C+4.0+GPA" />

<br><br>

<a href="https://mohammedsadathkhan-portfolio.netlify.app/"><img src="https://img.shields.io/badge/Portfolio-0f2027?style=for-the-badge&logo=safari&logoColor=white"></a>
<a href="https://www.linkedin.com/in/mohammed-sadath-khan-328188137/"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a>
<a href="https://leetcode.com/u/Mohammed_Sadath_Khan/"><img src="https://img.shields.io/badge/LeetCode-FFA116?style=for-the-badge&logo=leetcode&logoColor=black"></a>
<a href="mailto:mohammedsadathkhan123@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white"></a>

</div>

---

## 📈 Impact

<div align="center">

![saved](https://img.shields.io/badge/%245M-saved_per_year-22c55e?style=for-the-badge)
![sales](https://img.shields.io/badge/%241B-sales_handled-3b82f6?style=for-the-badge)
![revenue](https://img.shields.io/badge/%2B%2450K-revenue_per_month-a855f7?style=for-the-badge)
![push](https://img.shields.io/badge/500K%2B-pushes_per_month-f59e0b?style=for-the-badge)
![cost](https://img.shields.io/badge/-25%25-infra_cost-ef4444?style=for-the-badge)

</div>

| | What I built | Where |
|---|---|---|
| 💸 | Wallet write-off flow to reconcile unrecoverable payment amounts | Flipkart |
| 🛒 | Moved payment services from VMs to Kubernetes, load-tested for Big Billion Days | Flipkart |
| 📈 | Temporal + Kafka framework for resilient bulk-file processing | Yubi |
| 🔔 | Firebase push framework (mobile + web) | Yubi |
| 📉 | Golang → Java migration of the notification service, killed AWS Lambda | Yubi |

---

## 🧠 How I design systems

```mermaid
flowchart LR
    K[Kafka message] --> T[Temporal workflow]
    T --> W[Worker builds output file]
    W --> R{Per-row tasks}
    R --> O[Output file]
    T -. retries and durability .-> W
```

```mermaid
flowchart LR
    Q[Request] --> Z[Redis sorted set<br/>vendors ranked by live failure rate]
    Z --> V[Best vendor]
    V -->|success / failure| Z
    Z -. durable state .-> P[(PostgreSQL)]
```

<sub>Conceptual patterns, not proprietary code.</sub>

---

## 🚀 Projects

<div align="center">

<a href="https://github.com/Sadath-GitHub/AdSlot-AI"></a>
<a href="https://github.com/YOUR_USERNAME/RISK_REPO"></a>
</div>

- 🎬 **AdSlot AI**: FastAPI + Whisper + Claude API, recommends ad-break timestamps from video transcripts
- 🛡️ **Incident Risk Assessment**: LangGraph + RAG flags risky deploys against past incidents
- 🔐 **PrivacyGuard**: LLM-generated PII exposure reports on Kubernetes
- ⚙️ **MarketGen**: n8n + Supabase content automation for images, blogs, videos

---

## 🛠️ Stack

<div align="center">

<img src="https://skillicons.dev/icons?i=java,go,py,spring,fastapi,kafka,redis,postgres,mongodb,aws,docker,kubernetes,jenkins,grafana,git&perline=15" />

<sub>Temporal · LangGraph · LangChain · RAG · Pinecone · Claude API · n8n · Supabase</sub>

</div>
