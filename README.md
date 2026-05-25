# GT3N Forge

> A gamified open-source builder program for the GT3N Industries ecosystem.

[![Hosted on GitHub](https://img.shields.io/badge/Hosted-GitHub-181717?logo=github)](https://github.com/GT3Nxyz/forge)
[![License: Apache 2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](./LICENSE)
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](./LICENSE-CC-BY-4.0)
[![Status: Phase 1](https://img.shields.io/badge/Status-Phase%201-yellow)](#status)

---

## What is GT3N Forge?

GT3N Forge is the **open-source builder program** for [GT3N Industries](https://gt3n.xyz), a venture studio architecting ecosystems across sports, healthcare, knowledge preservation, and creative verticals.

**The premise:** GT3N builds multiple products. Builders contribute open-source work to those products through gamified missions, earning permanent recognition on the **GT3N Wall of Records** -- a public, cryptographically verified ledger of completed contributions.

```
Pick a mission  ->  Build it (AI-assisted or manual)  ->  Submit
       ->  Get validated  ->  Earn XP and Wall of Records entry
       ->  Level up  ->  Unlock harder missions
```

Inspired by Linux, Apache, and React: **a for-profit company maintaining open-source projects, with a community of contributors who earn recognition through verified work.**

---

## The GT3N Ecosystem

Missions in Forge contribute to GT3N's portfolio of projects:

| Project | Vertical | Status |
|---------|----------|--------|
| **GOGSverse** | Sports community | Active |
| **REKORD** | Knowledge-as-a-Service (KaaS) | Building |
| **GT3N Forge** | Builder platform (self-build) | Building |
| **ARK** | Senior living healthcare | Planned |
| **HERMES** | Health practitioner network | Planned |
| **PICASSO** | Digital art preservation for kids | Planned |

---

## How It Works

### For Builders

1. **Pick a track.** Are you a Developer (architecture, backend, systems) or a Vibe Coder (AI-assisted, design, content, research)? Both tracks earn the same XP and ranks.
2. **Browse missions.** Each mission belongs to a GT3N project, specifies deliverables and acceptance criteria, and has a difficulty level (Starter, Standard, Advanced, Elite).
3. **Claim a mission.** Max 3 active claims at a time.
4. **Build.** Use any tools you want -- ChatGPT, Claude, Copilot, manual coding, Figma, whatever fits the job.
5. **Submit.** Provide your output, process notes (how you did it), and an honest AI disclosure (what AI you used and how).
6. **Get validated.** Reviewers approve, reject, or request revisions.
7. **Earn XP and recognition.** Approved missions award XP scaled by difficulty (1x starter, 2x standard, 5x advanced, 10x elite).
8. **Progress.** Build your verified portfolio. Unlock harder missions. Become a Project Lead.

### Rank Ladder

```
Apprentice  ->  Builder  ->  Maker  ->  Architect  ->  Core Contributor
   0 XP        500 XP      2,000 XP    8,000 XP        25,000+ XP
```

Each rank unlocks:
- More complex missions
- Peer review eligibility
- The ability to propose new missions
- Project Lead roles
- Governance input

---

## What Makes Forge Different

| Feature | Why It Matters |
|---------|---------------|
| **Verified contributions** | Every approved submission is cryptographically hashed (SHA-256), chained per-builder, and recorded immutably. Your portfolio isn't a list of claims -- it's a verifiable proof chain. |
| **The GT3N Wall of Records** | Public, permanent, cryptographically verifiable ledger of every approved contribution. Survives platforms, survives time. |
| **REKORD-backed integrity** | Contributions sync to REKORD (GT3N's Knowledge-as-a-Service platform) for institutional-grade preservation. Your work survives platform changes. |
| **AI is a tool, not the platform** | Bring your own AI. We track usage transparently, not punitively. |
| **Real work, real impact** | Missions feed into actual GT3N products. No fake tasks. Your output ships. |
| **Open source by default** | Every contribution released under Apache 2.0 (code) or CC-BY 4.0 (design/content). Same model as Linux, Apache, React, Vercel, Supabase. |

---

## What Forge is NOT

To be clear about the relationship:

- ❌ **Not employment.** No wages, no benefits, no W-2 or 1099 for participation.
- ❌ **Not freelancing.** No invoices, no contracts per project.
- ❌ **Not volunteering for a non-profit.** GT3N is for-profit; contributions are open source and may be used commercially by GT3N and anyone else.

Forge is a **gamified open-source contributor program** -- similar in nature to how Google maintains Kubernetes, Meta maintains React, or Vercel maintains Next.js. The company benefits from the open-source work; contributors benefit from verified portfolio building and community recognition.

See the full [Terms of Participation](./TERMS.md) for details.

---

## The Wall of Records

GT3N Forge's central recognition layer:

```
Every approved submission becomes a permanent record on the Wall:

  - Builder handle (public)
  - Mission title + project
  - Date submitted + date approved
  - SHA-256 hash of output (re-verifiable by anyone)
  - Chain link to builder's previous record
  - License type (Apache 2.0 or CC-BY 4.0)
  - Reviewer attribution
  - XP awarded
  - Direct link to output

The Wall is:
  - Public  (anyone can browse)
  - Permanent  (never deleted)
  - Verifiable  (anyone can re-hash and check)
  - Chained  (per-builder hash chain proves no record was altered)
  - REKORD-synced for institutional preservation
```

A Wall of Records entry is more verifiable than any letter of recommendation, certificate, or unverified portfolio claim. It proves you did the work, when you did it, and that the work hasn't been altered since.

---

## Status

GT3N Forge is currently in **Phase 1** -- a hand-picked, invite-only no-code MVP. We're validating the core loop with 5-15 trusted Founder Builders before scaling.

**Roadmap:**

- **Phase 1** (Months 1-3): Open-source contributor program launch. No-code MVP. Wall of Records.
- **Phase 2** (Months 3-6): Custom platform build on Cloudflare. Same model, real platform.
- **Phase 3** (Months 6-12): REKORD integration. Contributions sync to REKORD's PostgreSQL + pgvector for institutional preservation and semantic search.

---

## How to Get Involved

**For now (Phase 1):** Forge is invite-only. If you've been invited, you'll receive a welcome email with onboarding details.

**Interested in becoming a builder later?** Star this repo and watch for announcements. Phase 2 will open to a broader group.

**Want to partner or contribute as a project?** GT3N Industries is exploring early-stage partnerships for builders interested in contributing to specific verticals. Reach out via [GT3N's contact channels].

---

## Founder Builders

The first 15 builders to contribute during Phase 1 receive permanent **Founder Builder** status:

- A unique badge on their Wall of Records profile
- Recognition as the founding cohort
- First access to leadership opportunities as Forge grows
- A permanent place in the GT3N Forge origin story

If you've been invited to Phase 1, you may be one of them.

---

## Documentation

| Document | Purpose |
|----------|---------|
| [Terms of Participation](./TERMS.md) | Legal framework, IP, contributor rights |
| [Contributor License Agreement](./CLA.md) | The IP grant for contributions |
| [Code of Conduct](./CODE_OF_CONDUCT.md) | Community standards |
| [Contributing Guide](./CONTRIBUTING.md) | How to participate in missions |
| [Governance](./GOVERNANCE.md) | Decision-making structure |
| [GT3N Forge Manual](./MANUAL.md) | Complete program specification |

---

## License

GT3N Forge contributions are released under one of two licenses based on content type:

- **[Apache License 2.0](./LICENSE)** -- for code contributions (software, scripts, technical artifacts)
- **[Creative Commons Attribution 4.0](./LICENSE-CC-BY-4.0)** -- for design, content, research, and creative works

Builders retain copyright on their contributions and grant GT3N (and the public) rights under the applicable open-source license. See the [Contributor License Agreement](./CLA.md) for details.

---

## About GT3N Industries

GT3N Industries is a San Diego-based venture studio building ecosystems across multiple verticals. Founded by GP Tenazas, GT3N operates with a small core team and a builder network powered by GT3N Forge.

- 🌐 Website: [gt3n.xyz]
- 📧 Contact: titan@gt3n.xyz
- 🏛️ Patent: REKORD provisional patent 63/821,990 (USPTO)

---

> *"I'm a builder. I create real systems with GT3N Forge -- work that's verified, visible, and built to last."*

---

**Built by builders. Recognized forever on the Wall of Records.**

*Last updated: May 2026*
