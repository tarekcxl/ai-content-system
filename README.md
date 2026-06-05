# Content Operations System

AI-powered modular content operations system built around specialized agents, focused skills, and reusable workflows to scale content ideation, repurposing, newsletter writing, social analytics, competitor analysis, fact-checking, and reporting across LinkedIn, Instagram, YouTube, blogs, and newsletters.

---

## What It Does

* Generates content ideas using Reddit + Google search insights
* Analyzes competitor social performance
* Repurposes content into:

  * carousels
  * videos
  * blogs
  * newsletters
* Writes newsletters using the CXL tone of voice
* Validates factual accuracy and reduces hallucinations
* Analyzes social performance
* Generates weekly/monthly reports
* Creates structured content calendars

---

## Architecture

```bash
/agents
  → orchestration and decision-making

/skills
  → focused execution capabilities

/skills/*/references
  → examples, tone references, frameworks

/workflows
  → outputs, reports, exports, drafts
```

---

## Agents

| Agent                             | Purpose                                         |
| --------------------------------- | ----------------------------------------------- |
| content-ideation-agent            | Finds content opportunities and trends          |
| competitor-social-analytics-agent | Analyzes competitor social performance          |
| repurposing-agent                 | Repurposes content into platform-native formats |
| social-copywriter                 | Writes newsletters and editorial content        |
| fact-check-agent                  | Validates accuracy and credibility              |
| social-analyst                    | Audits social media performance                 |
| reporting-agent                   | Generates weekly/monthly reports                |

---

## Skills

| Skill                  | Purpose                               |
| ---------------------- | ------------------------------------- |
| content-ideation       | Reddit + Google-based idea generation |
| content-calendar       | Structured publishing schedules       |
| competitor-analysis    | Competitor social analysis            |
| carousel-repurposing   | Carousel creation                     |
| video-repurposing      | Short/long-form video scripting       |
| blog-repurposing       | SEO/AEO/GEO blog creation             |
| newsletter-repurposing | Newsletter transformations            |
| newsletter-writing     | Newsletter writing using CXL tone     |
| fact-check             | Accuracy and hallucination validation |
| social-analysis        | Social performance analysis           |
| social-reporting       | Weekly/monthly reporting              |

---

## Example Workflow

```text
Topic Discovery
    ↓
Competitor Analysis
    ↓
Content Ideas
    ↓
Content Calendar
    ↓
Repurposing
    ↓
Newsletter Writing
    ↓
Fact-Checking
    ↓
Publishing
    ↓
Social Analysis
    ↓
Reporting
```

---

## Core Principles

* modular agents over giant prompts
* focused skills over overloaded instructions
* progressive disclosure
* platform-native optimization
* reusable workflows
* structured outputs
* audience-first content strategy

---

## Output Style

Prefer:

* concise outputs
* structured tables
* actionable recommendations
* platform-native deliverables

Avoid:

* generic AI writing
* repetitive summaries
* unnecessary context

---

## Workflow Usage

Use `/workflows` for:

* generated drafts
* reports
* exports
* scraped discussions
* automation outputs

---

## Philosophy

The goal is not to generate random content.

The goal is to identify, create, validate, analyze, repurpose, organize, and optimize content using real audience behavior and platform data.
