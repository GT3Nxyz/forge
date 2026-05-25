# GT3N FORGE -- The Complete Manual

**Document:** GT3N Forge Pre-Build Manual  
**Version:** 1.0  
**Date:** April 15, 2026  
**Authors:** GP Tenazas, Gwen (OpenAI), Claude (Anthropic)  
**Classification:** Internal -- GT3N Industries  
**Status:** Design Complete, Pre-Build

---

## Table of Contents

**Part I -- Foundation (Read First)**

1. Executive Summary
2. What is GT3N Forge
3. GT3N Ecosystem Context
4. Vision Statement

**Part II -- Product Design**

5. Core Mechanics
6. Builder Tracks
7. Gamification System

**Part III -- Systems Architecture**

8. High-Level Architecture
9. Core Components
10. Data Flow
11. AI Integration Design
12. REKORD Integration

**Part IV -- Technical Specification**

13. Data Model & Schema
14. API Specification
15. Tech Stack
16. Security Architecture

**Part V -- Execution**

17. MVP Build Plan (Phased)
18. Scalability Design

**Part VI -- Risk & Mitigation**

19. Risk Analysis & Failure Modes

---

# PART I -- FOUNDATION

---

## 1. Executive Summary

GT3N Forge is a gamified, AI-assisted builder ecosystem that serves as the development engine for GT3N Industries' venture studio portfolio. Builders complete real-world missions to build actual GT3N products across multiple verticals (sports, healthcare, finance, creative, verification). Contributions are verified through REKORD's integrity layer, builders earn XP and rank through a gamified progression system, and future phases introduce tokenized rewards convertible through SMARTCoins ATM.

Forge solves the venture studio's core constraint: too many projects, not enough builders. Instead of hiring a development team for each project, Forge creates a scalable builder network where verified contributors produce real products across the entire GT3N ecosystem.

---

## 2. What is GT3N Forge

### 2.1 Definition

GT3N Forge is a gamified **open-source builder program** operated by GT3N Industries, a for-profit venture studio. Builders contribute open-source work to real GT3N projects (GOGSverse, REKORD, ARK, HERMES, PICASSO) and earn permanent recognition on the **Wall of Records** -- a public, cryptographically verified ledger of completed contributions.

- **Forge is the factory, not the product.** Builders contribute to all GT3N projects through Forge.
- **Forge produces builders. The builders produce GT3N's ecosystem.**
- **Forge follows the established open-source contributor program model** used by Google (Android, Kubernetes), Meta (React, PyTorch), Microsoft (VS Code), Vercel (Next.js), Supabase, HashiCorp, Discourse, and many other for-profit tech companies.

### 2.2 The Analogy

**Mario / Zelda:** Missions are levels. You progress, unlock harder challenges, gain abilities. The game IS the work. The work IS the game.

**Linux / Apache / React:** Open-source contributors building real software for real companies. Contributors earn reputation, portfolio strength, and community position -- not direct payment. The work itself is the value.

**Bitcoin Mining (Long-term Vision):** Eventually, verified contributions could earn convertible tokens via SMARTCoins ATM (Phase 5+). The work is real, the proof is cryptographic, the recognition is permanent -- and someday, the economic layer arrives.

The critical difference: the work itself is useful. Open-source contributions produce apps, designs, research, and systems that GT3N actually ships. The Wall of Records makes every contribution verifiable forever.

### 2.3 The Phased Loop

**Phase 1-3 (Current):**
```
Builder joins Forge
  -> Picks an open-source mission (any GT3N project)
  -> Completes the work (using their own tools/AI)
  -> Work is validated
  -> Contribution recorded on Wall of Records (SHA-256 hashed, chained)
  -> Output released under Apache 2.0 / CC-BY 4.0 license
  -> Builder earns XP + rank + permanent recognition
  -> Builder's portfolio grows with verified, public contributions
  -> GT3N (and anyone else) can use the output
  -> Eventually: contributions sync to REKORD for institutional preservation
```

**Phase 4+ (Future):**
```
Same loop, plus:
  -> Some missions are paid contractor work (proprietary, $50-300 per mission)
  -> Funded by GT3N project revenue, grants, or sponsor-funded missions
  -> OSS missions continue alongside paid missions
  -> Wall of Records remains universal recognition layer
```

**Phase 5+ (Vision):**
```
Same loop, plus:
  -> Token economy via SMARTCoins ATM
  -> Retroactive token allocation to all Wall of Records contributors
  -> Founder Builders (Phase 1 contributors) receive highest multiplier
  -> New contributions earn tokens going forward
  -> Tokens convertible to real-world value
  -> Subject to proper legal structure and securities compliance
```

### 2.4 Key Principles

| Principle | Description |
|-----------|-------------|
| Real work only | No fake tasks. Every mission produces output for a GT3N project. |
| Verifiable contributions | Every contribution is SHA-256 hashed, chained per builder, and REKORD-compatible. Wall of Records is the permanent portfolio. |
| Open source by default | Phase 1-3 contributions released under Apache 2.0 (code) or CC-BY 4.0 (design/content). Public goods, not proprietary value extraction. |
| Gamified progression | Levels, XP, ranks, badges, streaks. The game IS the work. |
| AI is a tool, not the platform | Builders bring their own AI. Forge tracks usage transparently, doesn't provide it. |
| Recognition first, economy later | Community built before tokens. Wall of Records is the foundation; tokens are the future layer. |
| Founder Builders earn the highest position | Early contributors (Phase 1) hold permanent founder status and receive amplified retroactive recognition when tokens eventually launch. |

---

## 3. GT3N Ecosystem Context

GT3N Industries is a venture studio that architects ecosystems across multiple verticals. Forge serves as the builder engine for the entire portfolio.

### 3.1 Project Portfolio

