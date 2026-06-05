Subject Line: Building an SEO workflow - Episode 1
Pre-header: From Google Search Console data to real ranking opportunities


Title: Building an seo workflow in n8n to automate keyword research and identify ranking opportunities - Episode 1

When it comes to educational content, we usually show the polished end result. The best practices, the final framework, the “what works.”

But what often gets left out are the setbacks, the failed experiments, and the messy process that actually leads to those results.

That’s exactly why we’re launching this mini-series.

In this series, we’re building our own SEO workflow in public together, step by step.
Every week, we’ll share honest updates on how the workflow is evolving:
what’s working, what’s not, what’s changing, and how the plan is taking shape in real time.

Because the real learning doesn’t just come from the final answer but it comes from seeing the journey in its raw, unfiltered form.

In this first episode, we’re introducing the plan we have in mind and sharing what we’ve built so far.

The plan 




There’s a lot of noise online about fully automated SEO systems that can replace teams.

We want to move beyond the hype and actually test it ourselves: to see the real results, the real constraints, and where these tools truly help and where they don’t.

So here’s our plan.

We want to build an agent on n8n that alerts us whenever there’s a real opportunity hidden inside our Google Search Console data.

(Quick note: Google Search Console is a free tool from Google that shows how your website performs in search including the keywords you rank for, clicks, impressions, and average positions.)

This agent’s job is to continuously scan that data and highlight where we could realistically perform better.

Once an opportunity is identified, another agent is alerted to:

Analyze the top-ranking articles for that keyword using a SERP API.
Review the Google AI summary shown in search results.
Scrape and study the competing content.
Compare everything against our own article to uncover concrete improvement areas.

From there, we start making targeted optimizations.

Only after that will we expand into the second phase which is creating an agent for deeper keyword research and creating entirely new content around fresh opportunities.

We want to make sure we’re building something that anyone can use, regardless of their budget.
That’s why, for this test, we’re intentionally avoiding expensive SEO tools or APIs like SEMrush or Ahrefs.


What we’ve done so far



So far, we’re off to a good start.

Connecting our Google Search Console data turned out to be surprisingly simple.
Here’s how the workflow currently works (as shown in the screenshot above from n8n):

First, a form is triggered where we define the date range we want to analyze.




Next, the workflow connects directly to our Google Search Console (GSC) account, pulls all the relevant performance data, and stores each row into a structured spreadsheet table.




From there, an AI agent gets access to the spreadsheet and analyzes the full dataset to uncover SEO opportunities highlighting what’s working, what’s underperforming, and where we can realistically improve.



However, this is where we ran into our first real problem.

Up until this point, everything had worked perfectly.
The connection with Google Search Console was successful, and we generated a spreadsheet containing more than 2,000 rows of data including URLs, clicks, impressions, and average positions.

But when it came time for the agent to analyze the spreadsheet…things slowed down dramatically.

We waited 15 to 20 minutes, and it was still loading without producing any results.

So we tried a different approach.
We stepped outside of n8n, opened ChatGPT, uploaded the same spreadsheet, ran the exact same prompt and received clear insights and recommendations in under a minute.

On the bright side, this confirmed something important: the prompt itself was strong.

It successfully identified 10 key pages with real opportunities to improve rankings.

The downside?
This analysis wasn’t happening inside the n8n workflow, because the processing time there was simply too slow.
In practice, it was much faster to export the spreadsheet and analyze it separately using ChatGPT or Gemini.

If you’re wondering why this happened…In practice, n8n’s AI Agent was likely struggling with the token limit or the overhead of fetching 2,000+ individual rows through the spreadsheet tool interface, whereas ChatGPT’s Code Interpreter processes the file as a single batch in a sandbox.

The fix

To keep the workflow fully automated and fast enough to be practical, we reduced the analysis window from one month to one week.

This change:

Lowered the dataset from ~2,000 rows to around 500 rows.
Kept the insights recent and actionable.
Allowed the agent to complete the analysis by analyzing a smaller dataset.

And it actually worked.

Next steps

Now that we have an agent capable of identifying the top 10 pages with the highest potential for improvement, the next step is to build a second agent.

This new agent will search Google for the top-ranking articles for each target keyword, compare them with our own content, and highlight what’s missing along with concrete improvement suggestions.

We’re building this step as you read this, and in the second episode we’ll share how it went, the good, the bad, and everything in between.

And if you feel we’re over-focusing on one step, missing something, or should expand the workflow, just reply to this email and tell us.

This is a collaborative build, so your feedback is more than welcome.
