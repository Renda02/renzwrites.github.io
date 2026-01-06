---
date: 2025-01-07
title: "Building AI playbook: How I solved cross-functional communication with AI"
---

If you lead cross-functional initiatives, you know explaining context differs by stakeholder. Here's the AI playbook I built to structure my message for any audience without spending 45 minutes rewriting.

Leading cross-functional initiatives at Nexthink, I kept doing two things that slowed me down:
- Burying key points in long paragraphs
- Not stating my ask clearly

I'd write detailed updates explaining context, progress, blockers, then my manager would reply: "Sounds good, what do you need from me?"

The problem wasn't that I didn't know *what* to communicate. It's that I didn't know *how* to structure it for different stakeholders.

Engineers wanted technical details upfront. Marketing needed business impact. Leadership just wanted the bottom line and a clear ask.

I was spending 30-45 minutes rewriting the same update for different people.

**So I built Master Your Message (MYM)**, an AI playbook that asks clarifying questions about my stakeholder and structures my message using the right framework.

---

## What is an AI playbook?

AI playbooks are structured workflows that guide AI through multiple steps with clear inputs, decision logic, and quality controls.

Think of them as **recipes for AI**. Instead of "just prompt better," you build a system that works the same way every time.

Here's the difference:

**Without a playbook:**
"Rewrite this update for my tech lead"
→ You get a generic draft that still needs heavy editing

**With MYM playbook:**
MYM asks clarifying questions first:
- Who are you communicating with?
- What's the channel/format?
- What do you need from them?

Then it selects the right framework and drafts a structured message.

---

## How MYM works

MYM is built as a multi-step AI playbook. Not a single prompt, but a structured workflow with guardrails, decision logic, and quality controls at each stage.

### Step 1: Guardrails check and clarifying questions

Before MYM generates anything, it reviews your input for violations:

**Sensitive information detection:**
- Passwords, tokens, customer names
- Confidential details, internal incidents

**Harmful language detection:**
- Profanity, harassment, discriminatory language
- Threats or toxic tone

**Legal/HR/Compliance risk detection:**
- Firing, contract termination, reporting misconduct
- Medical information, security breaches

If any guardrail is triggered, MYM pauses and asks you to rephrase or directs you to HR/management for sensitive situations.

**Then it asks 3 clarifying questions:**
1. Who specifically will receive this message?
2. What action do you need from them?
3. How will you communicate this (Slack, email, meeting)?

### Step 2: Framework selection and message generation

Based on your answers, MYM matches your scenario to the right framework:

**BLUF (Bottom Line Up Front)** when:
- Audience = executives or senior leadership
- Format = Slack or email
- Goal = decision or approval needed

**PREP (Point-Reason-Example-Point)** when:
- You're recommending a technical approach
- You're proposing a solution
- You're arguing for a decision

**Observation-Impact-Question** when:
- You're giving feedback in a 1:1
- You're suggesting process improvements
- You're discussing behavior casually

**Before-After-Bridge** when:
- You're presenting results
- You're doing a demo
- You're showcasing achievements

### Step 3: Structured output

Once the framework is selected, MYM drafts your message using that framework's structure:

**For BLUF:**
- Line 1: Your ask or main point
- Lines 2-4: Supporting context (2-3 sentences max)
- Line 5: Next steps or what you need

**For PREP:**
- Point: Your recommendation
- Reason: Why it matters (business value)
- Example: Concrete proof (data, metrics)
- Point: Restate recommendation

**For Observation-Impact-Question:**
- Observation: "I noticed [specific behavior]"
- Impact: "This leads to [consequence]"
- Question: "What are your thoughts?"

**For Before-After-Bridge:**
- Before: The problem (vivid, relatable)
- After: The results (specific metrics)
- Bridge: How you got there (technical details)

### Step 4: Validation checks

Before delivering the message, MYM runs quality checks:

**Ask clarity validation:**
- Is the ask stated in the first 1-2 sentences?
- Is the ask specific and actionable?

**Framework adherence:**
- Does the message follow the selected framework structure?
- Are all required components present?

**Output quality:**
- Is the message free of AI fluff?
- Is the tone appropriate for the stakeholder?

If any check fails, MYM flags it and offers to regenerate.

---

**The process:**

1. Detect guardrail violations, pause if needed
2. Gather scenario context, ask clarifying questions
3. Match scenario to framework, apply decision logic
4. Generate structured message, validate quality
5. Deliver clean output

That's why it takes 2 minutes instead of 45. You're not editing vague AI drafts. You're using a system that knows how to structure your message.

---

## Example

Here's how I used MYM to propose a technical recommendation to our infrastructure team.

### My input:

"I am writing a message to a tech lead to propose a Crowdin integration this will help automate update for translation and minimize manual check and I will send this via slack and I will like an alignment to our infrastructure."

### What MYM did:

**Extracted details:**
- Audience: Tech lead
- Goal: Propose Crowdin integration and get alignment with infrastructure team
- Format: Slack
- Topic: Automating translation updates and reducing manual checks

**Selected framework:** PREP (Point-Reason-Example-Point) because this is a technical recommendation

### What MYM generated:

**Point:** "Hi [Name], I'd like to propose that we integrate Crowdin into our workflow to automate translation updates."

**Reason:** "Automating this process will reduce manual checks, lower the risk of outdated content, and better align our translation flow with existing infrastructure."

**Example:** "Right now, updates require periodic manual reviews, which slows down releases and introduces inconsistency. With Crowdin, we can sync source files automatically, push updates as they happen, and maintain a single, reliable path through our tooling."

**Point:** "Given these benefits, I recommend we move forward with exploring the Crowdin integration and ensure it aligns cleanly with our current infra setup. Happy to walk through an initial design if helpful."

---

**What changed:**

Before MYM, I'd write long paragraphs and bury my ask in explanations. After MYM generates the draft, I review it and finalize it to make sure the message is clear and appropriate.

This keeps me in control of the final output. MYM structures the message, but I verify it fits the situation. AI helps, it doesn't replace my judgment.

Same information. One version gets alignment. The other gets lost in paragraphs.

---

## What makes MYM different from "just ask ChatGPT"

**Built-in guardrails:**
- Detects sensitive information, offensive language, and HR/legal risks
- No generic AI fluff like "Here's a draft for you..."

**Clarifying questions before generating:**
- MYM won't draft anything until it understands your stakeholder, format, and ask
- No vague, one-size-fits-all messages

**Framework matching:**
- Automatically selects the structure that fits your scenario
- You don't need to know communication theory to use it

**Clean, ready-to-send output:**
- Delivers structured messages you can paste directly into Slack or email
- Minimal editing required

---

## The results

**Before MYM:**  
30-45 minutes rewriting the same update for different stakeholders

**After MYM:**  
2 minutes to generate tailored messages, and they're better structured than what I'd write manually

I built this during Maven's AI Engineering course and it's become my daily tool for stakeholder communication.

Whether I'm proposing technical changes to Engineering, updating leadership on project progress, or sharing status with cross-functional partners, MYM structures it instantly.