| Project | Vertical | Description | Status |
|---------|----------|-------------|--------|
| **GOGSverse** | Sports | Sports community platform | Active |
| **REKORD** | Verification / KaaS | Tamper-proof knowledge preservation system | Building (Patent 63/821,990) |
| **SMARTCoins ATM** | Finance | Token-to-real-value conversion system | Planned |
| **ARK** (ARuga at Kalinga) | Healthcare | Senior living healthcare platform | Planned |
| **HERMES** | Healthcare | Health practitioner network (serves ARK) | Planned |
| **PICASSO** | Creative | Digital art preservation for kids | Planned |
| **GT3N Forge** | Platform | Builder engine (self-build) | Building |

### 3.2 How Missions Flow Through the Ecosystem

```
GT3N Project needs a feature built
       |
       v
Founder / Project Lead breaks it into missions
       |
       v
Missions posted to Forge, tagged to project
       |
       v
Builder claims, builds, submits
       |
       v
Work validated -> recorded in REKORD -> XP awarded
       |
       v
Output deployed to actual GT3N project
```

### 3.3 Endgame

Once the builder pool is proven, GT3N takes on client projects and routes them through Forge as missions. Builders become GT3N's scalable workforce. GT3N becomes an agency powered by a gamified builder network, with every contribution verified by REKORD and every builder's track record immutable.

---

## 4. Vision Statement

"I'm a builder. I create real systems with GT3N Forge -- work that's verified, visible, and built for the digital economy."

---

# PART II -- PRODUCT DESIGN

---

## 5. Core Mechanics

### 5.1 The Core Loop

```
Pick Mission -> Build (AI or Manual) -> Submit -> Validate
    -> Earn XP & Recognition -> Level Up -> Unlock More Missions
```

### 5.2 Mission System

Every mission belongs to a GT3N project and targets a specific builder track.

**Mission Template:**

```
Mission: [Title]
Project: [GOGSverse / ARK / HERMES / PICASSO / Forge / REKORD / SMARTCoins]
Type: code | design | content | research | ops
Track: developer | vibe_coder | any
Difficulty: starter | standard | advanced | elite
XP: [number]
Rank Required: [minimum rank]
License: Apache 2.0 (code) | CC-BY 4.0 (design/content/research)

## Objective
[1-2 sentences: what the builder must produce]

## Deliverables
- [ ] [Specific output 1 with acceptance criteria]
- [ ] [Specific output 2 with acceptance criteria]

## Constraints
[Technical requirements, format, tools allowed]

## Validation Tier
[Tier 1: checklist | Tier 2: quality review | Tier 3: expert review]

## Context
[Why this matters to the project. Where the output lands.]

## Deployment Target
[e.g., "gogsverse-web/src/components/profile/"]

## License Note
Approved output will be released under [Apache 2.0 / CC-BY 4.0].
GT3N and others may use the contribution under license terms.
Builder retains copyright and earns Wall of Records entry.
```

### 5.3 Submission Requirements

Every submission includes:

| Field | Required | Description |
|-------|----------|-------------|
| Output URL | Yes | Link to deliverable (GitHub, Figma, Google Doc, etc.) |
| Output files | Optional | Attachments uploaded to R2 storage |
| Process notes | Yes (min 50 words) | How the builder approached and completed the work |
| AI disclosure | Yes (min 20 chars) | What AI tools were used and how |
| AI tools used | Yes | Structured list (e.g., Claude, Copilot, Midjourney) |
| AI percentage | Optional | Self-reported 0-100% of output that was AI-generated |

### 5.4 Validation Tiers

| Tier | For | Who Reviews | Time | SLA |
|------|-----|-------------|------|-----|
| **Tier 1: Checklist** | Starter missions, objective deliverables | Any Builder+ rank or Project Lead | 5-10 min | 24 hrs |
| **Tier 2: Quality Review** | Standard/advanced, subjective output | Maker+ peer or Project Lead | 15-30 min | 48 hrs |
| **Tier 3: Expert Review** | Elite missions, architecture, production code | Architect+ or Core Team | 30-60 min | 72 hrs |

### 5.5 Anti-Spam and Quality Gates

| Gate | Rule |
|------|------|
| Active claims | Max 3 per builder |
| Daily submissions | Max 5 per day |
| Process notes | Min 50 words required |
| AI disclosure | Required on every submission |
| Duplicate detection | SHA-256 hash compared against all prior submissions |
| Rejection cooldown | 2 rejections in 24hrs = 48hr cooldown |
| Reputation floor | Missions require minimum reputation scores |
| File limits | 50MB max per submission, whitelisted file types only |

---

## 6. Builder Tracks

### 6.1 Two Tracks

| Track | Who | Focus | Example Missions |
|-------|-----|-------|-----------------|
| **Developer** | Serious devs, CS background | Architecture, backend, infra, system design, security | "Build the HERMES practitioner search API" |
| **Vibe Coder** | Pseudo-dev + AI builders | AI-assisted features, frontend, UI/UX, content, research, prototyping | "Design the ARK patient intake flow in Figma" |

### 6.2 Shared Progression

Both tracks share:

- Same XP currency
- Same rank ladder
- Same reputation system
- Same REKORD contribution records
- Can take "any" track missions

### 6.3 Track Switching

Builders can switch tracks once per 30 days. XP and rank carry over. This prevents gaming while allowing genuine growth.

---

## 7. Gamification System

### 7.1 Rank Ladder

| Rank | XP Threshold | Reputation Min | Unlocks |
|------|-------------|----------------|---------|
| **Apprentice** | 0 | 0 | Starter missions only |
| **Builder** | 500 | 60 | Standard missions, Tier 1 review eligibility |
| **Maker** | 2,000 | 75 | Advanced missions, can propose missions |
| **Architect** | 8,000 | 85 | Elite missions, Project Lead eligibility, Tier 2 review |
| **Core Contributor** | 25,000+ | 90 + admin nomination | Revenue share eligibility, governance input, Tier 3 review |

### 7.2 XP Calculation

