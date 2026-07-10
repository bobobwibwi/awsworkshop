---
title: "Event 1 - Prompt Engineering, AI Mind Mapping & BMAD Method"
date: 2026-05-09
weight: 1
chapter: false
pre: " <b> 4.1. </b> "
---

| Information | Details |
|---|---|
| Date | 09/05/2026 |
| Location | 26th Floor, Bitexco Financial Tower, Saigon Ward, Ho Chi Minh City |
| Role | Attendee |

This page summarizes the content from the event, which covers three main topics: Automated Prompt Engineering, a mind map on effective AI interaction, and the BMAD development method.

---

### 1. Introduction

This document compiles content from various sources, including:
- Presentation: **“Automated Prompt Engineering: Enhancing LLM Output Quality”**
- Mind map: **“Effective AI Interaction & AWS Application Architecture”**
- AI development framework: **BMAD (Build More Architect Dreams)**

---

### 2. Detailed Content

#### 2.1 Presentation: Automated Prompt Engineering

**Speaker: Nguyen Tuan Thinh**

This presentation explains the importance of prompt engineering when working with Large Language Models (LLMs), while providing principles and tools to improve output quality.

**Why Prompt Engineering is important:**
- Overly generic prompts often yield poor results
- Wasting tokens
- Vague instructions reduce quality and productivity

**Components of an effective prompt:**

| Component | Description |
|---|---|
| Role | Defines a persona or role for the AI |
| Instructions | What the AI needs to perform |
| Context | Necessary background information |
| Input Data | The data that needs to be processed |
| Output Format | The desired presentation of the result |
| Examples | Sample input and output patterns |
| Constraints | Limits and rules to follow |

**Guidelines for writing prompts:**
- Clear and specific
- Use direct, imperative language
- Describe exactly what needs to be done
- Allow the model to answer "I don't know" when necessary
- Break down long tasks into steps

**Token economy:**
- Tokens are the processing units of LLMs
- Costs are calculated based on input and output tokens
- Costs vary by language, and Vietnamese typically consumes more tokens than English

**Advanced techniques:**
- Chain-of-Thought (CoT): step-by-step reasoning
- Tree-of-Thoughts (ToT): building multiple reasoning branches
- Self-Consistency: comparing multiple reasoning paths to select the best answer
- Retrieval-Augmented Generation (RAG): augmenting knowledge from external sources
- Role Prompting: assigning a specific role to the model

**Tool - Proptimizer:**

A browser extension that helps automate prompt optimization based on AWS serverless architecture:
CloudFront -> S3 -> Cognito -> API Gateway -> Lambda -> Bedrock -> DynamoDB -> CloudWatch

---

#### 2.2 Mind Map: Effective AI Interaction & AWS Application Architecture

**Optimizing interaction with AI:**
- Use the KFC (Knowledge, Format, Constraints) framework to provide clear context, formats, and constraints

**Recommended approaches:**
- Break down tasks
- Ask AI to suggest options
- Compare multiple alternatives
- Supplement with structured data

**Advanced AI techniques:**
- Apply CoT, ToT, Self-Consistency, RAG, and Role Prompting to improve results

**AWS Architecture (Serverless):**
CloudFront, S3, Cognito, API Gateway, Lambda, Bedrock, DynamoDB, CloudWatch

---

#### 2.3 BMAD Method (Build More Architect Dreams)

BMAD is an open-source, free, AI-oriented development framework that helps teams build solutions following a clearly structured process.

**Key features:**
- Phases: Analysis -> Planning -> Architecture -> Implementation
- Over 12 specialized agents assisting users at each step
- Agile practices integration
- AI assistant: `bmad-help`
- Party Mode for multi-agent collaboration

**Core modules:**

| Module | Description |
|---|---|
| BMM | Core framework - 34 processes |
| BMB | Custom agent builder |
| TEA | Testing and automation |
| BMGD | Game development |
| CIS | Innovation and design thinking |

**Quick installation (requires Node.js 20+, Python 3.10+, and `uv`):**
```bash
npx bmad-method install
```

**Community support:** Discord, YouTube, X/Twitter

---

### 3. Event Photos

Below are photos captured during the event:

![Event 1 Photo](/awsportfolio/images/4-Event/4.1-event1/event1-photo.jpg?width=40pc&classes=shadow)

---

### 4. Conclusion

This event clearly presented three distinct areas of content: prompt engineering, AI interaction frameworks, and the BMAD development method. Since each section has different objectives and origins, separating the content makes it easier for readers to understand and apply. Overall, this is a highly useful set of knowledge for working more effectively with AI systems and AWS cloud architectures.
