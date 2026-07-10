---
title: "Event 2 - AWS Vietnam Community Day 2026"
date: 2026-05-23
weight: 2
chapter: false
pre: " <b> 4.2. </b> "
---

| Information | Details |
|---|---|
| Date | 23/05/2026 |
| Location | 26th Floor, Bitexco Financial Tower, Saigon Ward, Ho Chi Minh City |
| Role | Attendee |

This page summarizes the presentation contents at **AWS Vietnam Community Day 2026**, covering AI context design, edge infrastructure, hackathon experience, LLM reliability, and enterprise-grade multi-agent systems.

---

### General Focus

> AI is not just a tool for demos. AI requires clear context, architecture, and deployment workflows.

- AWS serves as the foundation for AI infrastructure, security, operations, and scaling
- The presentations all emphasized practicality: from prompts, hackathons, and CloudFront to enterprise-grade multi-agent systems

---

### 1. Introduction

AWS Vietnam Community Day 2026 gathered experts to share practical experiences in building AI and cloud systems on AWS. The topics spanned from personal productivity with AI, enterprise assistant tools, CDN infrastructure, product development in hackathons, LLM reliability challenges, to enterprise-grade multi-agent credit scoring systems.

---

### 2. Summary of Presentations

#### 2.1 Tinh Truong - Build Second Brain

The session focused on how to work effectively with AI through **context management**. The speaker emphasized that current AI models are highly capable, but results are often poor because users either fail to provide sufficient context or include context that misses the core focus.

**A good context needs:**
- Objective to be achieved
- Current situation
- Technical constraints
- Relevant evidence or data

**Common mistakes:**
- Providing too many unselected documents
- Copy-pasting raw, lengthy files
- Merely restating obvious facts that the AI already knows

**Core principle:**
> Context quality is more important than context quantity.

**Second AI Brain concept:**
This is a personal knowledge management system that helps you recall project details and retrieve the correct information before prompting the AI.

**Key takeaway:** A skilled AI user is one who knows how to transform a vague request into a task with clear goals, data, and outputs.

---

#### 2.2 Pham Nguyen Hai Anh - Friendly AI Assistant with Amazon Quick Suite

The presentation addressed the common challenges faced by enterprise users and project managers: managing excessive documents, meetings, emails, data, and repetitive tasks. **Amazon Quick Suite** was introduced as an AI assistant built on Bedrock, utilizing web search and internal data to optimize these workflows.

**Amazon Quick Suite supports:**
- Intelligent chat and Q&A
- Smart research and search
- BI Dashboards
- Workflow automation
- Embedding APIs into enterprise processes
- Platform: Amazon Bedrock + Web Search + Internal Data

**Illustrative scenario:**
An AI assistant for project management can automatically generate meeting minutes, send emails to stakeholders, and schedule the follow-up meeting.

**Key values:**
- Reduces time spent on repetitive tasks and information gathering
- Enables users to focus more on decision-making and team collaboration

**Key takeaway:** AI delivers the greatest value when integrated directly into the workflow, understanding internal data and enabling subsequent actions.

---

#### 2.3 Nguyen Tuan Thinh - From Edge to Origin: CloudFront is Your Foundation

The session focused on **Amazon CloudFront** as a comprehensive foundational layer from edge to origin, covering cost, security, performance, and reliability at scale.

**Cost model:**
- Fixed pricing packages including CDN, WAF, DDoS, DNS, and logging
- Predictable pricing, suitable for small website owners, enterprise users, and growing businesses
- Handles traffic spikes without unexpected cost explosions

**Security features:**

| Feature | Description |
|---|---|
| DDoS Protection | Protection against high-traffic attacks |
| WAF | Web Application Firewall |
| DNS | Integration with Route 53 |
| TLS / mTLS | Free TLS along with mutual TLS for encrypted connections |
| Signed URL | Content delivery with authorization checks |
| Origin Cloaking | Hiding origin servers from public access |

**Performance optimization:**
- Multi-tier caching at the edge to reduce origin load and optimize bandwidth
- HTTP/3 support
- Data compression
- Persistent connections to reduce origin load
- Edge functions for low-latency logic

**Reliability factors:**
- Serving stale content when the origin is down
- Origin failover
- Intelligent routing

**Key takeaway:** CloudFront is not just a CDN. It is a foundational layer for cost optimization, security, performance, and fault tolerance.

---

#### 2.4 Team VIB - 36 Hours with LotusHacks: Building UTMorpho from Idea to Reality

Team VIB shared their real-world story of participating in the 36-hour **LotusHacks hackathon**, starting from no initial idea to completing a working demo of **UTMorpho**.

**What UTMorpho does:**
Users can take photos, sketch, or upload a UI draft, and the AI will generate a web interface from that input.

**Architecture used:**
```text
CloudFront -> API Gateway -> Lambda -> Bedrock -> S3 / DynamoDB
```

**AI Agent Pipeline:**
1. **Vision Analyst** - Analyzes the input sketch
2. **UI Designer** - Translates it into a design specification
3. **Coder** - Generates the actual source code

