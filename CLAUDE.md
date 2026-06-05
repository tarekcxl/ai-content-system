# Content Operations System

AI-powered content operations system for:

* content ideation
* social content creation
* content repurposing
* newsletter writing
* fact-checking
* social media analysis
* competitor social analysis
* social reporting
* content planning and scheduling

The system helps identify content opportunities, repurpose existing content into platform-native formats, validate content quality, analyze competitor strategies, monitor performance, and generate actionable reporting using audience behavior and platform data.

---

# Objective

Maximize:

* content output
* engagement
* reach
* retention
* content reuse efficiency
* platform-native performance
* editorial quality and trustworthiness

Through:

* content ideation
* content repurposing
* newsletter writing
* fact-checking
* competitor analysis
* social analysis
* social reporting
* structured content planning

---

# Architecture

* `/agents`
  → self-contained operational agents

* `/skills`
  → focused capabilities used by agents

* `/skills/*/references`
  → optional context, examples, frameworks, and best practices

* `/workflows`
  → generated outputs, drafts, reports, scraped discussions, and automation outputs

---

# Core Rules

* prioritize audience relevance over generic content
* optimize content for the target platform
* avoid generic repurposing
* focus on engagement, clarity, and retention
* preserve factual accuracy during generation and repurposing
* reuse high-performing ideas intelligently
* use focused skills instead of overloaded instructions
* load only relevant context and references
* prioritize actionable outputs over brainstorming noise
* preserve CXL tone of voice and editorial consistency

---

# Execution Flow

Default workflow:

1. `content-ideation`
2. `competitor-social-analytist`
3. `repurposing-agent`
4. `social-copywriter`
5. `fact-check`
6. `social-analyst`
7. `reporting`

Example:

topic discovery
→ competitor analysis
→ content ideas
→ content calendar
→ content repurposing
→ newsletter creation
→ fact-checking
→ publishing
→ performance analysis
→ reporting

---

# Agent Responsibilities

## content-ideation

Identifies content opportunities, audience pain points, trends, and platform-native content ideas.

## competitor-social-analysis
Analyzes competitor social media performance to identify winning content patterns and differentiation opportunities.

## repurposing-agent

Transforms existing content into platform-native formats for social and distribution channels.

## social-copywriter

Writes newsletters and editorial content using the CXL tone of voice and writing standards.

## fact-check

Validates factual accuracy, hallucinations, citations, and editorial credibility before publishing.

## social-analyst

Analyzes social media performance to identify winning patterns, weak-performing content, and improvement opportunities.

## reporting

Generates weekly or monthly social performance reports using platform analytics and comparative trend analysis.

---

# Skill Usage

Agents decide when to use skills.

Skills define how execution happens.

Use the most focused skill possible.

---

# Skills

## content-ideation

Identifies content opportunities using search demand, Reddit discussions, audience questions, and trend analysis.

## content-calendar

Creates structured content calendars, posting schedules, and platform-specific publishing plans.

## competitor-analysis

Analyzes competitor social media performance across LinkedIn, Instagram, and YouTube to identify winning patterns and strategic opportunities.

## blog-repurposing

Transforms content into SEO/AEO/GEO-optimized long-form written content.

## carousel-repurposing

Transforms content into high-retention carousel structures optimized for engagement and readability.

## video-repurposing

Transforms content into short-form and long-form video scripts optimized for hooks, pacing, and retention.

## newsletter-repurposing

Transforms content into newsletter-ready formats optimized for readability and engagement.

## newsletter-writing

Writes engaging newsletters using the CXL tone of voice, editorial patterns, and newsletter examples.

## fact-check

Validates claims, statistics, citations, and AI-generated outputs to reduce hallucinations and credibility risks.

## social-analysis

Analyzes social media performance using engagement, retention, and platform-specific metrics.

## social-reporting

Generates weekly or monthly social media performance reports using engagement, growth, and comparative platform analytics.

---

# Workflow Usage

Use `/workflows` for:

* generated outputs
* drafts
* reports
* scraped discussions
* content exports
* automation outputs
* social analysis exports
* competitor analysis exports
* reporting exports

Workflows execute tasks.

Agents perform reasoning.

---

# Output Expectations

Prefer:

* concise outputs
* structured tables
* actionable recommendations
* platform-specific deliverables
* content-ready outputs

Avoid:

* generic explanations
* repetitive summaries
* unnecessary context
* low-signal brainstorming

---

# Progressive Disclosure

Do not load unnecessary files.

Only load:

* relevant agents
* required skills
* necessary references
* relevant workflows

Focused context improves output quality.

---

# System Philosophy

The system is designed around:

* modular agents
* focused skills
* progressive disclosure
* reusable workflows
* scalable content operations

The goal is not to generate random content.

The goal is to identify, create, validate, analyze, report, repurpose, organize, and optimize content based on real audience behavior and platform dynamics.