```
base_xp = mission.xp_reward

multipliers:
  difficulty:   starter=1x, standard=2x, advanced=5x, elite=10x
  first_clear:  +20% if first builder to complete this mission
  streak:       +10% if 3+ consecutive approvals
  speed:        +5% if submitted in <50% of deadline window

final_xp = floor(base_xp * product(multipliers))
```

### 7.3 Reputation Formula

```
reputation = (approved_weighted / total_weighted) * 100

where weight = difficulty multiplier of each submission
```

An approved elite submission counts more than an approved starter. Reputation drops with rejections. This prevents spam -- a builder with many rejections gets locked out of advanced missions.

### 7.4 Badge Categories

| Category | Examples |
|----------|---------|
| **Founder** | **Founder Builder** (first 15 contributors, permanent, non-transferable, highest retroactive token multiplier in Phase 5+) |
| **General** | First Build, Hat Trick (3 approvals in a row), Polymath (3+ types) |
| **Project** | GOGSverse Champion (5+ contributions), ARK Pioneer (first 10 contributors), Forge Smith (contributed to Forge itself) |
| **Track** | AI Artisan (vibe coder, 5 missions with AI score >= 4), System Thinker (developer, 3 architecture missions) |
| **Streak** | Speed Demon (submit < 24hrs, approved first try), Ironclad (10 approvals, 0 rejections) |
| **Special** | Chain Verified (first REKORD-synced contribution), Wall Architect (10+ verified Wall of Records entries) |

### 7.5 Wall of Records

The Wall of Records is GT3N Forge's central recognition layer -- the public ledger that distinguishes Forge from generic builder programs.

```
Every approved submission becomes a permanent record on the Wall:

  - Builder handle (public)
  - Mission title + project
  - Date submitted + date approved
  - SHA-256 hash of output (re-verifiable by anyone)
  - Chain link to builder's previous record (prev_record_hash)
  - License type (Apache 2.0 / CC-BY 4.0 / future paid license)
  - Reviewer attribution
  - XP awarded + breakdown
  - Direct link to output

The Wall is:
  - Public  (anyone can browse)
  - Permanent  (never deleted, even if builder leaves)
  - Verifiable  (anyone can re-hash the output and check)
  - Chained  (per-builder hash chain proves no record was altered)
  - Searchable  (filter by project, builder, date, type)
  - Browsable per-builder  (filterable view of each builder's chain)
  - REKORD-synced (Phase 3+) for institutional preservation
```

The Wall of Records is what early Builders earn in Phase 1-3 instead of cash. It is also the foundation for future retroactive token allocation (Phase 5+).

---

# PART III -- SYSTEMS ARCHITECTURE

---

## 8. High-Level Architecture

### 8.1 System Overview

```
                     GT3N VENTURE STUDIO
  +-----------+ +-----------+ +-----------+ +-----------+
  | GOGSverse | |  REKORD   | |    ARK    | |  HERMES   | ...
  |  Sports   | |   KaaS    | |Healthcare | | Practitioner|
  +-----------+ +-----------+ +-----------+ +-----------+
        |            |             |             |
        +------------+------+------+-------------+
                            |
                   +--------v--------+
                   |   GT3N FORGE    |
                   |  Builder Engine |
                   +--------+--------+
                            |
              +-------------+-------------+
              |                           |
         +----v----+              +-------v-------+
         |  Devs   |              |  Vibe Coders  |
         |(serious)|              | (AI + build)  |
         +---------+              +---------------+

  +-----------------------------------------------------+
  |                 INFRASTRUCTURE                       |
  | +----------+  +---------------+  +-----------------+ |
  | |  REKORD  |  | SMARTCoins    |  | Forge Platform  | |
  | |PostgreSQL|  | ATM           |  | (Cloudflare)    | |
  | |pgvector  |  | Token->Value  |  | D1, R2, KV,     | |
  | |Hyperledger| |               |  | Workers, Queues | |
  | +----------+  +---------------+  +-----------------+ |
  +-----------------------------------------------------+
```

### 8.2 Component Architecture

```
  +-----------------------------------------------------------+
  |                      CLIENTS                               |
  | +----------+ +----------+ +----------+ +----------+       |
  | | Web App  | | Mobile   | | Admin    | | Public   |       |
  | | (Builder)| | (PWA)    | | Dashboard| | Profiles |       |
  +------+------------+------------+------------+--------------+
         |            |            |            |
         +------------+------+-----+------------+
                             |
                    +--------v--------+
                    |   API Gateway   |
                    | (Rate Limiting, |
                    |  Auth, Routing) |
                    +--------+--------+
                             |
         +-------------------+-------------------+
         |                   |                   |
   +-----v-----+      +-----v-----+      +------v----+
   |  Mission   |      |  Builder  |      |Submission |
   |  Service   |      |  Service  |      |  Service  |
   +-----+------+      +-----+-----+      +-----+-----+
         |                    |                  |
         +--------------------+------------------+
                              |
                    +---------v---------+
                    |    Event Bus      |
                    | (Cloudflare       |
                    |  Queues)          |
                    +---------+---------+
                              |
         +----------+---------+---------+----------+
         |          |         |         |          |
   +-----v---+ +---v----+ +--v---+ +---v-----+ +--v--------+
   |Validation| |  XP    | |Audit | |Notif-   | |  REKORD   |
   | Engine   | | Engine | |Logger| |ication  | |  Sync     |
   +----------+ +--------+ +------+ +---------+ +-----------+
                              |
                +-------------v--------------+
                |        Data Layer          |
                | +--------+ +--------+      |
                | |  D1    | |   R2   |      |
                | |(SQLite)| | (Blob) |      |
                | +--------+ +--------+      |
                | +--------+ +--------+      |
                | |   KV   | | Queues |      |
                | |(Cache) | | (Jobs) |      |
                | +--------+ +--------+      |
                +----------------------------+
                              |
                    +---------v---------+
                    |  REKORD Layer 4   |
                    |  (PostgreSQL +    |
                    |   pgvector)       |
                    |  Phase 3+ sync    |
                    +-------------------+
```

