+++
date = '2026-01-05'
draft = false
title = 'AI Tooling Case Study - A Better Reader for Documents'
+++

Over the holiday break as a side project I built a high-performance document viewer in React that supports PDF and scanned documents. It provides a seamless reading experience with progressive loading, advanced search, native-like text selection, advanced document comparison capabilities, integrated AI chat, etc.

![[bread-viewer.png]]

- I used **Cursor CLI** almost exclusively for all code writing on the frontend
- **Gemini 3 Flash** was my primary work horse, with **Gemini 3 Pro** for harder problems and planning. I switched to **Sonnet 4.5** when Gemini got stuck or I needed a second opinion.
- Used ~500M tokens for the project (Dec 18->Jan 4)
- Generated and individually reviewed about 200 commits, including some challenging algorithms, performance optimizations, Storybook, unit testing, and many big refactorings along the way.
- The backend was simple enough that I ended up re-coding most of it by hand. AI kept getting tripped up by our Staging env deploy ID setup, and I got tired of correcting the AI.
- Only a couple runaway prompts and Cursor crashes. 100K tokens is about the max before I'd have to start a new conversation.
- Building the custom routing / modal logic really threw AI for a loop, I guess because it went against the grain of its training data.
- Small files with highly targeted prompts and super tight review feedback loops work so much better than large one-shot hail mary attempts.
- I had _no_ Cursor rules files for this project. All vanilla prompts, with a README.md and ACHITECTURE.md doc so I didn't have to repeat myself in the prompts.
- Having a unique name for the project ("bread") helped AI search the relevant code files more easily I think.


![[bread-cursor-usage.png]]

Gemini Flash is great for most rote tasks, and it's crazy fast. But when it gets confused, it tends to generate more tokens and cost more than if I had just used Gemini Pro 3. I stayed away from Opus 4.5 because of the 10x cost, but everything I've read (and later experienced) shows it to be even better than Gemini Pro 3 at coding.

AI coding models and tooling feels like a step change in effectiveness since the last project I built at this scale 1 year ago.

If I had to write it all by hand and think through all the algorithms myself, this project would have easily taken me 1 year full time, probably longer. Instead it took about 2 weeks. And I was able to have a relaxing vacation while doing it! When I had a spare moment I'd kick off a prompt, let it churn in the background, then come back to review it when I freed up again. I didn't need the 100% focus that I would if I were writing all the code by hand. Very little willpower needed to keep going.

I haven't had this much fun building software since I was a kid.