---
layout: post
title: LLM Adventure Intro
---

Hello! Yes, this name is "borrowed" from Sebastian Lague's [Coding Adventures](https://www.youtube.com/playlist?list=PLFt_AvWsXl0ehjAfLFsp1PGaatzAwo0uK).

In this series of dev logs in the form of blog posts I'll explore how to create a toy LLM. By the end I expect to have a somewhat functional LLM with the following: 

 - Being able to complete sentences in a coherent way (_at the very least_).
 - Chatting and being able to respond coherently with provided context.
 - Be able to deploy somewhere and share with other people (both code and weights).

I'll explain how I'm gonna achieve each point and what they even mean, but I expect you to understand some of what is being said. I should also say that this is more of a devlog style than a tutorial.

Being able to complete sentences is the starting point if you wanna make something like this. This is what people call a _base model_: a model that's trained on a significant amount of data to learn patterns and relations between the words of a language and be able to complete sentences in a way that makes at least some sense to a human.

Making it able to chat is another big undertaking: it's not as computationally involved as training the base model but we also need to procure a lot of high quality data. In this part we basically teach the model to _output text in a very specific way by using a few special tokens and other techniques_.

Also, being able to respond coherently with provided context: by that I mean being able to fetch documents from somewhere and inject them in some sort of prompt. This way, even though the chatbot is presented with a question it doesn't know anything about (likely), it will be able to respond in a somewhat competent way.

The last point refers exactly to what it sounds like. Making the model code open source and allowing people to download the weights.

**Ambitious? Maybe, but I think it will be a fun learning experience. I also have nothing better to do with my free time (lol).**
