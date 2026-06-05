Email Subject Line: Building a Paid Media Co-Pilot
Pre-header: Built in minutes, not weeks

Title: Designing a Paid Media Co-Pilot with AI


When it comes to AI, most of us are already using it in one way or another.

Content creation.
Data analysis.
Automating the boring, repetitive stuff.

But one use case that keeps popping up more and more is research. Using AI to speed up discovery, surface patterns, and gather insights about our audience without spending hours digging.

Whether it’s ChatGPT, Claude, or Gemini, chances are you’ve already used one of these tools to research something. A market. A persona. A topic you needed to understand fast.

Now here’s the interesting question:

What if, instead of just using AI for research, you used AI to build your own research tool?

We saw this post by Kamil Rextin where he used AI to build his own paid media co-pilot.




Using Claude Code, he created a tool that turns a simple audience description into LinkedIn ad targeting. You describe who you want to reach, and the tool maps it to LinkedIn’s targeting options such as job titles, functions, seniority, skills, and more.



Instead of clicking through endless dropdowns, you review the matches and push the audience straight into LinkedIn as a draft campaign.

The result: 


Faster audience setup: Go from idea to campaign in minutes, not hours.
Less manual work: No more clicking through dozens of LinkedIn targeting dropdowns.
Fewer targeting mistakes: Reduces missed job titles, wrong seniorities, or forgotten exclusions.
More consistent campaigns: Audiences are built the same way every time.
Easier experimentation: Quickly create and test new audience variations.
Lower cognitive load: Focus on strategy instead of platform mechanics.

It felt like a no-brainer to give this a shot and build our own version, with a few tweaks.

Instead of going deep into LinkedIn alone, we wanted to go broader covering multiple ad platforms and pulling in their targeting criteria across Meta (Facebook and Instagram), Google (Search and YouTube), X, TikTok, and more.

We also thought it’d be interesting to go beyond targeting and generate different variations of ad copy alongside it.

Here’s how we did it.

Step #1: Go to Lovable

We used Lovable to build our version of this app, starting with this prompt structure:

1. System Role (Define who the AI is and how it should think)

You are a [role] with expertise in:
– [skill / domain 1]
– [skill / domain 2]
– [skill / domain 3]

Your goal is to [high-level objective].

2. User Inputs (Clearly list what the user needs to provide)

The user will provide:
– [Input #1]
– [Input #2]
– [Input #3]

These inputs are used as context for the analysis.

3. Analysis Instructions (Tell the AI exactly how to think, step by step)

Once all inputs are provided, follow these steps in order:

Step 1: Analyze [thing] to understand [outcome].
Step 2: Derive [insight / profile / structure].
Step 3: Adapt the output to [platform / channel / constraint].
Step 4: Generate [final outputs] based on best practices.

If you’re curious to try it yourself, you can find the exact prompt we used to build this app here.

Step #2: Adjust the prompt if needed

It took Lovable around five minutes to generate the first version, which honestly worked straight out of the gate. 

One thing to keep in mind though: the UX/UI won’t be perfect from the start. If you’re on the free plan, you get five daily credits, which limits how much you can refine things but the app still works.

If you’re on the Pro plan, you can keep prompting it to polish the UI, tweak colors, and refine visual elements.

Step #3: Test it out

First, we added our website URL, briefly described our product, and selected LinkedIn as the channel for targeting.



From there, the app visited our website and analyzed everything (our products, services, value proposition, and positioning).

it shared a summary of what it understood from the website.



Then, based on that analysis, it generated a potential ICP.




Then, it mapped that ICP to LinkedIn’s targeting criteria.



And finally, it produced ad copy and a few variations tailored to that audience.



To see whether it could actually differentiate between targeting across platforms, we ran a second example using Reddit. The targeting criteria it returned were specific to Reddit, including relevant subreddits and interest-based targeting.



Please note that this prototype is powered by Gemini, which means usage is tied to the account running it. For that reason, we’re not making the app publicly accessible.

That said, we’ve shared the full prompt here. You can copy it, spin up your own version, and have it running in about five minutes.

Future iterations

If you want to take this a step further, right now the app mainly gives you insights. You still need to manually copy the targeting criteria into LinkedIn, Reddit, or whichever platform you’re using, and do the same with the ad copy.

The next logical step is connecting the ad platform APIs (following a similar approach to Kamil’s), so campaigns can be drafted directly from within the app, removing even more friction from the process.

The app could pull in performance data for different audiences and targeting setups, learn what actually works, and then use that data to make smarter recommendations over time.

That’s where tools like this are headed: less setup, fewer handoffs, and systems that improve as they’re used.

Why this matters

Five minutes. That’s all it took to go from an idea to a functioning app.

What we’ve been showing in this edition and the last few is a broader shift: marketers no longer need to depend solely on third-party platforms. You can build your own toolstack.

Whether it’s content, automation, or research, the opportunity now is to spot friction and design your own solution.

