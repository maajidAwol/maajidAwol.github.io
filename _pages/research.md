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

- **Reliable AI agents.** Understanding how agents fail when they interact with tools, APIs, software repositories, and databases, and developing methods that make their behavior more reliable and predictable.
- **AI + software engineering.** Studying AI systems through a software engineering lens: how agents work with software artifacts, development tools, and complex software environments.
- **Programming languages for AI agents.** Adapting ideas such as contracts, refinement, state, provenance, and formal specification to reason about agent behavior.
- **Agent safety and security.** Detecting and mitigating incorrect or unsafe behavior caused by tool interactions, parameters, external state, and untrusted information.

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

For my MSc at Addis Ababa Science and Technology University, I studied how to **predict high-risk technical debt in open-source software projects using machine learning**, advised by Dr. Tesfaye Gidey. The thesis shifts the goal from _detecting_ debt, which static analysis tools already do at scale, to _prioritizing_ it: identifying which files are likely to become maintenance-intensive in the near future. Across 22 Apache Java projects, on projects the model had never seen, inspecting only the top 20% of files it ranked recovered about 82% of the files that became maintenance-intensive over the next six months, roughly 4.1× random inspection. The full pipeline is available as a [replication package](https://github.com/maajidAwol/technical-debt).

This work shaped my current direction: it taught me to treat software systems as objects of empirical study, and to care about the gap between what tools report and what actually matters to maintainers.
