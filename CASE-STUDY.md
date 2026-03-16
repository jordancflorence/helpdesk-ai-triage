# Case Study: Helpdesk AI — Self-Service Triage Platform

**Type:** Proof-of-concept | AI workflow design  
**Context:** Built for a live interview process at a tech-insurance startup  
**Tools:** Claude (Anthropic), custom system prompt configuration  

---

## The Problem

The role being interviewed for was a jack-of-all-trades IT position at a fast-growing startup. One person, responsible for everything: network infrastructure, hardware procurement and maintenance, vendor coordination, AV systems, and internal support tickets submitted by company staff.

The scope was intentionally broad. That breadth was the point of the role.

The operational challenge was obvious: with that volume and variety of responsibility, time management becomes the core competency. A skilled operator who spends the first three hours of their day walking users through password resets and cache clears is not available for the infrastructure work that actually requires expertise.

The question I brought into the interview was: how do you protect high-priority time in a one-person IT function?

---

## The Approach

Rather than proposing a process document or a ticketing policy, I built a working tool.

Helpdesk AI is a Claude Project configured as a first-line support assistant for non-technical staff. The core design principle was that most IT tickets are not IT problems — they are communication problems. Users do not know how to describe what is wrong, which means operators spend significant time translating "my computer stopped working" into something diagnosable.

The assistant addresses this at the source.

**For resolvable issues:** The assistant guides the user through a fix in plain language, step by step, with explanations of why each step works. No jargon. No assumed knowledge. The user either solves the problem themselves or understands it well enough to prevent it next time.

**For complex issues:** The assistant collects everything an IT operator needs — device type, operating system, exact error behaviour, timeline, steps already attempted — and formats it into a structured ticket. The operator receives a complete picture on first read, not a starting point for more questions.

**For security and critical issues:** The assistant escalates immediately without attempting to troubleshoot. Speed matters more than self-service when data or system integrity is at risk.

---

## Triage Design

The escalation framework was the core operational decision in this build.

Three tiers — self-service, try-and-escalate, immediate escalation — map directly to the real cost of operator time. Green issues (password resets, WiFi drops, email sync failures) should never reach the IT queue if the user can be guided to a fix in under five minutes. Yellow issues warrant one or two attempts before escalation. Red issues bypass the assistant entirely and go straight to IT with no delay.

This is not a novel concept in IT operations. What matters is that it is encoded into the tool's behaviour, not left to the judgment of a non-technical user who does not know what tier their problem belongs to.

---

## What It Demonstrates

This project was not built to replace an IT operator. It was built to make one more effective.

The design reflects how I approach operational problems with broad scope and constrained resources:

- **Prioritization by impact** — not all tickets are equal, and the system reflects that
- **Process design for non-expert users** — the tool meets users where they are, not where IT wishes they were
- **Documentation as a workflow output** — the ticket format is not an afterthought, it is the product when self-service fails
- **Honest scoping** — the assistant acknowledges its limits and escalates rather than guesses

---

## Limitations and What I Would Build Next

The assistant cannot verify whether a fix worked. It relies on the user's word. In a production environment, this gap would be addressed through integration with a helpdesk platform (such as Jira Service Management or Freshdesk) where ticket status and resolution confirmation are tracked systematically.

Additional improvements for a production build:
- Category tagging for ticket routing (hardware vs. software vs. network)
- Recurring issue detection with a flag for pattern escalation
- Conversation logging for audit and quality review purposes

---

## Outcome

The hiring panel acknowledged the initiative directly. The role ultimately went to a candidate with stronger networking credentials — a gap that was identified clearly and had nothing to do with the quality of the work. The panel's feedback confirmed the project landed as intended: as evidence of operational thinking and a builder mentality, not just a resume claim.

---

## About

Jordan Florence is an IT operations professional with 9 years of experience in regulated financial environments, currently transitioning toward analyst and AI workflow roles. He holds a Contract Professor credential at St. Clair College, where he teaches mobile app development.

[GitHub](https://github.com/jordancflorence) | [LinkedIn](#)
