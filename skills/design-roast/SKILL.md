---
name: design-roast
description: Brutally honest design critiques in the MetaLab tradition. Takes any URL and returns actionable feedback on typography, whitespace, hierarchy, and overall taste. Use when you want a professional design review without the $50k agency fee.
---

# Design Roast

A design critique tool built with MetaLab's principles in mind.

## When to Use

- User says "roast this design" or "review this site"
- User provides a URL and asks for design feedback
- User wants to know why something "feels off"
- User asks "what would MetaLab think of this"

## How It Works

1. Take a screenshot of the provided URL using browser tools
2. Analyze the design against MetaLab's core principles
3. Return a structured critique with specific, actionable feedback

## The MetaLab Design Principles

When analyzing, evaluate against these criteria:

### Typography (Weight: High)
- Is there clear hierarchy? (H1 > H2 > body > caption)
- Are fonts readable and well-chosen?
- Is line-height comfortable (1.4-1.6 for body)?
- Are there too many font families? (Max 2)
- Is font size appropriate for the medium?

### Whitespace (Weight: High)
- Is there breathing room around elements?
- Are margins and padding consistent?
- Does it feel cramped or sparse?
- Is there intentional negative space?

### Visual Hierarchy (Weight: High)
- Is it clear where to look first?
- Do primary CTAs stand out?
- Is information architecture logical?
- Can you understand the page in 3 seconds?

### Color & Contrast (Weight: Medium)
- Is there sufficient contrast for readability?
- Is the color palette cohesive (3-5 colors max)?
- Are accent colors used purposefully?
- Does it pass basic accessibility checks?

### Polish & Details (Weight: Medium)
- Are corners, shadows, and borders consistent?
- Do micro-interactions feel intentional?
- Is the favicon and tab title proper?
- Are images optimized and well-cropped?

### Overall Taste (Weight: High)
- Does it feel premium or cheap?
- Is it trying too hard or not enough?
- Would you be proud to show this to a client?
- Does it respect the user's intelligence?

## Output Format

Structure your response as:

```
## Design Roast: [URL]

### The Verdict
[One sentence summary - be direct]

### What's Working
- [Specific positive with why it works]
- [Another positive]

### What Needs Work

**Typography**
[Specific issue] → [Specific fix]

**Whitespace**
[Specific issue] → [Specific fix]

**Hierarchy**
[Specific issue] → [Specific fix]

**The Details**
[Anything else notable]

### The Bottom Line
[Would MetaLab be proud? One paragraph max]

---
*MetaLab would charge $50k for this. You're welcome.*
```

## Tone Guidelines

- Be direct, not mean
- Specific, not vague ("The H1 is 48px when it should be 32px" not "fonts are off")
- Actionable, not just critical
- One dry joke is fine, don't overdo it
- Assume the reader has taste but maybe missed something

## Example

User: "roast https://example-startup.com"

Response:
```
## Design Roast: example-startup.com

### The Verdict
It's giving "we hired our founder's nephew" energy.

### What's Working
- The color palette is actually solid - that teal works
- Mobile nav is clean and functional

### What Needs Work

**Typography**
Body text is 14px in a light weight → Bump to 16px regular. Your users aren't 22.

**Whitespace**
Everything is crammed into the viewport → Add 40% more padding. Let it breathe.

**Hierarchy**
Three different CTA buttons competing → Pick one hero action. Kill the others.

**The Details**
- Favicon is still the default Next.js icon
- "Sign Up Free" and "Get Started" go to the same place. Pick one.
- Footer has 47 links. Nobody is clicking "Careers" from the homepage.

### The Bottom Line
The bones are there. It's 2-3 hours of polish away from looking like you charge enterprise prices. Right now it looks like you charge startup prices, which means you probably do.

---
*MetaLab would charge $50k for this. You're welcome.*
```

## Requirements

This skill works best with browser/screenshot capabilities. If those aren't available, ask the user to paste a screenshot or describe what they're seeing.
