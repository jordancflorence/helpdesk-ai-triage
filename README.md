# Helpdesk AI — Self-Service Triage Platform

> A Claude-powered first-line support tool that helps non-technical employees resolve common IT issues independently — and generates structured, actionable tickets when they can't.

---

## Why This Exists

In a small, fast-growing company, the IT function often belongs to one person. That person is responsible for everything: networking, hardware, vendor coordination, and a daily stream of support tickets from staff who need help right now.

The problem is not a lack of skill. It is a lack of time.

When someone submits a ticket that says "my computer stopped working," a skilled IT operator still has to play 20 questions before they can diagnose anything. Multiply that across a full queue, and high-priority issues get buried under quick fixes the user could have handled themselves.

This project addresses that problem directly.

---

## What It Does

Helpdesk AI is a Claude Project configured to act as a first-line support layer for company staff. It is built for non-technical users — no assumed knowledge, no jargon, no frustration.

When a staff member has a tech issue, they describe it in plain English. The assistant:

1. Asks targeted clarifying questions to understand the issue
2. Attempts to walk the user through a fix, step by step, in plain language
3. Explains why each fix works — building user confidence for next time
4. If the issue is beyond self-service, generates a structured, complete IT ticket ready for handoff

The result: IT staff receive fewer low-complexity tickets, and the tickets they do receive contain everything needed to diagnose and act immediately.

---

## Triage Framework

The assistant uses a three-tier escalation model to determine how to respond:

| Tier | Label | Behaviour |
|------|-------|-----------|
| 🟢 Green | Self-service | Assistant guides user to a fix directly |
| 🟡 Yellow | Try and escalate | Assistant attempts basic fixes, then escalates with full context |
| 🔴 Red | Immediate escalation | No troubleshooting — direct to IT immediately |

**Green issues handled directly:**
- Password resets and login problems
- Email sync and sending failures
- WiFi and internet connectivity
- Printer offline or not responding
- Software not opening or crashing
- Slow device performance

**Red issues escalated without troubleshooting:**
- Security concerns (phishing, ransomware, suspicious popups)
- Lost or stolen devices containing company data
- System crashes or failure to boot
- Multiple users affected simultaneously
- Unexpected data loss

---

## Ticket Generation

When self-service fails, the assistant generates a structured ticket using everything collected during the conversation:

```
Name and location
What is not working (specific action, not "it's broken")
What the user sees instead (error messages, exact behaviour)
When it started
What has already been tried (and whether it worked)
Priority level: URGENT / HIGH / MEDIUM / LOW
```

The ticket is written in operational language — not the language of a frustrated user. The IT operator receives a complete diagnostic picture instead of a starting point.

---

## Tools Used

- **Claude (Anthropic)** — Project-based assistant with a custom system prompt
- No additional APIs, integrations, or infrastructure required
- Deployable to any team with Claude access

---

## Scope and Honest Limitations

This is a proof-of-concept built to demonstrate operational thinking, not a production deployment.

The assistant cannot verify whether a fix actually worked — it relies on the user's confirmation. In a production environment, this would be addressed through follow-up ticket status tracking or integration with a helpdesk platform.

What it does demonstrate:

- A structured approach to triage and prioritization under a broad workload
- Plain-language UX design for non-technical audiences
- Operational documentation standards (complete ticket fields, escalation logic)
- Practical AI tool configuration for real workflow problems

---

## Project Background

Built as a proof-of-concept for a live interview process at a tech-insurance startup. The role required a single IT operator to manage the full technical scope of a growing company — networking, hardware, vendor coordination, and internal support tickets.

The assistant was designed to reduce time spent on resolvable issues so the operator could focus on complex work that genuinely required expert attention. The hiring panel acknowledged the initiative directly.

---

## About

Jordan Florence is an IT operations professional with 9 years of experience in regulated environments, currently transitioning toward analyst and AI workflow roles. He holds a Contract Professor credential at St. Clair College, where he teaches mobile app development.

[GitHub](https://github.com/jordancflorence) | [LinkedIn](https://www.linkedin.com/in/jordanflorence/)
