---
layout: post
title: Why Reliability Matters for Tool-Using AI Agents
date: 2026-10-01 10:00:00-0500
description: A short note on why tool use changes the reliability question for AI systems.
tags: ai-agents reliability
categories: research-notes
related_posts: false
---

A language model that only produces text can be wrong, but its mistakes stay on the page until a person acts on them. An agent with tools is different: its outputs are **actions**. It can delete a file, run a shell command, transfer data, or call an external API. Once an agent can act, reliability stops being only about answer quality and becomes a question about the behavior of a software system.

### Why this is hard

A few properties make agent reliability harder than it first appears:

1. **Long trajectories.** Agents often take many steps before finishing a task. A small error early on can propagate, and the final state may depend on the whole sequence, not on any single step.
2. **External state.** Tools read and modify an environment the agent does not fully control. The same action can be safe in one state and harmful in another.
3. **Untrusted inputs.** Agents read web pages, documents, and tool outputs that may contain incorrect or adversarial content, and that content can influence later actions.
4. **Composition.** Steps that are each acceptable in isolation can combine into an unacceptable outcome, and a harmful goal can be broken into steps that each look benign. Checking one step at a time can miss both cases.

### A software engineering view

These problems are familiar in a new setting. Software engineers already deal with state, untrusted input, and components that interact in unintended ways. We have tools for them: specifications and contracts that state what an operation may do, type systems and static analyses that rule out classes of errors, provenance tracking that records where data came from, and testing methods that deliberately inject faults.

The research question is how to adapt these ideas to agents, whose "program" is generated at run time by a model rather than written in advance. For example:

- What is the right contract for a tool call, and who checks it?
- How do we track the provenance of the information behind an action?
- How do we evaluate an agent on its trajectory rather than only on its final answer?

These are some of the questions I am exploring in my PhD. I don't have answers yet, but I think the framing matters: treating agents as software systems makes much of what we already know about building reliable systems available to us.
