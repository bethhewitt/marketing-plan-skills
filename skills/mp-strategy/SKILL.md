---
name: mp-strategy
description: Step 6 of the marketing-plan framework. Sets marketing strategy through segmentation, targeting and positioning (five positioning questions, longlist, routes, objection test, positioning statement), then turns it into activation across Brand (awareness), Land (new audience) and Expand (grow current audience). Solo mode for small teams; team mode adds stakeholder alignment. Use for "positioning", "marketing strategy", "STP", "positioning statement", "how should we position", "brand land expand", "activation strategy", or when running the marketing-plan framework.
---

# Strategy & activation (mp-strategy)

Read `../marketing-plan/references/conventions.md` (the shared conventions file in the `marketing-plan` skill, a sibling of this skill's folder) and `references/positioning-toolkit.md` (in this skill's folder) first. Then run the dependency check. This skill needs: 1, 3, 4, 5.

Mode comes from `00-brief.md`: **solo** (the default) or **team**. Team-mode steps are marked **[team]**.

## Part A: Segmentation and targeting

Segmentation and audience profiles live in `04-icp.md`. Don't redefine them. Here you make the strategic choice:

1. Restate the ICP segments in a table: size or reach, value to the brand, how winnable they are given `03-landscape-competitors.md`, and which objective in `05-objectives.md` each one serves.
2. Recommend the targeting: which segment each motion (Brand, Land, Expand) aims at. Expand usually targets the existing audience. Land targets the segment most like the best existing audience. Brand can go wider.
3. Confirm with the user.

## Part B: Positioning

Positioning answers five questions, **in this order**. Order matters. Don't debate differentiation before the audience and the competition are settled.

1. **Who is it for?** (from targeting above)
2. **What is it?** The category: which box the audience puts us in, what they compare us to, and what "good" looks like before we've said a word.
3. **What does it compete against?** What they do if they don't choose us (from 03, including doing nothing).
4. **What value does it deliver?** Why anyone wants something like this at all. It doesn't need to be unique, but it must be clearly valuable.
5. **Why choose us?** Differentiation: true, compelling, provable, and hard for a competitor to claim with the same credibility.

### Steps

1. **Longlist.** Generate a broad longlist under each of the five slots, from conservative to bold, using the angles in the toolkit. Draw on the research pack, the ICP language and the competitor whitespace. Aim for range over quality (10–30 per slot). Save it to `working/positioning-longlist.md` with a parking lot for rejected ideas.
2. **Working document.** Answer the five questions one at a time. For each, give 2–4 options and a recommendation with its reasoning, and confirm with the user before moving to the next question.
   - **[team]** Settle questions 1–3 (audience, category, competition) in a group session first. Open by explaining what positioning is, so the room debates shared criteria rather than personal taste. Produce the session agenda and pre-read.
3. **Routes.** Using the agreed answers to 1–3, develop 3–4 distinct routes that vary value and differentiation. Label them as explorations. For each route, give:
   - Core idea, in one sentence
   - Positioning statement
   - What it implies for audience, competitive framing and value emphasis
   - 2–3 example messages
   - Risks
4. **Objection test.** Argue against each route bluntly. Which competitor could claim this with equal or greater credibility? Which part isn't provable today? Does it describe the category rather than take a point of view? What does choosing it cost us?
5. **Decide.** Show a comparison table and your recommendation, plus how to graft the best of the losing routes onto the winner. The user chooses.
   - **[team]** Take the decision one to one rather than by group vote. Produce a short brief per decision-maker. A useful test is showing a second decision-maker the headline statements blind.
6. **Final statement.** *For {target audience}, {brand} is a {category} that {primary value}. Unlike {competitive alternative}, {brand} {key differentiation}.* Run it against the four tests: clear, differentiated, credible, strategic.
7. **Pressure test (recommended action).** Write a short script for 3–5 audience members and 2–3 people who represent the brand. Don't ask whether they like it. Ask: Is it true? What does it mean (can they say it back)? Does it change how they think about us? What would they expect us to be able to do? For people representing the brand, also ask: Where would you use it, and what would you say next? Add it to the plan's next steps. It doesn't block approval.
   - **[team]** Add a socialisation plan: preview sessions with each stakeholder group before anything public changes.

## Part C: Activation (Brand / Land / Expand)

Turn positioning into how each motion will deliver its objective. For each motion:

| Field | Content |
|-------|---------|
| Objective | from `05-objectives.md` |
| Target | segment or persona from `04-icp.md` |
| The job of this motion | e.g. "be the name that comes to mind for {category}" |
| Strategic approach | the big idea for how we win, in 2–3 sentences, rooted in the positioning |
| What the audience should think, feel, do | before → after |
| Where we'll show up | channel types (owned, earned, shared, paid), not the tactics yet |
| Proof we'll lean on | from the positioning |
| Hand-offs | how this motion feeds the next (Brand → Land → Expand → advocacy → Brand) |

Close with the **flywheel**: one paragraph on how the three motions reinforce each other.

## Output: `06-strategy-activation.md`

```markdown
# Strategy & activation
{header block}

## Targeting
{table + recommendation}

## Positioning
### Positioning statement
### The five answers
{each with the chosen answer and one line of why}
### Routes considered
{comparison table; full routes stay in working/}
### Objection test outcome
### Pressure-test plan

## Activation
### Brand
### Land
### Expand
### The flywheel
```
