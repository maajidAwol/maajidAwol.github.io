---
layout: page
title: research
permalink: /research/
description: Building reliable AI agents through software engineering and programming-language principles.
nav: true
nav_order: 1
---

My research focuses on the reliability of AI agents and the software systems around them. I am particularly interested in how concepts from software engineering and programming languages can help us reason about, evaluate, and improve agent behavior. This is my current research direction as an early-stage PhD student in the [Laboratory for Software Design](https://lab-design.github.io/) at Tulane University, and it is still evolving.

---

### Research interests

#### Reliable AI agents

AI agents increasingly interact with tools, APIs, software repositories, databases, and other external systems. I am interested in understanding the failure modes that arise from these interactions and in developing methods that make agent behavior more reliable and predictable.

<small>_AI agents · reliability · agentic systems · tool use_</small>

#### AI + software engineering

I study AI systems through a software engineering lens, including how agents interact with software artifacts, development tools, and complex software environments.

<small>_AI4SE · software engineering · agentic software engineering_</small>

#### Programming languages for AI agents

Programming-language concepts such as contracts, refinement, provenance, state, and formal specification provide useful abstractions for reasoning about agent behavior. I am interested in adapting these ideas to agentic systems.

<small>_programming languages · contracts · state · provenance · verification_</small>

#### Agent safety and security

I am interested in how tool interactions, parameters, external state, and untrusted information can cause agents to behave incorrectly or unsafely, and in techniques for detecting and mitigating these failures.

<small>_agent safety · security · tool misuse · provenance_</small>

---

### Current research

My current work focuses on the **reliability and security of tool-using AI agents**. I am interested in moving beyond evaluating agents only by their final outputs, and instead reasoning about the intermediate interactions, state changes, tool calls, parameters, and provenance that lead to those outcomes. This direction draws on software engineering and programming-language ideas including contracts, state management, refinement, provenance analysis, and fault-based evaluation. The goal is to develop systematic ways to identify agent failures, characterize their causes, and evaluate techniques that improve reliability.

**Questions I am exploring**

- How can agent–tool interactions be specified and checked?
- How can we detect incorrect or unsafe tool use?
- How should state be represented and managed across long-running agent interactions?
- How can provenance help explain why an agent produced a particular action?
- How can we systematically evaluate agent reliability under realistic failures?
- Which software engineering abstractions transfer effectively to AI agents?

These are open questions I am investigating, not results I am claiming.

---

### Previous research: technical debt prediction

For my MSc at Addis Ababa Science and Technology University, I studied how to **predict high-risk technical debt in open-source software projects using machine learning**, advised by Dr. Tesfaye Gidey. The thesis shifts the goal from _detecting_ debt, which static analysis tools already do at scale, to _prioritizing_ it: identifying which files are likely to become maintenance-intensive in the near future. See the [project page]({{ '/projects/technical-debt/' | relative_url }}) for details.

This work shaped my current direction: it taught me to treat software systems as objects of empirical study, and to care about the gap between what tools report and what actually matters to maintainers.

---

### How I approach research

I am interested in research questions that connect conceptual ideas with measurable software and system behavior. I value clear problem definitions, reproducible evaluation, meaningful baselines, and explicit analysis of both positive and negative results. My software engineering background influences how I approach AI research: I try to understand systems through their abstractions, interfaces, state, contracts, failure modes, and empirical behavior.
