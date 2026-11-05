---
name: mp-objectives
description: Step 5 of the marketing-plan framework. Turns the business goal and mission into marketing objectives as OKRs organised across Brand (awareness), Land (new audience) and Expand (grow and deepen the current audience), with baselines and targets. Use for "marketing objectives", "set OKRs", "what should our goals be", "marketing goals for the quarter", or when running the marketing-plan framework.
---

# Objectives (mp-objectives)

Read `../marketing-plan/references/conventions.md` (the shared conventions file in the `marketing-plan` skill, a sibling of this skill's folder) first, then run its dependency check. This skill needs: 1, 2.

Objectives connect the business goal (`00-brief.md`) and the mission (`02-mission-vision.md`) to everything that follows. Strategy has to deliver them, and the Marketing Manager will measure against them. They are written as OKRs across three motions:

| Motion | Job | Typical key results |
|--------|-----|---------------------|
| **Brand** | Build awareness and meaning with people who don't know us yet | Reach, impressions, share of voice, branded search, press mentions, brand-recall survey |
| **Land** | Turn aware people into a new audience, customers or members | Follows, subscribers, sign-ups, first listens or purchases, conversion rate, cost per acquisition |
| **Expand** | Deepen and grow the people we already have | Retention, frequency, completion, repeat purchase, referrals, community participation, revenue per head, sponsor renewals |

## Process

1. **Start from the business goal.** State it as given in the brief. If it has no number, ask for one, or agree a directional goal and flag it as a gap.
2. **Set baselines.** Pull current numbers from the research pack's performance snapshot. Every key result needs a baseline or a `[Gap: baseline needed from {source}]`.
3. **Diagnose the bottleneck.** Look at the Brand → Land → Expand funnel numbers and say where the biggest leak or constraint is. That's where the weight of the objectives should go. Recommend the split (e.g. "60% Expand, because retention is the leak"), then confirm with the user.
4. **Draft 1 objective per motion,** or 2 for the priority motion and none for a motion that's deliberately parked. Say so if one is parked. Each objective:
   - **Objective:** qualitative and directional, one line. It should be inspiring but specific to this brand.
   - **Key results:** 2–4 per objective, each measurable: metric, baseline → target, by when.
   - **Why this matters:** one line linking it to the business goal or mission.
5. **Sense-check the targets.** For each key result, label it as committed (should hit) or stretch (70% would be good). Check it against the capacity and budget in the brief. Flag anything that needs resources the brief doesn't have.
6. **Confirm with the user** one objective at a time: wording, then targets.

## Rules

- Key results measure outcomes, not activity. "Publish 3 Reels a week" is a tactic, so it goes in the backlog. "Grow Instagram saves per post from 40 to 120" is a key result.
- No more than 4 objectives in total. Focus is the point.
- Every key result must be measurable with the tools the brand actually has. Name the source (e.g. Spotify for Podcasters, Instagram Insights, GA4).

## Output: `05-objectives.md`

```markdown
# Objectives
{header block}

## Business goal
{goal} · **Mission link:** {one line}

## Where the weight goes
{funnel diagnosis + split, 2–3 sentences}

## Brand: {objective}
Why: {line}
| Key result | Baseline | Target | By | Type | Source |

## Land: {objective}
...

## Expand: {objective}
...

## Not this period
{anything deliberately parked, and why}
```