---

## 9. Core Components

### 9.1 Mission Lifecycle

```
Draft --> Published --> Claimed --> Active --> Submitted
              |           |                      |
              v           v                 +----v----+
          Archived    Expired               | Review  |
                                            +----+----+
                                         +-------+-------+
                                         v       v       v
                                     Approved Rejected Revision
                                         |
                                         v
                                       Closed
```

### 9.2 Claim Rules (Server-Side)

```
canClaim(builder, mission):
  if builder.active_claims >= 3           -> reject "Max 3 active claims"
  if builder.rank < mission.required_rank -> reject "Rank too low"
  if builder.reputation < mission.min_rep -> reject "Reputation too low"
  if builder.track mismatch               -> reject "Track mismatch"
  if builder.cooldown_until > now()       -> reject "Cooldown active"
  if mission.max_claims_reached           -> reject "Mission full"
  -> allow
```

### 9.3 Role Matrix

| Action | Apprentice | Builder | Maker | Architect | Core | Admin |
|--------|-----------|---------|-------|-----------|------|-------|
| Claim starter | Y | Y | Y | Y | Y | Y |
| Claim standard | - | Y | Y | Y | Y | Y |
| Claim advanced | - | - | Y | Y | Y | Y |
| Claim elite | - | - | - | Y | Y | Y |
| Tier 1 review | - | Y | Y | Y | Y | Y |
| Tier 2 review | - | - | Y | Y | Y | Y |
| Propose missions | - | - | Y | Y | Y | Y |
| Project Lead eligible | - | - | - | Y | Y | Y |
| Tier 3 review | - | - | - | - | Y | Y |
| System admin | - | - | - | - | - | Y |

### 9.4 Validation Engine

```
TIER 1: Checklist (5-10 min)
  1 reviewer (Builder+ or Project Lead)
  Binary checklist: Y/N per deliverable item
  All Y = APPROVED | Any N = REJECTED with feedback
  SLA: 24 hours

TIER 2: Quality Review (15-30 min)
  2 reviewers (Maker+ or Project Lead)
  Random assignment, no self-selection
  Both approve = APPROVED
  Both reject = REJECTED
  Split = ESCALATE to Tier 3
  Timeout = reassign + flag reviewer
  SLA: 48 hours

TIER 3: Expert Review (30-60 min)
  1 reviewer (Architect+ / Core / Admin)
  Deep review with written feedback
  Can request 1 revision
  SLA: 72 hours
```

### 9.5 Project Lead System

Project Leads are Architect-rank builders who specialize in a GT3N project.

**Requirements:**

- Architect rank (8,000+ XP, 85+ reputation)
- 5+ approved contributions to the specific project
- Appointed by admin

**Permissions:**

- Create missions for their assigned project
- Validate Tier 1 and Tier 2 submissions for their project
- Cannot validate their own submissions
- Earn bonus XP for project lead duties

**Impact:** Each Project Lead removes approximately 80% of the founder's review load for that project.

### 9.6 Audit Log

Every state change emits an immutable event. Key events:

| Event | Target | Key Metadata |
|-------|--------|-------------|
| builder.registered | builder | provider, handle, track |
| builder.rank_changed | builder | from, to, xp_at_change |
| mission.created | mission | project_id, type, difficulty |
| mission.claimed | claim | mission_id, builder_id |
| submission.created | submission | output_hash, ai_score, project_id |
| review.completed | review | decision, tier |
| submission.approved | submission | xp_awarded, project_id |
| submission.rejected | submission | feedback_summary |
| xp.awarded | builder | amount, breakdown |
| badge.earned | builder | badge_id, category |
| contribution.recorded | contribution | output_hash, record_hash, chain_valid |
| rekord.synced | contribution | rekord_record_id |
| project_lead.assigned | project | builder_id, project_id |

---

## 10. Data Flow

### 10.1 End-to-End Flow

```
Builder opens Forge
       |
       v
[Project Selection] --> GET /v1/projects
       |
       v
[Mission Board] --> GET /v1/missions?project=gogsverse&track=vibe_coder
       |
       v
[Mission Detail] --> GET /v1/missions/:id
       |
       v
[Claim] --> POST /v1/missions/:id/claim --> canClaim() check
       |
       v
[Builder works -- uses their own AI tools, IDE, etc.]
       |
       v
[Submit] --> POST /v1/submissions
       |         |
       |   Pre-validation + Hash generation + R2 upload
       |         |
       |   Queue: VALIDATE --> Validation Engine (Tier 1/2/3)
       |
       v
[Dashboard: "In Review"]
       |
       v (on approval)
[XP Engine] --> Calculate XP + check rank up
[Audit Log] --> Record immutable event
[Contribution Record] --> Hash chain extended
[REKORD Sync Queue] --> Phase 3+ sync
[Notification] --> "Your submission was approved! +450 XP"
```

---

## 11. AI Integration Design

### 11.1 Bring Your Own AI (BYOAI)

```
Builder's Environment           GT3N Forge
+---------------------+   +------------------------+
|                     |   |                        |
| ChatGPT --------+  |   |  Submission Form       |
| Claude ---------+  |   |                        |
| Copilot --------+  |-->|  ai_disclosure: text   |
| Midjourney -----+  |   |  ai_tools_used: [...]  |
| Local LLM ------+  |   |  ai_percentage: 0-100  |
| No AI ----------+  |   |                        |
|                     |   |  (all tracked, none    |
| Builder controls    |   |   provided by Forge)   |
| their own tools     |   |                        |
+---------------------+   +------------------------+
```

AI is a tool, not the platform. Builders use whatever AI they want. Forge tracks what was used, not what should be used.

### 11.2 AI Disclosure Scoring

