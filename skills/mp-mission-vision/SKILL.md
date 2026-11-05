---
name: mp-mission-vision
description: Step 2 of the marketing-plan framework. Defines or sharpens a brand's mission, vision and the values or beliefs behind them, drafting options from the research pack and testing them before the user chooses. Use for "mission statement", "vision statement", "what's our purpose", "brand mission", "why do we exist", or when running the marketing-plan framework.
---

# Mission & vision (mp-mission-vision)

Read `../marketing-plan/references/conventions.md` (the shared conventions file in the `marketing-plan` skill, a sibling of this skill's folder) first, then run its dependency check. This skill needs: 1.

## Definitions (agree these before drafting)

- **Mission:** what the brand does, for whom, and why, today. It's present tense and operational. It guides what we do on a Tuesday.
- **Vision:** the future the brand is working towards if the mission succeeds. It's aspirational, but it should be specific enough to say no to things.
- **Beliefs / values (optional):** the 3–5 convictions behind both, expressed as behaviours, not adjectives ("We let guests finish the story", not "Authentic").

## Process

1. **Harvest.** Pull every existing mission, vision, purpose, bio or "about" line from the research pack and the project. Quote them. Note what they agree on.
2. **Decide: keep, sharpen or replace.** If an existing mission survives the tests below, recommend sharpening rather than replacing. Ask the user with AskUserQuestion.
3. **Draft options.** For the mission, write 3–4 options that span conservative to bold, using different angles:
   - Audience-led: "For {who}, we {do what} so that {change}."
   - Outcome-led: "We {change} by {how}."
   - Belief-led: "We believe {conviction}, so we {do what}."
   - Do the same for the vision: one option each for the audience's world changed, the category changed, and the brand's place in the world.
4. **Test each option** in a table:

| Test | Question |
|------|----------|
| Clear | Could a new team member repeat it after one reading? |
| True | Does the evidence in the research pack support it today (mission), or is it plausible (vision)? |
| Distinctive | Would it be wrong if a competitor from the research pack said it? |
| Useful | Does it help decide between two pieces of work? Name one thing it rules out. |
| Ambitious (vision only) | Is it bigger than the current plan period, but not fantasy? |

5. **Recommend.** Give one mission and one vision with a short rationale, then ask the user to choose or adjust, one question at a time (mission first, then vision, then beliefs).
6. **Mission into plan.** Write 2–3 sentences on what this mission means for this plan period. These sentences bridge into `mp-objectives`.

## Output: `02-mission-vision.md`

```markdown
# Mission & vision
{header block}

## Mission
{statement}
**What it rules out:** {one or two examples}

## Vision
{statement}

## What we believe {if included}
1. {belief as behaviour}: {one line on what this looks like in practice}

## What this means for {plan name}
{2–3 sentences}

## Options considered
{the tested options table, so the reasoning survives handover}
```

Avoid empty words ("inspire", "empower", "world-class", "passionate") unless the sentence would collapse without them.
