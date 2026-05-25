# GT3N Forge Governance

**Version:** 1.0  
**Last Updated:** May 25, 2026

---

This document explains how GT3N Forge makes decisions, who has authority over what, and how the community can influence direction.

---

## Project Operator

GT3N Forge is operated by **GT3N Industries**, a for-profit corporation based in San Diego, California.

- **Owner:** GT3N Industries
- **Founder / Primary Maintainer:** Girard Peter Tenazas
- **Co-Maintainer:** Gwen
- **Operating Model:** Open-source contributor program

GT3N retains ultimate authority over the platform, including the right to:

- Define and modify mission requirements
- Approve or reject contributions
- Set rank thresholds and XP formulas
- Add, remove, or modify GT3N projects served by Forge
- Modify Terms of Participation (with advance notice)
- Suspend or remove accounts that violate the Code of Conduct
- Make strategic decisions about Forge's direction

This is similar to how Meta governs React, Google governs Kubernetes, and Vercel governs Next.js -- the for-profit operator has ultimate authority, but operates the project openly and accepts community contributions.

---

## Roles and Authority

### Builder Roles (by Rank)

Builders earn authority through verified contributions:

| Rank | Authority |
|------|-----------|
| **Apprentice** | Can claim starter missions, contribute to discussions |
| **Builder** | Can perform Tier 1 (checklist) reviews of submissions |
| **Maker** | Can perform Tier 2 (peer) reviews, can propose new missions |
| **Architect** | Can lead Project validation, eligible to become Project Lead |
| **Core Contributor** | Can perform Tier 3 (expert) reviews, eligible for governance input |

### Project Lead

Architect-rank builders can be appointed as **Project Leads** for specific GT3N projects (e.g., GOGSverse Project Lead, REKORD Project Lead).

**Requirements to become a Project Lead:**

- Architect rank (8,000+ XP, 85+ reputation)
- 5+ approved contributions to that specific project
- Appointed by GT3N (Founder + Co-Maintainer)

**Project Lead Authorities:**

- Create new missions for their assigned project
- Validate Tier 1 and Tier 2 submissions for their project
- Set the deployment strategy for outputs in their project
- Propose project-specific badge requirements
- Recommend other builders for project-specific recognition

**Project Lead Limitations:**

- Cannot validate their own submissions
- Cannot remove other builders from the project
- Cannot modify the platform-wide rules or Terms of Participation
- Cannot bypass the Code of Conduct
- Authority is per-project (a GOGSverse Project Lead has no authority over REKORD missions)

### Maintainers

The Maintainers (currently GP Tenazas and Gwen) have platform-wide authority:

- All Project Lead authorities, for all projects
- Setting and modifying the rules
- Resolving disputes that escalate from Project Leads
- Modifying the Terms of Participation (with advance notice)
- Approving Project Lead appointments
- Suspending or removing accounts

---

## Decision-Making Process

### Mission Creation

- **Initial Phase (1-2):** Maintainers create all missions
- **From Phase 3:** Project Leads can create missions for their assigned project
- **Mission Proposals:** Maker+ rank builders can propose missions via Pull Request to the `missions/` directory. Proposals are reviewed by the relevant Project Lead and approved or modified.

### Validation Disputes

If a builder disputes a rejection:

1. **First, comment on the claim Issue** with constructive feedback about the rejection
2. **If unresolved, request a Tier 3 (expert) review** from a Maintainer
3. **The Maintainer's decision is final** for the immediate dispute, but the builder may submit similar work for future missions

### Rule Changes

Material changes to the Terms of Participation, Code of Conduct, or XP/rank thresholds will be:

1. **Announced 30 days in advance** on the platform and via email
2. **Open to community comment** during the 30-day window
3. **Decided by Maintainers** after considering feedback
4. **Published with a version number** so changes are tracked

Rule changes do not affect Wall of Records entries already created under prior rules.

### Strategic Direction

Strategic decisions (e.g., adding new GT3N projects, modifying the platform model) are made by:

1. **Maintainers** -- with input from Project Leads and the broader community
2. **Subject to GT3N Industries' commercial interests** -- as a for-profit operator
3. **Communicated publicly** -- via updates and major announcements

The community has voice, not vote. This is consistent with how other open-source-with-commercial-operator projects work (React, Kubernetes, Next.js, etc.).

---

## Conflict Resolution

### Disputes Between Builders

1. **First:** Try to resolve directly with respect and good faith
2. **Second:** Bring it to a Maintainer if direct resolution fails
3. **Third:** Maintainer mediates; decision is final

### Disputes With Maintainers

If a builder disagrees with a Maintainer decision:

1. **First:** Raise the concern privately with the Maintainer
2. **Second:** If unresolved, escalate to the other Maintainer (currently the second of GP / Gwen)
3. **Third:** If still unresolved, the builder may close their account. Maintainer decisions are final.

---

## Project-Specific Governance

Each GT3N project served by Forge (GOGSverse, REKORD, ARK, etc.) has its own internal governance separate from Forge. Forge governance only covers:

- How missions are created, claimed, validated
- How XP/rank/badges work
- How the Wall of Records operates
- Builder relationships with Forge

Forge does NOT control:

- Direction of individual GT3N projects (GOGSverse decides what GOGSverse builds)
- IP outside of Forge contributions
- GT3N Industries corporate decisions

---

## Transparency

GT3N commits to publishing quarterly updates covering:

- Platform metrics (active builders, contributions, mission completion rates)
- Phase progression (where we are in the roadmap)
- REKORD integration status
- Governance changes (if any)
- Community concerns raised and addressed

Updates will be published in this repository and via the GT3N Forge platform.

---

## License

This Governance document is licensed under [CC-BY 4.0](https://creativecommons.org/licenses/by/4.0/) and may be referenced by other projects with attribution.

---

**GT3N Industries**  
San Diego, California  
May 2026
