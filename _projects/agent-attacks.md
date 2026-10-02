---
layout: page
title: Compositional & Decompositional Attacks on AI Agents
description: "Ongoing PhD research · 2026–present. Preventing attacks that hide harmful behavior across individually harmless-looking agent steps."
importance: 1
category: research
---

**Status:** ongoing (PhD research, Laboratory for Software Design, Tulane University, 2026–present)

### Motivation

Tool-using AI agents carry out tasks as sequences of steps: they plan, call tools with parameters, read results, and update their state. Safety checks often look at one request or one action at a time. That leaves a gap. A harmful goal can be **decomposed** into sub-tasks that each look benign, and actions that are individually acceptable can **compose** into an unsafe outcome. Neither shows up when each step is inspected in isolation.

### What I am working on

My current research investigates how to prevent these compositional and decompositional attacks. I am approaching the problem from a software engineering and programming-language perspective, treating an agent's trajectory (its tool calls, parameters, intermediate state, and the provenance of the information it acts on) as something that can be specified, tracked, and checked, rather than judging only the final output.

### Focus areas

- Agent reliability and safety across multi-step interactions
- Tool-call and parameter-level behavior
- State tracked across long-running interactions
- Failure analysis and systematic evaluation
- Software engineering abstractions (contracts, refinement, provenance) applied to agents

_This is work in progress. Results will be added here once they are published._
