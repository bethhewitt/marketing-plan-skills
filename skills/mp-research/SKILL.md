---
name: mp-research
description: Step 1 of the marketing-plan framework. Sets up a marketing plan's brief (scope, timeframe, owner, budget, capacity, constraints, decision-makers) and builds a research pack from existing materials, audience data, performance data and desk research, which every later section reads first. Use when starting a marketing plan, "kick off the marketing plan", "planning and research", "build the research pack", "audit our existing marketing materials", or when the research pack needs refreshing.
---

# Planning & research (mp-research)

Read `../marketing-plan/references/conventions.md` (the shared conventions file in the `marketing-plan` skill, a sibling of this skill's folder) first.

This skill produces two files. `00-brief.md` sets the rules of play. `01-research-pack.md` is the evidence base. Every later skill reads both first, so the more that's settled here, the less anyone gets asked twice. Spend the effort here.

## Part A: The brief

Start by reading the project (CLAUDE.md, README, any brand/knowledge folders) so you can pre-fill what's already known. Then confirm or ask for the rest, one question at a time:

1. **Offering:** what is being marketed, in one or two sentences. What kind of thing it is (product, service, media brand, creator, venue, etc.).
2. **Plan scope:** the whole brand, or a campaign or launch within it.
3. **Timeframe:** the period the plan covers. Any fixed dates inside it (launches, events, seasons, deadlines).
4. **Business goal:** what the business needs marketing to deliver (revenue, sponsorship income, audience size, bookings, donations). Ask for the real number if there is one.
5. **Who decides:** who signs the plan off, who has a veto, who must be consulted, and who just needs to be informed. Who the Marketing Manager picking it up will be, if known.
6. **Mode:** **solo** (one or two decision-makers; Claude does the legwork and the user decides) or **team** (several stakeholders to interview and align). Recommend solo unless three or more people must be consulted. Mode carries through to `mp-strategy`.
7. **Resources:** budget (or "none / organic only"), team and capacity (hours per week, skills, tools), and existing channels and assets.
8. **Constraints:** brand rules, legal or sector rules, things that are off-limits, previous commitments.
9. **What's been tried:** previous plans or positioning attempts, what they landed on, and why they did or didn't stick.

Save `00-brief.md`:

```markdown
# Brief
{header block}

## The offering
## Plan scope and timeframe
| Date | What | Why it matters |
## Business goal
## Decision-making
| Role | Name | Sign-off / Veto / Consult / Inform |
Mode: solo | team
## Resources
Budget · Team & capacity · Channels and assets we already have
## Constraints
## What's been tried before
## Success for this plan
{what the plan owner said would make this a success}
```

## Part B: The research pack

### 1. Existing-materials audit

Collect everything that already exists. Search the project first; ask only for what you can't find:

- Previous marketing plans, positioning or messaging documents, however old
- Brand guidelines and tone of voice
- Website copy (homepage and the top 2–3 pages), bios, about pages
- Pitch decks, sponsor or sales decks, media kits
- Strategy documents, annual plans, OKRs
- Audience research, surveys, reviews, comments, testimonials, NPS verbatims, win/loss notes
- Analytics: follower and audience numbers, reach, engagement, downloads, traffic, conversion, email list size, growth over time
- The job description for the last marketing hire (it shows where leadership thinks the gap is)

Then analyse what you've gathered:

- What position does each document claim, in its own words? Quote it.
- Where do they contradict each other or emphasise different things? Don't smooth over inconsistencies. They're the point.
- What claims appear in internal documents but never reach customer-facing ones, or the other way round?
- What category label is used for the offering, and is it used consistently?
- What did the last attempt land on, and why didn't it stick? Most of the time it failed for a reason that's still true today. Name it.

### 2. Audience and performance snapshot

Summarise the numbers you have: who the audience is now, how it's grown, which channels and content perform best and worst. Use tables. Mark every estimate as an estimate.

### 3. Market and category desk research

Use web search. Cover the category's size and direction, audience behaviour trends, platform and channel shifts that affect this category, and seasonal patterns. Cite every source with its URL and date. Keep this to the signals that matter for decisions. Don't write an essay. `mp-competitors` turns these into the plan's market landscape (section 3).

### 4. Stakeholder discovery (team mode only)

Produce an interview guide for 5–15 one-to-ones across the people listed in the brief. Use the same core set for everyone so answers can be compared:

- **Opening:** What do you do here? Give me the five-minute pitch for {offering}.
- **The two that matter most:** What makes us different from the alternatives? Why do people actually choose us: not why we think they should, but why they currently do?
- **Audience and market:** Describe our best-fit customer or audience member. Who do we serve badly? When we lose someone, what do we lose them to, including "nothing"?
- **Value:** What surprises people about us? What do they value a year in, compared with what got them through the door?
- **Story and alignment:** If five people here explained our value, how similar would the answers be? What do we say about ourselves that isn't quite true? What's the truth nobody wants to say out loud? What happened the last time someone tried to fix this?
- **Closing:** What would make this plan a success for you? Who else should I speak to?

When the notes come back, save them to `working/interviews/` and synthesise them into the pack. Cover the 3–5 recurring themes and who said what, every distinct answer to "what makes us different" grouped by idea and how consistent it is, direct contradictions, and what nobody mentioned. Quote people where their phrasing is telling.

### 5. Diagnosis

Close the pack with a playback that creates agreement on the problem before anyone backs a solution. It contains no recommendations.

Save `01-research-pack.md`:

```markdown
# Research pack
{header block}

## Evidence base
{what was reviewed, with links/paths; what was asked for but not available}
## Existing materials audit
### What we currently say (quoted, by source)
### Contradictions and gaps
### Why previous attempts didn't land
## Audience and performance snapshot
## Market and category
## Stakeholder discovery {team mode only}
## Diagnosis
### Current state
### Core tensions to resolve {named as tensions, not problems}
### Challenges and opportunities
### Emerging hypotheses {labelled as hypotheses}
### What's still missing
```

Get approval on each file separately (brief first), save both, then update `index.md`.
