---
title: 'First Two Weeks at the Northwestern AI Bootcamp'
date: 2026-06-17
permalink: /posts/2026/06/first-two-weeks/
tags:
  - AI
  - bootcamp
  - learning
---

The first two weeks of the Northwestern Agentic AI Bootcamp have been more hands-on than I expected. I came in with some Python experience but had never made an API call or worked with language models before, so most of it was new.

To prepare before the project starts, I spent the time learning the basics on my own. The first thing I figured out was how API calls work, which involves sending messages with a role attached and getting responses back the same way, and to have a conversation you keep adding messages to a list and send the whole list each call, since the model doesn't remember anything between them. From there I started working with tool use, which is what lets the model actually take actions instead of just generating text. You describe tools to the model, it decides when to use them, and your code runs them and sends back the result. I built a small research assistant that could pull from Wikipedia and handle some basic memory and calculation tasks, and what surprised me most was how much the tool descriptions matter, since vague ones kept making the model use the tools at the wrong times.

Alongside the AI work, I set up the technical environment I'll need for the project stage. That meant getting VS Code and a GitHub account set up, and learning how to write code locally and push it to a remote repo. I used these tools to build the website you're reading this post on, which let me get comfortable with the basic coding workflow on something simple before doing it on actual research code. I also got my first real exposure to AI coding assistants inside an editor, which I think will be a big part of how I work going forward.

Looking ahead, I'm about to start the research portion of the program. I plan to spend more time making sure I actually understand the basics before moving on to harder material.