```
Score 1: "used AI"                                  -> FLAGGED
Score 2: "used Claude for code"                     -> FLAGGED
Score 3: "used Claude to draft the API routes"      -> ACCEPTABLE
Score 4: "used Claude to draft routes, manually
          wrote validation logic and tests"         -> GOOD
Score 5: "used Claude for SQL schema gen, manually
          optimized indexes, wrote all tests"       -> EXCELLENT
```

### 11.3 Centralized AI Layer (Future)

Optional GT3N-provided AI tools via Cloudflare AI Gateway in Phase 4+. BYOAI remains supported. Centralized layer would add automatic usage tracking and prompt analytics.

---

## 12. REKORD Integration

### 12.1 REKORD Overview

REKORD (Retrievable Expansive Knowledge Organized Repository Database) is GT3N's tamper-proof, AI-powered Knowledge-as-a-Service (KaaS) platform.

### 12.2 REKORD's Actual Tech Stack

| Component | Technology | Role |
|-----------|-----------|------|
| Knowledge Store | PostgreSQL + pgvector | Relational data + semantic embeddings |
| File Storage | Local disk / S3-ready | Original files |
| Integrity Layer | SHA-256 hashing + audit chain | Tamper-proof verification |
| Search Engine | Hybrid (semantic + full-text + structured) | RRF-fused search |
| API | FastAPI + RBAC | Application layer |
| Blockchain (future) | Hyperledger Fabric | Permissioned chain for institutional proof |

### 12.3 Where Forge Plugs Into REKORD

```
REKORD 8-Layer Stack:

  Layer 8:  MCP Bridge
  Layer 7:  Application API (FastAPI)
  Layer 6:  AI / Search Engine
  Layer 5:  Query Engine (RRF)
  Layer 4:  Knowledge Store (PostgreSQL + pgvector)  <-- Forge contributions stored
  Layer 3:  File Vault
  Layer 2:  Integrity Layer (SHA-256 + audit chain)  <-- Forge hashes anchor here
  Layer 1:  Hardware Security (Blackhole Drive)
```

### 12.4 Per-Builder Hash Chain

Every builder's contributions form a linked hash chain:

```
record_hash = SHA-256(output_hash + process_hash + disclosure_hash
              + builder_id + timestamp)
prev_record_hash = hash of builder's previous contribution

Contribution #1: record_hash = "a3f2b8...", prev = null
Contribution #2: record_hash = "7d1e4c...", prev = "a3f2b8..."
Contribution #3: record_hash = "9b5f2a...", prev = "7d1e4c..."
```

If any record is tampered with, the chain breaks. Verifiable without any blockchain.

### 12.5 Progressive Integration Phases

| Phase | Status | Description |
|-------|--------|-------------|
| Phase 1-2 | `local` | Hash chain in Forge D1. REKORD-compatible, not connected. |
| Phase 3 | `synced` | Contributions sync to REKORD PostgreSQL (Layer 4). |
| Phase 3 | `indexed` | Embedded + searchable in REKORD (Layer 6). |
| Phase 4+ | `anchored` | Merkle root on Hyperledger Fabric. |

---

# PART IV -- TECHNICAL SPECIFICATION

---

## 13. Data Model and Schema

### 13.1 Entity Overview

```
projects ----< missions ----< claims ----< submissions ----< submission_files
    |              |              |              |
    +----< project_leads         +----< reviews
    |                                    |
    +----< builder_projects              +----> contribution_records
                                                    |
builders ----< claims, submissions, reviews         +----> rekord_sync_queue
    |         builder_badges, builder_projects
    |         contribution_records, token_ledger
badges ----< builder_badges
audit_log (append-only, references all entities)
```

### 13.2 Projects

```sql
CREATE TABLE projects (
  id              TEXT PRIMARY KEY,
  name            TEXT UNIQUE NOT NULL,
  slug            TEXT UNIQUE NOT NULL,
  description     TEXT NOT NULL,
  vertical        TEXT NOT NULL,
  icon_url        TEXT,
  color           TEXT,
  status          TEXT NOT NULL DEFAULT 'active'
                  CHECK(status IN ('active','building','planned','paused')),
  is_client       INTEGER NOT NULL DEFAULT 0,
  mission_count   INTEGER NOT NULL DEFAULT 0,
  builder_count   INTEGER NOT NULL DEFAULT 0,
  created_at      TEXT NOT NULL DEFAULT (strftime('%Y-%m-%dT%H:%M:%SZ','now'))
);
```

### 13.3 Builders

```sql
CREATE TABLE builders (
  id                TEXT PRIMARY KEY,
  handle            TEXT UNIQUE NOT NULL,
  email             TEXT UNIQUE NOT NULL,
  provider          TEXT NOT NULL,
  provider_id       TEXT NOT NULL,
  avatar_url        TEXT,
  bio               TEXT,
  track             TEXT NOT NULL DEFAULT 'vibe_coder'
                    CHECK(track IN ('developer','vibe_coder')),
  primary_project_id TEXT REFERENCES projects(id),
  xp                INTEGER NOT NULL DEFAULT 0,
  rank              TEXT NOT NULL DEFAULT 'apprentice'
                    CHECK(rank IN ('apprentice','builder','maker',
                                   'architect','core_contributor')),
  reputation        REAL NOT NULL DEFAULT 100.0,
  streak            INTEGER NOT NULL DEFAULT 0,
  best_streak       INTEGER NOT NULL DEFAULT 0,
  active_claims     INTEGER NOT NULL DEFAULT 0,
  total_submissions INTEGER NOT NULL DEFAULT 0,
  total_approved    INTEGER NOT NULL DEFAULT 0,
  total_rejected    INTEGER NOT NULL DEFAULT 0,
  projects_contributed INTEGER NOT NULL DEFAULT 0,
  cooldown_until    TEXT,
  is_admin          INTEGER NOT NULL DEFAULT 0,
  is_project_lead   INTEGER NOT NULL DEFAULT 0,
  created_at        TEXT NOT NULL DEFAULT (strftime('%Y-%m-%dT%H:%M:%SZ','now')),
  updated_at        TEXT NOT NULL DEFAULT (strftime('%Y-%m-%dT%H:%M:%SZ','now'))
);
```

