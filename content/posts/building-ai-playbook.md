---
date: 2025-01-06
title: "Building AI playbook: How I solved cross-functional communication with AI"
---

I kept rewriting the same update for different stakeholders. Engineers wanted technical details upfront. Marketing needed business impact. Leadership just wanted the bottom line.

30-45 minutes per message. Every time.

The problem wasn't that I didn't know *what* to communicate. I didn't know *how* to structure it for different people.

So I built **Master Your Message (MYM)** - an AI playbook that structures my message in 2 minutes instead of 45.

---

## How MYM works

MYM is a multi-step workflow with guardrails, decision logic, and quality controls.

### Step 1: Safety checks and clarifying questions

Before generating anything, MYM checks for:
- Sensitive information (passwords, customer names, confidential details)
- Harmful language (profanity, harassment, threats)
- Legal/HR risks (firing, medical info, security breaches)

If triggered, MYM pauses and asks you to rephrase.

Then it asks 3 questions:
1. Who are you communicating with?
2. What action do you need from them?
3. How will you communicate this (Slack, email, meeting)?

### Step 2: Framework selection

Based on your answers, MYM matches your scenario to the right framework:

- **BLUF (Bottom Line Up Front)** - for executives needing decisions
- **PREP (Point-Reason-Example-Point)** - for technical recommendations
- **Observation-Impact-Question** - for feedback in 1:1s
- **Before-After-Bridge** - for showcasing results

### Step 3: Structured output

MYM drafts your message using the selected framework's structure.

**For BLUF:**
- Line 1: Your ask or main point
- Lines 2-4: Supporting context (2-3 sentences max)
- Line 5: Next steps

**For PREP:**
- Point: Your recommendation
- Reason: Why it matters
- Example: Concrete proof
- Point: Restate recommendation

### Step 4: Quality checks

Before delivering, MYM validates:
- Is the ask in the first 1-2 sentences?
- Does it follow the framework structure?
- Is it free of AI fluff?

If any check fails, MYM flags it and offers to regenerate.

---

## Example

Here's how I used MYM to propose a technical recommendation to our infrastructure team.

**My input:**

"I am writing a message to a tech lead to propose a Crowdin integration this will help automate update for translation and minimize manual check and I will send this via slack and I will like an alignment to our infrastructure."

**What MYM did:**

Extracted details:
- Audience: Tech lead
- Goal: Propose Crowdin integration and get alignment
- Format: Slack
- Topic: Automating translation updates

Selected framework: PREP (technical recommendation)

**What MYM generated:**

**Point:** "Hi [Name], I'd like to propose that we integrate Crowdin into our workflow to automate translation updates."

**Reason:** "Automating this process will reduce manual checks, lower the risk of outdated content, and better align our translation flow with existing infrastructure."

**Example:** "Right now, updates require periodic manual reviews, which slows down releases and introduces inconsistency. With Crowdin, we can sync source files automatically, push updates as they happen, and maintain a single, reliable path through our tooling."

**Point:** "Given these benefits, I recommend we move forward with exploring the Crowdin integration and ensure it aligns cleanly with our current infra setup. Happy to walk through an initial design if helpful."

---

**What changed:**

Before MYM, I'd write long paragraphs and bury my ask. After MYM generates the draft, I review and finalize to make sure it fits the situation.

This keeps me in control. MYM structures the message, but I verify it works.

Same information. One version gets alignment. The other gets lost in paragraphs.

---

## The results

**Before MYM:** 30-45 minutes rewriting the same update for different stakeholders

**After MYM:** 2 minutes to generate tailored messages

I built this during Maven's AI Playbook Challenge and it's become my daily tool for stakeholder communication.

Whether I'm proposing technical changes to Engineering, updating leadership on project progress, or sharing status with cross-functional partners, MYM structures it instantly.