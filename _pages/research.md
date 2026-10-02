---
layout: page
title: Research
permalink: /research/
description: Building reliable AI agents through software engineering and programming-language principles.
nav: true
nav_order: 1
---

AI agents no longer just answer questions. They **act**: calling tools, editing code, querying databases, and changing the systems around them. Once an agent can act, a mistake is no longer just a wrong answer; it is a wrong action. I study how to make those actions reliable, using ideas that software engineering and programming languages have refined for decades.

I came to this from software engineering. Years of building web, mobile, and AI systems taught me where software breaks, and my MSc thesis studied that empirically. Static analysis tools flag thousands of problems in a mature codebase, but maintainers need to know which ones will actually hurt, so I built a cross-project model that predicts which files will become maintenance hotspots. On projects it had never seen, the **top 20% of files it ranked contained about 82% of future hotspots, roughly 4.1× better than random**. AI agents are the next step on that path: software that acts on software, and that breaks in new ways.

### What I work on

- **Reliable AI agents.** Why agents fail when they use tools, and how to make them predictable.
- **Agent safety and security.** Catching unsafe tool use, untrusted inputs, and harmful side effects.
- **Programming languages for agents.** Contracts, state, refinement, and provenance as ways to reason about agent behavior.
- **AI + software engineering.** Agents as software that works on software.

My current work, in the [Laboratory for Software Design](https://lab-design.github.io/), focuses on the reliability and security of tool-using agents: judging an agent by the actions it takes along the way, not only by its final answer.

### Questions I'm exploring

- Can we write contracts for agent–tool interactions, and check them as the agent runs?
- How do we catch unsafe tool use before it causes harm?
- Can provenance explain _why_ an agent took a particular action?
- Which software engineering abstractions actually transfer to AI agents?

_Open questions I am working on, not results I am claiming._

### Open source

- **[Flutter Clean Architecture VS Code extension](https://github.com/resourceful-nebil/Flutter-Clean-Architecture-Starter-Kit-Template)** (350+ users). Scaffolds a full Clean Architecture feature for a Flutter app in one command, then detects and repairs structural drift. It is an early version of an idea I still care about: turning a project's implicit structural rules into something a tool can check.
- **[Technical debt prediction pipeline](https://github.com/maajidAwol/technical-debt)**. The full replication package for my MSc thesis: data processing, labeling, features, models, and evaluation.

### Education

<table class="table table-sm table-borderless">
  <tbody>
    <tr>
      <td style="width: 9rem;">2026 – present</td>
      <td><b>PhD in Computer Science</b><br>Tulane University, New Orleans, USA<br>Advisor: Dr. Hridesh Rajan</td>
    </tr>
    <tr>
      <td>2024 – 2026</td>
      <td><b>MSc in Software Engineering</b> (Fast Track Program)<br>Addis Ababa Science and Technology University, Ethiopia<br><i>Thesis: Predicting High-Risk Technical Debt in Open-Source Software Projects Using Machine Learning</i></td>
    </tr>
    <tr>
      <td>2021 – 2025</td>
      <td><b>BSc in Software Engineering</b>, with Very Great Distinction (GPA 3.78/4.0)<br>Addis Ababa Science and Technology University, Ethiopia</td>
    </tr>
  </tbody>
</table>

### Toolkit

Python · Java · TypeScript · ML · LLM APIs · empirical software engineering · Git · Docker · CI/CD