### 13.4 Missions

```sql
CREATE TABLE missions (
  id                TEXT PRIMARY KEY,
  project_id        TEXT NOT NULL REFERENCES projects(id),
  title             TEXT NOT NULL,
  description       TEXT NOT NULL,
  type              TEXT NOT NULL
                    CHECK(type IN ('code','design','content','research','ops')),
  difficulty        TEXT NOT NULL
                    CHECK(difficulty IN ('starter','standard','advanced','elite')),
  target_track      TEXT NOT NULL DEFAULT 'any'
                    CHECK(target_track IN ('developer','vibe_coder','any')),
  xp_reward         INTEGER NOT NULL,
  required_rank     TEXT NOT NULL DEFAULT 'apprentice',
  min_reputation    REAL NOT NULL DEFAULT 0,
  max_claims        INTEGER,
  claims_count      INTEGER NOT NULL DEFAULT 0,
  validation_method TEXT NOT NULL
                    CHECK(validation_method IN ('automated','peer',
                                                'core_team','project_lead')),
  status            TEXT NOT NULL DEFAULT 'draft'
                    CHECK(status IN ('draft','published','closed','archived')),
  deadline          TEXT,
  deliverables      TEXT NOT NULL DEFAULT '[]',
  context           TEXT,
  deployment_target TEXT,
  created_by        TEXT NOT NULL REFERENCES builders(id),
  created_at        TEXT NOT NULL DEFAULT (strftime('%Y-%m-%dT%H:%M:%SZ','now')),
  updated_at        TEXT NOT NULL DEFAULT (strftime('%Y-%m-%dT%H:%M:%SZ','now'))
);
```

### 13.5 Submissions

```sql
CREATE TABLE submissions (
  id                  TEXT PRIMARY KEY,
  mission_id          TEXT NOT NULL REFERENCES missions(id),
  project_id          TEXT NOT NULL REFERENCES projects(id),
  builder_id          TEXT NOT NULL REFERENCES builders(id),
  claim_id            TEXT NOT NULL REFERENCES claims(id),
  builder_track       TEXT NOT NULL,
  output_url          TEXT NOT NULL,
  process_notes       TEXT NOT NULL,
  process_notes_words INTEGER NOT NULL,
  ai_disclosure       TEXT NOT NULL,
  ai_disclosure_score INTEGER NOT NULL DEFAULT 0,
  ai_tools_used       TEXT NOT NULL DEFAULT '[]',
  ai_percentage       INTEGER,
  output_hash         TEXT NOT NULL,
  status              TEXT NOT NULL DEFAULT 'pending'
                      CHECK(status IN ('pending','in_review','approved','rejected',
                                       'revision_requested','escalated')),
  revision_count      INTEGER NOT NULL DEFAULT 0,
  xp_awarded          INTEGER,
  submitted_at        TEXT NOT NULL DEFAULT (strftime('%Y-%m-%dT%H:%M:%SZ','now')),
  reviewed_at         TEXT
);
```

### 13.6 Contribution Records (REKORD-Compatible, Immutable)

```sql
CREATE TABLE contribution_records (
  id                TEXT PRIMARY KEY,
  builder_id        TEXT NOT NULL REFERENCES builders(id),
  submission_id     TEXT NOT NULL REFERENCES submissions(id),
  mission_id        TEXT NOT NULL REFERENCES missions(id),
  project_id        TEXT NOT NULL REFERENCES projects(id),
  mission_type      TEXT NOT NULL,
  mission_difficulty TEXT NOT NULL,
  builder_track     TEXT NOT NULL,
  output_hash       TEXT NOT NULL,
  process_hash      TEXT NOT NULL,
  disclosure_hash   TEXT NOT NULL,
  record_hash       TEXT NOT NULL,
  prev_record_hash  TEXT,
  ai_tools_used     TEXT NOT NULL DEFAULT '[]',
  ai_percentage     INTEGER,
  xp_earned         INTEGER NOT NULL,
  rank_at_time      TEXT NOT NULL,
  rekord_sync_status TEXT NOT NULL DEFAULT 'local'
                     CHECK(rekord_sync_status IN
                       ('local','synced','indexed','anchored')),
  rekord_record_id  TEXT,
  rekord_synced_at  TEXT,
  rekord_anchor_tx  TEXT,
  rekord_anchored_at TEXT,
  verified          INTEGER NOT NULL DEFAULT 1,
  recorded_at       TEXT NOT NULL DEFAULT (strftime('%Y-%m-%dT%H:%M:%SZ','now'))
);
-- NO UPDATE OR DELETE ON THIS TABLE
```

### 13.7 Additional Tables

The complete schema also includes: claims, submission_files, reviews, badges, builder_badges, builder_projects, project_leads, audit_log, rekord_sync_queue, mission_proposals, and token_ledger (future). See the full schema in the separate Data Model document (03_GT3N_Forge_Data_Model.md).

### 13.8 Seed Data: Projects

| ID | Name | Slug | Vertical | Status |
|----|------|------|----------|--------|
| prj_gogs01 | GOGSverse | gogsverse | sports | active |
| prj_rekord | REKORD | rekord | verification | building |
| prj_smart1 | SMARTCoins ATM | smartcoins | finance | planned |
| prj_ark001 | ARK | ark | healthcare | planned |
| prj_hermes | HERMES | hermes | healthcare | planned |
| prj_pcasso | PICASSO | picasso | creative | planned |
| prj_forge1 | GT3N Forge | forge | platform | building |

---

## 14. API Specification

### 14.1 Design Decisions

| Decision | Choice | Rationale |
|----------|--------|-----------|
| Style | REST | Low complexity, HTTP caching, Cloudflare Workers native |
| Auth | JWT (15-min access + 7-day refresh) | Short-lived tokens, HttpOnly refresh cookie |
| Pagination | Cursor-based | Consistent performance at scale |
| Naming | snake_case | JSON convention |
| Timestamps | ISO 8601 | Universal standard |

