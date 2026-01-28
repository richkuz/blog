+++
date = '2026-01-28'
draft = false
title = "LLMs Crossed a Threshold in December 2025"
+++

Andrej Karpathy, the AI researcher, educator, and OpenAI founding member, wrote [A few random notes from claude coding](https://xcancel.com/karpathy/status/2015883857489522876). It's a short post, worth reading in full. Everything in it matches my experience during the past month of software engineering.

> LLM agent capabilities (Claude & Codex especially) have crossed some kind of threshold of coherence around December 2025 and caused a phase shift in software engineering

Over the past 6 months, and increasing this January, I've observed a measurable increase in PR activity among engineers on my teams who have been early adopters of AI tools. The code they produce is high quality, too. Engineers who were previously specialists are now solving problems end-to-end. Their breadth of capability has increased. They are using AI tools to diagnose and fix issues across multiple services and languages. They are also using AI tools to improve their developer experience, which has had a compounding effect on their ability to ship more PRs faster.

I observe this trend in my own work, too. On December 18, I had a spark of an idea to [build a PDF viewer as a side project](2026-01-05 A Better Reader for Documents). I used Cursor's CLI agent almost exclusively to build the feature, with heavy use of `git diff` to review the code and a lot of manual testing. In 2 short days I had a proof of concept implementation that solved my use cases better than a $25K/year paid commercial library. 2 weeks, 500M tokens, 3 major refactors, and 200 commits later I had a production-ready, highly performant, accessible, readable, extensible, maintainable PDF reader almost ready to ship. This project would have easily taken me 1+ years to build without AI tooling.


> Armed with LLMs, do generalists increasingly outperform specialists?

Now more than ever software companies need people who can solve problems truly end-to-end (not just full-stack), from problem discovery, design, architecture, planning, implementation, testing, and closing the loop soliciting end-user feedback. People who can operate end-to-end on a project will experience much tighter feedback loops. They will be able to deliver more value faster. LLMs have enabled smart, motivated people to become passing associate-level designers, product managers, project managers, quality engineers, and software engineers.

People who can effectively break down complex problems into projects that individuals can solve end-to-end will accelerate entire organizations. Architecture and organizational design have to keep pace.

And software companies still need people with specialized skills to provide feedback in their respective domains. It's not an either/or tradeoff.


> What happens to the "10X engineer" - the ratio of productivity between the mean and the max engineer? It's quite possible that this grows *a lot*.

Intuitively it seems plausible, but I've not observed it empirically in my teams yet. Subjectively, I have observed "average" engineers in one domain leveling up their breadth and increasing their value and impact as a result of AI tooling adoption.

Karpathy notes LLMs are less about speedups, and more about an expansion of capabilities. I see engineers approach code now that they wouldn't have touched before. LLMs give them courage to try.


> Tenacity. It's so interesting to watch an agent relentlessly work at something

A colleague shared a quote from a basketball coach in their youth: "The ball doesn't get tired." Pass the ball around, wear out the defense, create an opening, and take the shot.


> Atrophy. I've already noticed that I am slowly starting to atrophy my ability to write code manually.

In early December I practiced a few Advent of Code exercises (no LLMs, language references only) to brush up on my atrophying Python skills. In hindsight, given the progress of LLM coding I experienced in late December, I think it was a wasted effort.

Writing code by hand matters only for learning fundamentals and as a signal in outdated engineering interview processes. Reading code, reviewing code, organizing code, and scrutinizing code are still important skills.


> What does LLM coding feel like in the future? Is it like playing StarCraft? Playing Factorio? Playing music?

Maybe. A few engineers who are running swarms of coding LLMs at the extreme end believe they are operating at such a high level of constant decision making that [they have to take naps they are so exhausted](https://steve-yegge.medium.com/steveys-birthday-blog-34f437139cb5).


> Slopacolypse. I am bracing for 2026 as the year of the slopacolypse across all of github, substack, arxiv, X/instagram, and generally all digital media.

It's a race to the bottom. Marketing teams need to flood every zone with AI generated content for their companies or be drowned out by their competitors. Attention is only getting scarcer.


> 2026 is going to be a high energy year as the industry metabolizes the new capability.

I remember December 2024 as the month when I first tried MCP tools, which felt like a revolutionary advance in AI automation. December 2025 is when I first tried Opus 4.5 and felt the step change in AI coding capabilities. Even if models remain stagnant (they won't), software engineering is forever changed. The accelerated pace is accelerating.