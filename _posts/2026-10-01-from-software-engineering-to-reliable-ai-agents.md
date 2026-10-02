---
layout: post
title: From Software Engineering to Reliable AI Agents
date: 2026-10-01 09:00:00-0500
description: How building software and studying technical debt led me to research on reliable AI agents.
tags: ai-agents software-engineering reliability
categories: research-notes
related_posts: false
---

Before starting my PhD, most of my time went into building software: web platforms, mobile apps, automation pipelines, and AI-enabled tools. This note explains how that work led me to my current research on reliable AI agents.

### Lessons from building systems

Building production systems teaches you that most failures happen at the boundaries: between services, between a program and the data it receives, between what an API promises and what it actually does. The interesting bugs are rarely inside a single function. They appear when components that each work correctly are put together in ways nobody fully specified.

### Lessons from technical debt

My master's thesis looked at technical debt in open-source projects. Static analysis tools can flag thousands of issues in a mature codebase, but a list of problems is not a plan. The question that mattered to maintainers was not _what is wrong_ but _what will cost us the most if we leave it_. Answering that meant building labels that reflect real maintenance consequences rather than raw tool output, and validating models on projects they had never seen.

Two lessons stayed with me. First, be careful about what a metric actually measures. Second, the gap between what a tool reports and what matters to people can be large.

### Why AI agents

AI agents are software that acts. They call tools, edit files, query databases, and send messages, often through long sequences of steps. Both of the lessons above apply directly:

- **Failures live at the boundaries.** An agent can produce a reasonable-looking final answer while making an unsafe tool call along the way, or carry out a harmful task as a series of steps that each look harmless.
- **Final outputs are not the whole story.** Judging an agent only by its final output is like judging a codebase only by whether it compiles.

Software engineering and programming languages have decades of ideas for reasoning about systems like this: contracts, specifications, state, refinement, provenance, testing, and empirical evaluation. My research asks which of these ideas transfer to AI agents, and what new ideas we need where they don't.

That question is where I am starting my PhD. I expect my understanding of it to change, and I plan to use these notes to document how it does.
