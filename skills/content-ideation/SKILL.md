---

name: content-ideation
description: Identify social content opportunities using search demand, Reddit discussions, audience questions, and trending conversations.
-------------------------------------------------------------------------------------------------------------------------------------------

# Content Ideation

A skill for identifying high-potential content ideas using real audience behavior and search demand.

This skill combines:

* Google search behavior
* People Also Ask questions
* Related Searches
* Reddit discussions and pain points

to identify content opportunities for social media and content marketing.

---

## What this skill does

Use this skill to:

* identify content opportunities
* surface audience pain points
* identify recurring questions
* discover trending discussions
* generate social content ideas
* generate hooks and content angles
* identify high-interest themes

---

## Inputs

This skill expects:

* a primary keyword or topic from the user

Examples:

* “AI marketing”
* “SEO”
* “content strategy”
* “YouTube automation”

---

## Data Sources

This skill may use:

* Search API
* Google search results
* People Also Ask
* Related Searches
* Reddit scraping workflows
* subreddit discussions
* Reddit comments and recurring questions

---

## How to Work

### Step 1: Analyze search demand

Use Search API to:

* run a Google search for the keyword
* review search result patterns
* identify recurring themes
* identify common content angles

Also extract:

* People Also Ask questions
* Related Searches
* recurring modifiers and search intent patterns

Focus on:

* repeated questions
* beginner confusion
* tactical problems
* controversial discussions
* high-interest subtopics

---

### Step 2: Analyze Reddit discussions

Before scraping, identify 3–5 relevant subreddits where the target audience actually discusses this topic.

Do not use a generic Reddit search — it returns trending off-topic posts, not practitioner discussions.

**Subreddit map for common CXL topic areas:**

| Topic area | Target subreddits |
|------------|-------------------|
| AI marketing / AI tools | r/marketing, r/digitalmarketing, r/artificial, r/ChatGPT |
| B2B marketing / demand gen | r/marketing, r/b2bmarketing, r/sales |
| SEO / content | r/SEO, r/bigseo, r/content_marketing |
| Marketing automation | r/marketing, r/marketingautomation, r/nocode |
| Social media marketing | r/socialmedia, r/marketing, r/Instagram |
| Paid ads | r/PPC, r/FacebookAds, r/marketing |
| Startups / growth | r/startups, r/Entrepreneur, r/GrowthHacking |
| No-code / automation tools | r/nocode, r/n8n, r/zapier, r/automation |

If the topic doesn't match a row above, identify subreddits by asking:
* Where do practitioners in this space congregate on Reddit?
* What subreddits cover the tools, platforms, or job functions involved?

**How to scrape:**

Use `startUrls` with subreddit-specific search URLs. This restricts the search to each community.

URL format:
```
https://www.reddit.com/r/SUBREDDIT/search/?q=QUERY&sort=top&t=month&restrict_sr=1
```

Example for "AI agents B2B marketing":
* `https://www.reddit.com/r/marketing/search/?q=AI+agents+B2B&sort=top&t=month&restrict_sr=1`
* `https://www.reddit.com/r/b2bmarketing/search/?q=AI+agents&sort=top&t=month&restrict_sr=1`
* `https://www.reddit.com/r/digitalmarketing/search/?q=AI+agents&sort=top&t=month&restrict_sr=1`

Target at least 3 subreddits per topic. Run them as a single scraper call using multiple `startUrls`.

**Extract from results:**

* recurring questions
* frustrations and pain points
* trending conversations
* highly engaged discussions
* misconceptions or debates

Focus on:

* emotional language
* repeated struggles
* beginner mistakes
* controversial opinions
* tactical questions
* recurring requests for help

Do not summarize Reddit blindly.

Extract patterns and insights.

---

### Step 3: Identify content opportunities

Combine:

* search demand
* Reddit pain points
* recurring questions
* trend patterns

Then identify:

* content opportunities
* social post ideas
* educational angles
* contrarian angles
* hook opportunities
* platform-native ideas

Focus on ideas that:

* solve a real problem
* create curiosity
* teach something actionable
* align with audience intent

---

### Step 4: Organize ideas

Group ideas into themes or categories.

Examples:

* beginner mistakes
* tactical tips
* myths and misconceptions
* unpopular opinions
* tutorials
* workflows
* case studies

---

## Output Structure

### Audience insights

Key patterns identified from:

* search behavior
* People Also Ask
* Reddit discussions

---

### Content opportunities

Provide:

* content idea
* hook/angle
* why it matters
* suggested platform

---

### Recurring pain points

List the most repeated audience struggles or questions.

---

### Suggested content themes

Group ideas into repeatable content pillars.

---

## Output Expectations

Prefer:

* concise outputs
* grouped ideas
* actionable opportunities
* platform-native suggestions
* high-signal insights

Avoid:

* generic brainstorming
* repetitive ideas
* weak “listicle” topics
* low-signal summaries

---

## Rules

* prioritize real audience behavior over assumptions
* identify patterns instead of isolated examples
* focus on actionable opportunities
* avoid generic content ideas
* optimize for engagement and usefulness
* identify ideas that can scale into multiple formats

---

## Working Style

Think like a content strategist focused on identifying scalable content opportunities.

Your job is not to generate random ideas.

Your job is to identify what people are actively:

* searching for
* discussing
* struggling with
* debating
* engaging with
