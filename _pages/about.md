---
layout: about
title: home
permalink: /
subtitle: PhD Student in Computer Science · <a href='https://sse.tulane.edu/cs'>Tulane University</a> · School of Science and Engineering

profile:
  align: right
  # image: profile/abdulmajid.jpg # uncomment once assets/img/profile/abdulmajid.jpg exists (the build fails if the file is missing)
  image_circular: false # crops the image to make it circular
  more_info: >
    <p>Graduate Research Assistant</p>
    <p><a href="https://lab-design.github.io/">Laboratory for Software Design</a></p>
    <p>Tulane University</p>
    <p>New Orleans, LA</p>

selected_papers: false # includes a list of papers marked as "selected={true}"
social: true # includes social icons at the bottom of the page

announcements:
  enabled: true # includes a list of news items
  scrollable: true # adds a vertical scroll bar if there are more than 3 news items
  limit: 5 # leave blank to include all the news in the `_news` folder

latest_posts:
  enabled: true
  scrollable: true # adds a vertical scroll bar if there are more than 3 new posts items
  limit: 3 # leave blank to include all the blog posts
---

**I study reliable AI agents at the intersection of artificial intelligence, software engineering, and programming languages.**

[Research]({{ '/research/' | relative_url }}) · [Publications]({{ '/publications/' | relative_url }}) · [CV]({{ '/cv/' | relative_url }}) · [GitHub](https://github.com/maajidAwol) · [Email](mailto:maajidawol@gmail.com)

I am a PhD student in Computer Science at Tulane University, where I am a graduate research assistant in the [Laboratory for Software Design](https://lab-design.github.io/), advised by [Dr. Hridesh Rajan](https://sse.tulane.edu/cs/faculty/rajan). My interests lie at the intersection of artificial intelligence, software engineering, and programming languages, with an emphasis on making agentic systems more dependable when they interact with tools, software artifacts, and external environments.

Before starting my PhD, I completed a BSc (with Very Great Distinction) and an MSc in Software Engineering at Addis Ababa Science and Technology University, and worked as a software engineer on web, mobile, and AI-enabled systems. My master's thesis studied how to predict high-risk technical debt in open-source software projects using machine learning.

#### Current research

My current work focuses on **preventing compositional and decompositional attacks in AI agents**: cases where a harmful goal is split into steps that each look harmless, or where individually acceptable tool actions combine into an unsafe outcome. More broadly, I am interested in moving beyond judging agents only by their final outputs, and instead reasoning about the intermediate tool calls, parameters, state changes, and provenance that lead to those outcomes. This connects to ideas from software engineering and programming languages such as contracts, state, refinement, and provenance analysis.

Questions I am currently exploring:

- How can agent–tool interactions be specified and checked?
- How can we detect incorrect or unsafe tool use, including unsafe behavior that only appears when actions are composed?
- How can provenance help explain why an agent took a particular action?
- Which software engineering abstractions transfer effectively to AI agents?

These are open questions I am working on, not solved problems. More on the [research page]({{ '/research/' | relative_url }}).

#### How I approach research

I am drawn to questions that connect conceptual ideas with measurable software and system behavior. I value clear problem definitions, reproducible evaluation, meaningful baselines, and honest reporting of both positive and negative results. My engineering background shapes how I look at AI systems: through abstractions, interfaces, state, contracts, failure modes, and empirical evaluation.

[More about me →]({{ '/about/' | relative_url }})
