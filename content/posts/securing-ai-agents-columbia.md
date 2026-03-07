---
title: "Securing AI Agents: Guest Lecture at Columbia University"
date: 2026-03-06
tags: ["AI Security", "AI Agents", "Prompt Injection", "LLM Security", "MCP", "Cybersecurity"]
draft: false
---

I had the honor of giving an [invited guest lecture](https://github.com/lghupan/intro-to-agentic-security/blob/main/ai-agents-security-slides.pdf) at Columbia University, hosted by [Prof. Xiaofan (Fred) Jiang](https://fredjiang.com/), on the topic of **"Securing AI Agents."**

## Why AI Agent Security Matters

Autonomous agents like [OpenClaw](https://openclaw.ai/) have the potential to transform daily work — automating complex, multi-step tasks that previously required human judgment at every turn. But with that power comes a critical question: **how do we ensure it's safe to deploy them?**

## What We Covered

The lecture walked through the full threat landscape and defense stack for agentic AI systems:

### Threat Vectors
- **Prompt injection** — manipulating agent behavior through crafted inputs in the environment
- **MCP supply chain attacks** — compromising the tools and integrations agents rely on

### Defense Layers
- **Model level** — aligning the model itself to resist manipulation
- **System level** — sandboxing agent execution to limit blast radius
- **Application level** — runtime monitoring and anomaly detection, including Agentic AI Detection and Response (ADR) in production at Uber

**The slides and materials are available in the [GitHub repo](https://github.com/lghupan/intro-to-agentic-security).**

## A Side Quest: AI-Generated Slides Are Still Broken

One unexpected finding from preparing this talk: **generating presentation slides is still an unsolved problem for AI agents.**

I tried three approaches before landing on something workable:

| Approach | Result |
|---|---|
| Python / python-pptx | Layout control was painful; output looked mediocre |
| AI in Google Slides | Inconsistent formatting, hard to iterate |
| HTML generation | Reasonable, but fragile for complex layouts |
| **Claude Code + LaTeX Beamer** | **Winner — precise, reproducible, version-controllable** |

Claude Code driving LaTeX Beamer ended up being the most reliable pipeline. It's not the most glamorous toolchain, but the output is clean and the whole thing is scriptable. Curious what stacks others are using — drop a comment below.
