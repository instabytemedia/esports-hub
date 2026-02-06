# 00 - Market Research

> **Agent:** Research Agent
> **Goal:** Gather real market data BEFORE building
> **Priority:** CRITICAL - Execute this phase FIRST

---

## Context

**Product:** Esports Hub
**Domain:** A blockchain-based social network for athletes, fans, and gamers
**Target Audience:** Esports and gaming communities, athletes, and fans
**Core Entities:** Idea, Crypto, Stadium

---

## Instructions for Claude Code

This document contains research tasks that YOU (Claude Code) should execute using WebSearch before proceeding with the build phases.

**Why do research first?**
1. Inform pricing decisions with real competitor data
2. Identify gaps in the market to exploit
3. Avoid building features competitors have proven don't work
4. Craft landing page copy that addresses real pain points

---

## Phase 0.1: Competitor Analysis

Use WebSearch to find competitors in the A blockchain-based social network for athletes, fans, and gamers space.

### Search Queries to Execute

```
best A blockchain-based social network for athletes, fans, and gamers apps 2024
```

```
A blockchain-based social network for athletes, fans, and gamers software alternatives comparison
```

```
top A blockchain-based social network for athletes, fans, and gamers tools for blockchain_social_network
```

```
A blockchain-based social network for athletes, fans, and gamers app reviews reddit
```

```
G2 A blockchain-based social network for athletes, fans, and gamers software comparison
```

### For Each Competitor Found (aim for 5-8)

Create a file `research/competitors/[name].md` with:

```markdown
# [Competitor Name]

## Overview
- **URL:**
- **Founded:**
- **Tagline:**

## Pricing
| Plan | Price | Key Features |
|------|-------|--------------|
| Free | $0 | ... |
| Pro | $X/mo | ... |
| Enterprise | Custom | ... |

## Key Features
1.
2.
3.

## Strengths (what users love)
-

## Weaknesses (common complaints)
-

## Our Opportunity
How Esports Hub can be better:
-
```

### Summary File

After researching competitors, create `research/competitor-summary.md`:

```markdown
# Competitor Summary for Esports Hub

## Market Leaders
1. [Name] - [Market position / USP]

## Pricing Landscape
| Competitor | Lowest | Mid | Highest |
|------------|--------|-----|---------|
| ... | ... | ... | ... |

## Feature Comparison Matrix
| Feature | Us | Comp 1 | Comp 2 | Comp 3 |
|---------|----|----|----|----|
| social_networking | Yes | ? | ? | ? |

## Gaps We Can Exploit
1.
2.
3.

## Recommended Positioning
[How should Esports Hub position itself?]
```

---

## Phase 0.2: Market Data

Research the market size and trends for A blockchain-based social network for athletes, fans, and gamers.

### Search Queries to Execute

```
A blockchain-based social network for athletes, fans, and gamers market size 2024 TAM
```

```
A blockchain-based social network for athletes, fans, and gamers industry growth rate CAGR
```

```
blockchain_social_network software market trends 2024 2025
```

```
A blockchain-based social network for athletes, fans, and gamers market report statistics
```

### Save to `research/market-data.md`

```markdown
# Market Data for Esports Hub

## Market Size
- **TAM (Total Addressable Market):** $X billion
  - Source: [URL]
- **SAM (Serviceable Addressable Market):** $X billion
- **SOM (Serviceable Obtainable Market):** $X million

## Growth
- **CAGR:** X%
- **Expected market size by 2028:** $X billion

## Key Trends
1. [Trend 1] - [What it means for Esports Hub]
2. [Trend 2] - [What it means for Esports Hub]
3. [Trend 3] - [What it means for Esports Hub]

## Target Segment
- **Primary:** Esports and gaming communities, athletes, and fans
- **Size:** X million potential users
- **Willingness to pay:** $X-$Y/month

## Sources
- [Source 1](URL)
- [Source 2](URL)
```

---

## Phase 0.3: Pricing Benchmark

Research competitor pricing in detail.

### Search Queries to Execute

```
blockchain_social_network software pricing comparison
```

```
blockchain_social_network SaaS pricing models
```

```
how much do blockchain_social_network tools cost
```

```
blockchain_social_network freemium vs paid conversion rates
```

### Save to `research/pricing-strategy.md`

```markdown
# Pricing Strategy for Esports Hub

## Competitor Pricing Analysis

| Competitor | Free Tier | Starter | Pro | Enterprise |
|------------|-----------|---------|-----|------------|
| ... | Yes/No | $X | $Y | Custom |

## Common Pricing Models
- [ ] Per user/seat
- [ ] Per project/workspace
- [ ] Usage-based (API calls, storage, etc.)
- [ ] Feature-based tiers
- [ ] Flat rate

## Pricing Sweet Spot
Based on competitor analysis:
- **Free tier:** [What to include]
- **Starter:** $X-Y/month (comparable to...)
- **Pro:** $X-Y/month (comparable to...)

## Recommended Pricing for Esports Hub

| Plan | Price | Rationale |
|------|-------|-----------|
| Free | $0 | [Why this limit?] |
| Starter | $X/mo | [Competitive with...] |
| Pro | $Y/mo | [Includes...] |

## Monetization Strategy
1. Primary revenue: [subscriptions / usage / one-time]
2. Upsell path: [Free → Starter → Pro]
3. Key conversion trigger: [What makes free users upgrade?]
```

---

## Phase 0.4: User Pain Points

Research what users hate about existing solutions.

### Search Queries to Execute

```
blockchain_social_network software frustrations reddit
```

```
blockchain_social_network app complaints reviews
```

```
what users hate about blockchain_social_network tools
```

```
blockchain_social_network software missing features
```

```
social_networking feature requests blockchain_social_network
```

### Save to `research/pain-points.md`

```markdown
# User Pain Points Analysis

## Top 10 Complaints About Existing A blockchain-based social network for athletes, fans, and gamers Tools

| # | Pain Point | Source | Severity | Esports Hub Solution |
|---|------------|--------|----------|------------------------|
| 1 | ... | Reddit/G2/etc | High/Med/Low | ... |
| 2 | ... | ... | ... | ... |

## Feature Requests Users Want
1. [Feature] - [How many mention it?]
2. ...

## Pricing Complaints
- [What users say about competitor pricing]

## UX Frustrations
- [Common UX complaints]

## Support Issues
- [Common support complaints]

## Our Differentiation Opportunities
Based on these pain points, Esports Hub should:
1. [Do this differently]
2. [Focus on this]
3. [Avoid this mistake]
```

---

## Validation Checklist

Before proceeding to `01-setup.md`, verify:

- [ ] 5+ competitors documented in `research/competitors/`
- [ ] `research/competitor-summary.md` created with comparison matrix
- [ ] `research/market-data.md` has TAM/SAM/SOM with sources
- [ ] `research/pricing-strategy.md` has recommended pricing
- [ ] `research/pain-points.md` has top 10 pain points

---

## Using Research in Later Phases

Reference these files in:
- **09-landing.md:** Use competitor positioning for copy
- **Pricing page:** Use pricing-strategy.md recommendations
- **Feature prioritization:** Address top pain points first
- **Marketing:** Reference market size for pitch decks

---

**Next Phase:** `docs/01-setup.md`