**Key challenges:**
- Token limits from the LLM's context window
- AI generating excessive content leading to noisy output
- Presentation time pressure
- Scope creep due to having too many ideas

**Key takeaway:** Real-world frustrations spark real ideas. A hackathon requires good team coordination, tight scope control, and a focus on a single truly useful core experience.

---

#### 2.5 Dao Duc - The Non-Determinism of Deterministic LLM Settings

This presentation answered an important technical question: **Why can LLMs still produce different results even when `temperature=0` is set?** This is a critical issue for high-stakes systems like legal, financial, or medical information retrieval.

**How LLMs generate tokens:**
- Logit computation -> Softmax -> Sampling
- `temperature` only adjusts the probability distribution, it does not completely eliminate the sources of non-determinism

**Experiments conducted:**
- **5 models tested:** GPT-3.5, GPT-4o, Llama-3 70B, Llama-3 8B, Mixtral 8x7B
- **8 tasks x 10 runs** per model; the results showed significant accuracy fluctuations between identical runs

**Technical causes:**

| Cause | Explanation |
|---|---|
| Floating-point operations | GPU computations are not fully deterministic |
| Parallel execution order | Scheduling order of GPU threads can vary |
| Inference batching | Provider-side batching alters processing sequence |

**Mitigation strategies:**
- Run multiple times and use **majority voting**
- Use **structured outputs** such as JSON, regex, or grammar constraints
- Apply **regression testing** to evaluate output stability
- **Self-host** models when complete control over the inference process is required
- Design the system to **tolerate variance** from the start

**Sweet spot:** `temperature ~= 0.1` provides a better balance between stability and output quality compared to fixing it absolutely at `temperature=0`.

**Key takeaway:** `temperature=0` is not a guarantee of reliability. Systems must be architected to handle output variance from the beginning.

---

#### 2.6 Vy Lam - Enterprise Multi-Agent Systems: Credit Scoring for Startups

The session presented a **multi-agent credit scoring system** for startups, a domain where traditional credit assessment models often fail because startup data differs fundamentally from that of long-established businesses.

**Why traditional credit scoring is unsuitable for startups:**
- Requires long financial history, collateral, and stable revenue models
- Startups often only have traction, team quality, IP, and unstructured data

**Data dimensions of startups:**

| Dimension | Example |
|---|---|
| Financial | Revenue, burn rate, runway |
| Market | Market size, competitive landscape |
| Team | Experience, background, diversity |
| Traction | User growth, retention rate, partnerships |

**System design - Virtual Credit Committee:**

| Agent | Responsibility |
|---|---|
| Manager | Coordinates the entire evaluation process |
| Financial Analyst | Evaluates financial metrics |
| Market Analyst | Assesses market opportunities |
| Team Evaluator | Reviews the founding team |
| Risk Evaluator | Identifies risk factors |
| Compliance Checker | Ensures regulatory compliance |

**Output requirements:**
- Credit score
- Risk rating level
- Confidence level
- Audit logs with decision explainability

**Enterprise-level considerations - 6 pillars:**

| Pillar | Scope |
|---|---|
| Security | Authentication, authorization, encryption |
| Data Governance | Data lineage, access control, storage |
| Network | VPC isolation, private endpoints |
| Operations | Monitoring, alerting, troubleshooting |
| Human Element | Explainability, approval workflows |
| Compliance | Regulatory alignment, audit readiness |

**Guardrails - Three layers (Input -> Processing -> Output):**

| Layer | Control |
|---|---|
| Input | Content filtering, PII detection, prompt injection defense |
| Processing | Model selection control, inference constraints |
| Output | Response validation, compliance check |

**Deployment roadmap:**
```text
Local App / CrewAI -> AgentCore -> Docker -> ECR -> Bedrock -> API Gateway
                    + VPC, IAM, Secrets, Monitoring, Autoscaling, DR Strategy
```

**Expected ROI:**
- Processing time: from weeks to hours
- Reduction in analyst work hours
- Increased approval accuracy through multi-dimensional assessment

---

![Event 2 Photo](/awsportfolio/images/4-Event/4.2-event2/event2-photo.jpg?width=40pc&classes=shadow)

---

### 4. Conclusion

AWS Vietnam Community Day 2026 demonstrated that the value of AI lies not in the model alone, but also in how context is supplied, architecture is designed, security and guardrails are deployed, and the system is operated at a practical scale.

| Audience | Key Lesson |
|---|---|
| Individuals | Learn to provide quality context and build a personal knowledge base to work more effectively with AI |
| Product Teams | Prioritize real problems, scope tightly, and embed AI into concrete workflows |
| Infrastructure | Leverage CloudFront and AWS services for performance, security, and reliability |
| Enterprises | Multi-agent systems require guardrails, audit logs, regulatory compliance, and a clear ROI before production deployment |

> **General message:** AI only truly creates value when combined with product thinking, appropriate system architecture, and reliable operational processes.