### 14.2 Endpoint Summary

| Group | Method | Path | Auth |
|-------|--------|------|------|
| Auth | POST | /v1/auth/register | Public |
| Auth | POST | /v1/auth/login | Public |
| Auth | POST | /v1/auth/refresh | Cookie |
| Auth | POST | /v1/auth/logout | Bearer |
| Projects | GET | /v1/projects | Public |
| Missions | GET | /v1/missions | Public |
| Missions | GET | /v1/missions/:id | Public |
| Missions | POST | /v1/missions | Admin/Architect |
| Missions | POST | /v1/missions/:id/claim | Builder |
| Missions | DELETE | /v1/missions/:id/claim | Builder |
| Missions | POST | /v1/missions/propose | Maker+ |
| Submissions | POST | /v1/submissions | Builder |
| Submissions | GET | /v1/submissions/:id | Builder/Reviewer |
| Submissions | GET | /v1/submissions | Builder |
| Submissions | POST | /v1/submissions/:id/revise | Builder |
| Reviews | GET | /v1/reviews/queue | Builder+ |
| Reviews | POST | /v1/reviews/:id | Reviewer |
| Profile | GET | /v1/builders/:handle | Public |
| Profile | GET | /v1/builders/:handle/chain | Public |
| Profile | GET | /v1/builders/me/xp | Builder |
| Profile | GET | /v1/builders/me/badges | Builder |
| Leaderboard | GET | /v1/leaderboard | Public |

Full API specification with request/response examples is in the separate API document (04_GT3N_Forge_API_Spec.md).

---

## 15. Tech Stack

| Layer | Technology | Rationale |
|-------|-----------|-----------|
| **Frontend** | Next.js 15 + Tailwind + shadcn/ui | SSR for public profiles/SEO, fast iteration |
| **Backend API** | Hono on Cloudflare Workers | Type-safe, edge-native, matches existing infra |
| **Primary Database** | Cloudflare D1 (SQLite) | Zero config, scales to Phase 2-3 |
| **Scale Database** | Neon Postgres via Hyperdrive | Escape hatch when D1 hits limits |
| **File Storage** | Cloudflare R2 | Submission files, avatars |
| **Cache** | Cloudflare KV | Sessions, rate limits, leaderboard |
| **Queue** | Cloudflare Queues | Validation pipeline, XP calc, REKORD sync |
| **Auth** | Clerk | OAuth (GitHub, Google), JWT |
| **Email** | Resend | Transactional notifications |
| **Monitoring** | Cloudflare Analytics + Sentry | Errors, performance |
| **CI/CD** | GitHub Actions + Wrangler | Auto-deploy on merge |
| **REKORD Sync** | Forge Workers -> REKORD FastAPI | Phase 3+: D1 -> PostgreSQL |
| **Blockchain** | Hyperledger Fabric (via REKORD) | Phase 4+: batch anchoring |

---

## 16. Security Architecture

### 16.1 Authentication

- Clerk OAuth (GitHub, Google)
- JWT: 15-min access + 7-day refresh (HttpOnly cookie, rotation)
- Admin 2FA required

### 16.2 Rate Limiting

| Scope | Limit | Window |
|-------|-------|--------|
| Global API | 60 req | 1 min |
| Auth endpoints | 10 req | 1 min |
| Submissions | 5 | 24 hrs |
| Claims | 3 active | ongoing |
| File uploads | 50MB per sub | per req |
| Registration | 3 per IP | 24 hrs |

### 16.3 Data Integrity

- Audit log is append-only (no UPDATE/DELETE)
- Contribution records are immutable
- Per-builder hash chains break on tampering
- XP only increases via approved submissions
- Reputation recalculated from source data
- R2 files versioned (no overwrite)

---

# PART V -- EXECUTION

---

## 17. MVP Build Plan

### 17.1 Timeline

```
Week  1-2   | PHASE 1: No-Code OSS MVP (Codeberg + GitHub mirror + Sheets + Discord)
              All missions are open source (Apache 2.0 / CC-BY 4.0)
              No payments. Wall of Records is the recognition layer.

Week  3-6   | PHASE 2: First Custom Build (Next.js + Hono + D1)
              Still OSS-only. Custom platform, real data, automated flows.

Week  7-12  | PHASE 3: Scale Prep + REKORD Integration
              Wall of Records syncs to REKORD PostgreSQL.
              Still OSS-only. Founder bandwidth reduced via Project Leads.

Year 2+     | PHASE 4: Add Paid Contractor Missions
              OSS missions continue. Paid missions added for proprietary work.
              Funded by GT3N project revenue, grants, or sponsor-funded missions.

Year 3+     | PHASE 5: Token Economy via SMARTCoins ATM
              Subject to legal infrastructure and regulatory compliance.
              Retroactive token allocation to Wall of Records contributors.
              Founder Builders (Phase 1) get highest multiplier.
```

See the separate **Tokenization Roadmap document** for the public statement of intent regarding future phases.

### 17.2 Phase 1: No-Code OSS MVP (Weeks 1-2)

**Tools:** Codeberg (primary) + GitHub (public mirror) + Google Forms (submissions) + Google Sheets (XP) + Discord (notifications)  
**Users:** 5-15 invite-only Founder Builders  
**License Model:** Open Source ONLY (Apache 2.0 for code, CC-BY 4.0 for design/content/research)  
**Cost:** $0  
**Legal status:** Standard OSS contributor program (same model as Google, Meta, Vercel, Supabase)  
**Goal:** Prove the core loop works with real contributions before writing code

**Phase 1 Priority Projects:**

Phase 1 focuses on the GT3N projects with active build momentum. Other ecosystem projects (ARK, HERMES, PICASSO, SMARTCoins ATM) remain visible as "coming soon" and are added to the mission board as they progress from `planned` to `building` status.

