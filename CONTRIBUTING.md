# Contributing to GT3N Forge

Welcome, Builder. This document explains how to contribute to GT3N Forge missions and what to expect from the process.

---

## Quick Start

1. **Read the [Terms of Participation](./TERMS.md)** -- understand what you're signing up for
2. **Sign the [Contributor License Agreement (CLA)](./CLA.md)** -- one-time, applies to all your future contributions
3. **Read the [Code of Conduct](./CODE_OF_CONDUCT.md)** -- our community standards
4. **Browse [Available Missions](./missions/)** -- find one that matches your track and rank
5. **Claim a mission** -- by opening an Issue in this repo with the mission ID
6. **Build it** -- using your own tools, AI assistants, and workflow
7. **Submit your work** -- via the Google Form linked in the mission spec
8. **Get validated** -- reviewers check your work against the mission's acceptance criteria
9. **Earn your Wall of Records entry** -- if approved, you receive XP, attribution, and a permanent verified record

---

## What is GT3N Forge?

GT3N Forge is a gamified open-source builder program operated by [GT3N Industries](https://gt3n.xyz). Builders contribute work to real GT3N projects (GOGSverse, REKORD, ARK, HERMES, PICASSO) and earn permanent recognition on the Wall of Records.

**This is an open-source contributor program.** All contributions are licensed under Apache 2.0 (code) or CC-BY 4.0 (design/content). GT3N and anyone else may use the outputs under license terms. Builders earn recognition through verified contributions on the Wall of Records.

The program model is the same as how Google maintains Kubernetes, Meta maintains React, or Vercel maintains Next.js -- a for-profit company maintaining open-source projects with a community of contributors who earn recognition and portfolio value through their work.

---

## Builder Tracks

Choose your track when you sign up:

- **Developer** -- Architecture, backend, systems, security, infrastructure
- **Vibe Coder** -- AI-assisted features, frontend, UI/UX, content, research, prototyping

Both tracks earn the same XP and ranks. Some missions are open to "any" track.

You can switch tracks once per 30 days. Your XP and rank carry over.

---

## How Missions Work

### Mission Structure

Each mission is a Markdown file in `missions/[project]/[mission-id].md`. The mission specifies:

- **Project** -- Which GT3N project it serves
- **Type** -- code | design | content | research | ops
- **Difficulty** -- starter (1x XP) | standard (2x) | advanced (5x) | elite (10x)
- **Target Track** -- developer | vibe_coder | any
- **XP Reward** -- Base XP before multipliers
- **Required Rank** -- Minimum rank to claim
- **Deliverables** -- Specific outputs with acceptance criteria
- **Validation Tier** -- Tier 1 (checklist) | Tier 2 (peer review) | Tier 3 (expert review)
- **License** -- Apache 2.0 (code) or CC-BY 4.0 (design/content)
- **Deployment Target** -- Where the output goes in the GT3N project

### Claiming a Mission

1. Browse `missions/[project]/` and find a mission that matches your track and rank
2. Open an Issue in this repo with the title: `[CLAIM] MSN-XXX: [Mission Title]`
3. Include in the issue body:
   - Your contributor handle
   - Confirmation you've signed the CLA
   - Estimated completion timeframe
4. Wait for a maintainer to add the `claimed` label (usually within 24 hours)
5. You now have up to 14 days to complete the mission (extendable on request)

### Claim Limits

- Maximum **3 active claims** per builder at any time
- Maximum **5 submissions** per day
- If 2 of your submissions are rejected in 24 hours, a 48-hour cooldown applies before new claims

### Releasing a Claim

If you can't complete a mission, release the claim by commenting on your claim Issue: `[RELEASE] No longer working on this`. No penalty -- this is better than missing the deadline silently.

---

## Building Your Submission

### Tools and AI

Use whatever tools work best for you:

- IDEs, editors, design software (Figma, Sketch, etc.)
- AI assistants (ChatGPT, Claude, Copilot, Midjourney, local models)
- Manual work, research, references

**AI disclosure is mandatory.** You must honestly report what AI tools you used and how. This is not a penalty -- it's transparency. The community values honest process documentation more than the absence of AI.

### Process Notes

Every submission requires process notes (minimum 50 words) explaining:

- How you approached the problem
- What decisions you made and why
- Where you used AI vs. did manual work
- Any challenges and how you resolved them

Process notes are part of the public Wall of Records entry. Write them like you'd want a future hiring manager to read them.

### Quality Standards

Reviewers evaluate submissions against:

- Does it meet the deliverables and acceptance criteria?
- Is the work quality acceptable for the mission difficulty?
- Are process notes substantive and honest?
- Is the AI disclosure honest and detailed?
- Does the output align with the GT3N project's needs and aesthetic?

---

## Submission Process

### How to Submit

When your work is complete:

1. Go to the GT3N Forge Submission Form (link provided after claim approval)
2. Fill out:
   - Mission ID
   - Output URL (link to GitHub repo, Figma file, Google Doc, etc.)
   - Process notes
   - AI disclosure
   - AI tools used (multi-select)
   - AI percentage (0-100% slider)
   - File uploads (if applicable, up to 50MB)
3. Comment on your claim Issue: `[SUBMITTED] Form filed at [time]`

### What Happens Next

- **Tier 1 (Checklist):** Reviewed within 24 hours
- **Tier 2 (Quality Review):** Reviewed within 48 hours
- **Tier 3 (Expert Review):** Reviewed within 72 hours

You'll receive feedback in your claim Issue. Outcomes:

- **Approved** -- XP awarded, Wall of Records entry created, contribution merged
- **Rejected** -- Written feedback explaining why, no XP, claim closed
- **Revision Requested** -- Feedback provided, you may resubmit once

---

## Rank Progression

| Rank | XP | Reputation | Unlocks |
|------|-----|-----------|---------|
| Apprentice | 0 | 0 | Starter missions |
| Builder | 500 | 60 | Standard missions, Tier 1 review eligibility |
| Maker | 2,000 | 75 | Advanced missions, can propose missions |
| Architect | 8,000 | 85 | Elite missions, Project Lead eligibility |
| Core Contributor | 25,000+ | 90 + nomination | Revenue share eligibility, governance input |

Reputation is calculated from approved-vs-rejected ratio, weighted by mission difficulty. Higher difficulty submissions count more.

---

## Wall of Records

Every approved contribution becomes a permanent entry on the Wall of Records:

- Public and verifiable
- SHA-256 hashed and chained per builder
- REKORD-synced (Phase 3+)
- Becomes part of your portfolio forever

The Wall of Records is the permanent recognition layer -- a verifiable record that you did this work and that the work hasn't been altered since.

---

## Founder Builder Status

The first 15 builders to contribute during Phase 1 receive permanent **Founder Builder** status:

- A unique badge on their Wall of Records profile
- Recognition as the founding cohort
- A permanent place in GT3N Forge history
- First access to leadership opportunities as Forge grows

If you're reading this in Phase 1, you may be one of them.

---

## Community Standards

- Read and follow the [Code of Conduct](./CODE_OF_CONDUCT.md)
- Be respectful in reviews and discussions
- Submit honest work and honest disclosures
- Help fellow builders when you can
- Report issues through proper channels (not by harassing maintainers)

---

## Getting Help

- **General questions:** Post in the GT3N Forge Discord #help channel
- **Mission-specific questions:** Comment on the mission Issue
- **Conduct issues:** Email titan@gt3n.xyz (subject: "Conduct Report")
- **Account/admin issues:** Email titan@gt3n.xyz (subject: "Admin Issue")

---

## Maintainers

GT3N Forge is maintained by:

- **Girard Peter Tenazas** (Founder, GT3N Industries)
- **Gwen** (Co-maintainer)
- **Project Leads** (Architects who lead validation for specific GT3N projects)

---

## Thank You

Open-source communities are built on voluntary contribution and mutual respect. By contributing to GT3N Forge, you're helping build something that may eventually power multiple ecosystems -- from sports communities to healthcare to knowledge preservation.

You're not just building features. You're building the foundation of GT3N.

We see you, and the Wall of Records remembers.

---

**GT3N Industries**  
San Diego, California  
May 2026
