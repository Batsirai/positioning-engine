---
name: positioning-engine
description: "Install the StoryBrand positioning framework into your OpenClaw agent. Runs an 8-question positioning session and outputs a one-liner, website hero copy, email subject lines, and 3 testable positioning angles. Used to reframe 'AI prompt packs' into 'revenue systems for AI operators' — same products, higher conversion."
requiredEnv: []
permissions:
  - filesystem: Writes positioning documents to working directory
source:
  url: https://github.com/Batsirai/carson-skills
  author: Carson Jarvis (@CarsonJarvisAI)
  github: https://github.com/Batsirai/carson-skills
  verified: true
security:
  note: No API keys required. All processing is done by your agent using your LLM. No credentials are stored or transmitted.
---

# Positioning Engine

> Stop sounding like everyone else. One session. Your unfair positioning angle — ready to test.

---

## What This Is

Bad positioning is why good products fail.

Not "bad" as in wrong — bad as in *vague*. "We help businesses grow." "AI-powered productivity tool." "The smart way to do X." These say nothing. They position against nothing. They give the buyer no reason to choose you.

The Positioning Engine installs the StoryBrand framework into your agent and runs a structured session that ends with:

1. **A one-liner** — your positioning in one sentence, specific enough to make someone say "that's for me" or "that's not for me"
2. **Website hero copy** — headline, subheadline, and CTA, ready to drop in
3. **Three positioning angles** — problem-led, outcome-led, villain-led — to A/B test
4. **Email subject lines** — 5 options built from your positioning, not from a generic template
5. **The villain** — the real enemy your buyer is fighting, which your product helps them defeat

---

## When to Load This Skill

- User says "help me with my messaging" or "I don't know how to explain what I do"
- User is writing a website, landing page, or pitch deck
- User's product isn't converting and they want to audit the positioning
- User is launching something new and needs a positioning foundation
- User asks "how do I stand out from competitors?"
- User says "my tagline feels generic" or "I don't know what to put on the homepage"
- User wants to A/B test messaging

---

## The Positioning Protocol

When this skill is active, your agent runs an 8-question positioning session. Do not skip questions. The answers compound — later outputs depend on earlier inputs.

### The 8 Questions

**Question 1: Who is your customer?**
Be specific. "Founders" is not specific. "Solo founders who ship their first SaaS product on weekends without a co-founder" is specific.

The more specific the customer, the more powerful the positioning. Broad positioning is for companies with $10M+ in marketing budget. You don't have that — specificity is your unfair advantage.

**Question 2: What is their #1 problem right now?**
Not their general pain. The one thing keeping them stuck today. The thing they searched for before finding you.

If you can't name it, you don't know your customer well enough yet. Ask more questions before proceeding.

**Question 3: What does that problem cost them?**
Quantify the cost — time, money, reputation, or opportunity. "It's frustrating" is not a cost. "It costs them 3 hours per week and one lost client per month" is a cost.

The more concrete the cost, the stronger the urgency in your positioning.

**Question 4: What do they want instead?**
The dream outcome. Not your product. The life they want after your product works.

"They want to feel organized" is weak. "They want to ship their first paying customer without working nights and weekends" is strong.

**Question 5: What have they already tried?**
List the alternatives — DIY, competitors, workarounds, hiring someone, YouTube tutorials. Every failed attempt is evidence of real demand.

**Question 6: Why did those attempts fail?**
This is where the villain lives. The villain is not a person — it's the force making every other solution inadequate.

Examples:
- The villain is complexity ("every solution requires a 90-minute onboarding")
- The villain is time ("they require hours of content creation per week")
- The villain is fragmentation ("10 separate tools that don't talk to each other")
- The villain is inaccessibility ("you need a $5K consultant to do this properly")

Name the villain. Your product is the weapon that defeats it.

**Question 7: What makes your solution different?**
One thing. Not five. Not "we're faster, cheaper, and easier." That's not positioning — that's a features list.

The one thing that makes your solution work when everything else has failed. Usually it's the mechanism — *how* you solve the problem, not just *that* you solve it.

**Question 8: What happens if they do nothing?**
The stakes. If they ignore this problem for 6 more months, what gets worse?

Stakes create urgency. Without stakes, there's no deadline. Without a deadline, people defer.

---

## Outputs

### 1. The One-Liner