| Project | Why Phase 1 Priority |
|---------|----------------------|
| **GOGSverse** | Active product with real users. UX research, profile design, feed mockups, Gen Z visual treatment, athlete onboarding flows. Builder output ships to real users. |
| **REKORD** | Active build with Campus Commons MVP. Pilot prep for Dr. Zimmer, KaaS explainers, librarian UX research, dissertation use case documentation. Builder output strengthens the pilot pitch. |
| **GT3N Forge** (self-build) | Meta-missions: mission board UI, builder profile design, brand assets, Forge documentation, gamified platform research. Builders help build the system they use. |

**Starter Missions (15 across 3 active projects):**

| Project | Missions | Types |
|---------|----------|-------|
| GOGSverse | 6-7 | design (profiles, feed), research (Gen Z UX), content (social posts), onboarding flow |
| REKORD | 4-5 | research (KaaS landscape, dissertation cases), content (explainers, pilot docs), design (librarian UX) |
| GT3N Forge | 4-5 | design (mission board UI, profiles), content (Forge explainer), research (gamified platforms), brand assets |

**Kill signals (stop and redesign if):**

- Less than 30% claim rate after 1 week
- Less than 50% of claims result in submission
- More than 50% of process notes are filler
- More than 30% abandon the form at AI disclosure
- More than 2 hours/day spent reviewing
- Less than 40% return for a second mission

### 17.3 Phase 2: First Custom Build (Weeks 3-6)

**Build:** Registration + profiles, project listing, mission board (by project), claiming, submissions (with hashing), admin review (Tier 1 + 3), XP/rank, contribution records, audit log, chain verification endpoint.

**Do NOT build:** Peer review (Tier 2), badges, leaderboard (use Sheet), notifications (use Discord), mission proposals, tokens, REKORD sync.

### 17.4 Phase 3: Scale Preparation (Weeks 7-12)

**Week 7-8:** Project Lead system + Tier 2 peer review  
**Week 9-10:** REKORD sync (D1 -> PostgreSQL Layer 4)  
**Week 11-12:** Badges, real-time leaderboard, notifications, mission proposals

### 17.5 Priority Matrix

```
BUILD FIRST (Phase 2):     Mission board + projects, submissions + hashing,
                           XP/rank + tracks, builder profiles

BUILD SECOND (Phase 3):    Peer review, Project Leads, badges, REKORD sync,
                           notifications, mission proposals

KEEP SIMPLE:               Leaderboard (Sheet embed), Discord for notifications

BUILD LATER (Phase 4+):    Token layer, Hyperledger anchoring, client projects,
                           mobile app, social features
```

---

## 18. Scalability Design

| Phase | Users | Architecture | Cost |
|-------|-------|-------------|------|
| Phase 1 | 5-15 | No-code (Notion + Sheets) | $0-50/mo |
| Phase 2 | 15-50 | Single Worker + D1 + R2 | $25-100/mo |
| Phase 3 | 50-500 | Split Workers + Queues + KV | $100-500/mo |
| Phase 4+ | 500-10K | Service mesh + Postgres via Hyperdrive | $500-2K/mo |

**What scales first:** Mission board queries, file uploads, leaderboard reads.  
**What doesn't need to scale early:** Badge calculation, mission creation, REKORD sync.

---

# PART VI -- RISK AND MITIGATION

---

## 19. Risk Analysis and Failure Modes

### 19.1 Risk Summary

| # | Risk | Likelihood | Impact | Mitigation |
|---|------|-----------|--------|-----------|
| 1 | Mission supply runs dry | Very High | Critical | Multi-project missions, Project Leads create missions (Phase 3) |
| 2 | Founder burns out on reviews | High | Critical | Tiered validation, Project Leads reduce load by 60% |
| 3 | Builders churn after 2-3 missions | High | High | Project variety, track system, corrected XP multipliers |
| 4 | Value prop weak for strangers | High | High | REKORD verification, focus on intrinsic motivation early |
| 5 | Peer review quality unreliable | Medium | High | Tiered system limits peer review to Tier 2 only |
| 6 | AI disclosure is theatrical | Medium | Medium | Structured tracking, pattern analysis over time |
| 7 | Economic layer causes split | Medium | High | Publish retroactive policy before Phase 4 |
| 8 | Project sprawl | High | Medium | Focus Phase 1 on 2-3 projects, expand as builders grow |
| 9 | Gamification rewards grinders | Medium | Medium | Multipliers 1x/2x/5x/10x prevent starter grinding |
| 10 | Sybil / collusion | Low | Medium | OAuth identity, IP throttling, pattern detection |

### 19.2 What NOT to Build Early

| Feature | Why It's a Trap |
|---------|----------------|
| Token economy | Legal complexity, zero users to reward |
| Blockchain proof | SHA-256 hash chain IS verifiable at this scale |
| Built-in AI tools | Builders already have their tools |
| Social features | Discord exists |
| Analytics dashboard | Cloudflare Analytics + spreadsheet is enough |
| Fancy onboarding | Notion doc beats a wizard at 15 users |
| API for third parties | Zero third parties exist |

### 19.3 The Two Things That Will Kill Forge

1. **Mission supply.** If builders log in and see nothing to do, they leave. Pre-load 16+ missions. Create 5-10 new ones per week. Enable Project Leads as soon as possible.

2. **Founder bandwidth.** If the founder spends all day reviewing submissions instead of building the platform and creating missions, everything stalls. Tiered validation and Project Leads are not optional features -- they are survival mechanisms.

Everything else is manageable if these two are solved.

---

**End of GT3N Forge Manual**

---

*This document consolidates the complete GT3N Forge design: concept, product design, systems architecture, technical specification, execution plan, and risk analysis. It represents the full pre-build reference for GT3N Forge v1.0.*

*Prepared by: GP Tenazas, Gwen (OpenAI), Claude (Anthropic)*  
*For: GT3N Industries*  
*Date: April 15, 2026*
