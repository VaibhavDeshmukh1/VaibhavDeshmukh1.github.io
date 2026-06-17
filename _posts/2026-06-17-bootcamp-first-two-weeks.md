---
title: 'First Two Weeks at the Northwestern AI Bootcamp'
date: 2026-06-17
permalink: /posts/2026/06/first-two-weeks/
tags:
  - AI
  - bootcamp
  - learning
---

These first two weeks of the Northwestern Agentic AI Bootcamp have been a lot more hands-on than I expected. I came into the program with some Python experience, but I had never made an actual API call or worked with any language models programmatically, so almost everything I learned was new.

The first thing I worked through was making basic calls to a language model. The pattern is simple once you see it, since you send a message with a role attached to it and the model sends back a response with its own role, and to have a conversation you just keep adding messages to a list and sending the whole list each time. The model itself does not remember anything between calls, so the conversation history is really something you maintain on your side.

After that I moved on to tool use, which is the part that actually makes a system feel like an agent rather than just a chatbot. The idea is that you describe a set of tools to the model and let it decide when to call them, and then your own code runs the tool and sends the result back. I built a small research assistant that could look up information on Wikipedia, save notes, recall notes, and do calculations, and what struck me about it was how much the descriptions you give the model matter, because vague descriptions led to the model calling the tools at the wrong times.

The last topic I touched was retrieval augmented generation, which is a way of letting a model answer questions about documents it was never trained on. I built a small system that would take a Wikipedia article, break it into chunks, convert each chunk into a vector representation, and then search for the chunks most relevant to a question before giving them to the model as context. I am still working on understanding why the embedding step actually works the way it does, but the overall pattern made sense to me.

Looking ahead, I am about to start the research project portion of the program, and I am hoping to keep building on these basics rather than rush into anything I do not yet understand.