**Formula:** "I help [specific customer] who [specific problem] get [specific outcome] without [specific obstacle]."

**Examples:**
- Weak: "I help businesses with AI tools."
- Strong: "I help solo founders who can't afford a marketing team build a 90-day content pipeline using one OpenClaw agent — without writing every post themselves."

Your one-liner should make the right people say "that's exactly for me" and everyone else say "that's not for me." Both reactions are correct.

---

### 2. Website Hero Copy

**Structure:**

```
HEADLINE:    [The outcome they want — not what you sell]
SUBHEADLINE: [How you get them there] — for [who specifically]
CTA BUTTON:  [What they get, not what they do]
```

**Rules:**
- Headline = outcome, not mechanism
- Subheadline = mechanism + audience
- CTA = specific action or specific thing they receive
- No "Learn more." No "Get started." Name the thing.

**Examples:**
- Weak headline: "AI-powered marketing tools"
- Strong headline: "Ship a 90-day content calendar this weekend"
- Weak CTA: "Get started"
- Strong CTA: "Get the content system" or "Build my pipeline"

---

### 3. Three Positioning Angles

Run all three. Test them with real copy. Keep the winner.

**Angle 1 — Problem-led:**
Lead with the pain. Make the problem feel felt before offering the solution.

Formula: "[Specific painful situation]? [Your product] was built for this."

**Angle 2 — Outcome-led:**
Lead with the result. Make the dream feel real before earning the right to pitch.

Formula: "[Dream outcome] — without [the thing they hate doing]."

**Angle 3 — Villain-led:**
Name the real enemy. Position your product as the weapon that defeats it.

Formula: "The problem isn't [surface symptom]. It's [real villain]. [Your product] kills the villain."

---

### 4. Email Subject Lines (5 Options)

Generated from your positioning, using these structures:
- Curiosity: "[Counterintuitive claim about their problem]"
- Direct: "[Specific outcome] in [timeframe]"
- Question: "Why is [common approach] still failing you?"
- Story: "I [did thing]. Here's what changed."
- Urgency: "[Deadline or scarcity hook] — [outcome]"

---

### 5. The Villain Statement

One paragraph naming the villain clearly. Used in:
- About page
- Sales page "why most solutions fail" section
- Email sequences
- Pitch decks

Format: "Most [buyers] try [common solution]. It fails because [villain]. [Your product] works because [mechanism that defeats villain]."

---

## Output Files

| File | Contents |
|------|----------|
| `positioning-[product]-[date].md` | Full positioning document |
| `one-liner-[product].md` | The one-liner, ready to use |
| `hero-copy-[product].md` | Website hero copy variants |
| `email-subjects-[product].md` | 5 subject line options |

---

## Conversation Starters

```
"Run the Positioning Engine on my product: [description]."

"My current tagline is [X]. Run the positioning protocol — what am I missing?"

"I sell [product] to [audience]. Find my positioning angle."

"My homepage copy isn't converting. Run the Positioning Engine and rewrite the hero section."

"I have two positioning angles I'm testing. Run the Positioning Engine and tell me which to lead with: [A] vs [B]."
```

---

## Common Positioning Mistakes

| Mistake | What It Sounds Like | Fix |
|---------|---------------------|-----|
| Feature-led headline | "47 AI-powered prompts" | → "Ship 3 months of content in a weekend" |
| Vague outcome | "Grow your business" | → "Go from 0 to $1K/month in 90 days" |
| Wrong hero | "We are the leading..." | → "You're one system away from..." |
| Missing villain | No enemy = no urgency | → Name the force making other solutions fail |
| Too many CTAs | "Learn more / Get started / Sign up" | → One button. One action. |
| Generic audience | "For entrepreneurs" | → "For solo operators with one agent and no team" |

---

## The StoryBrand Framework (Quick Reference)

| Element | Role | Your Version |
|---------|------|-------------|
| Hero | Your customer | Who they are specifically |
| Problem | What's broken | External + internal + philosophical |
| Guide | You | "We've been where you're going" |
| Plan | 3 steps | Simple enough to remember |
| CTA | Direct ask | One thing to do right now |
| Failure | What if they don't | The stakes |
| Success | What if they do | The dream outcome |

---

*Positioning Engine v1.0 — April 2026*  
*A product by Carson Jarvis (@CarsonJarvisAI)*  
*Part of the Agent Revenue OS — shopclawmart.com*
