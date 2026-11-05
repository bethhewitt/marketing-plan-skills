---
name: mp-icp
description: Step 4 of the marketing-plan framework. Defines the ideal customer / audience profile, covering segments, demographics, psychographics, jobs-to-be-done, pains, triggers, where they spend time, and personas, from the research pack and audience data. Works for B2C, B2B, media and creator audiences. Use for "ICP", "ideal customer profile", "target audience", "who are we for", "audience personas", "build personas", or when running the marketing-plan framework.
---

# Ideal customer profile (mp-icp)

Read `../marketing-plan/references/conventions.md` (the shared conventions file in the `marketing-plan` skill, a sibling of this skill's folder) first, then run its dependency check. This skill needs: 1. Section 3 (landscape & competitors) helps: use its platform and behaviour shifts for "where they spend time", and its competitors for "what they do today instead".

The ICP is not "everyone who buys today". It's the overlap between the people who are **most valuable to the brand** and the people who **get the most value from it**. This file is the single source for audience definitions. `mp-strategy` targets these segments and `mp-messaging` writes to these personas. Neither redefines them.

## Process

1. **Look at existing audience evidence** in the research pack and project: analytics demographics, existing persona files, comments and reviews, sponsor or customer lists, survey data. Separate **observed** (data) from **assumed** (opinion), and label which is which throughout.
2. **Draft 3–6 candidate segments.** Cut the audience along whichever lenses fit the offering. Use at least two:
   - Demographic or firmographic (age, life stage, location, income; or industry, size, role for B2B)
   - Behavioural (how they consume, buy, travel, use; frequency; channel)
   - Psychographic (values, aspirations, identity, attitudes)
   - Need-state or job-to-be-done (what they're trying to get done when they reach for an offering like this)
3. **Score the segments** in a table: value to the brand (revenue, sponsor appeal, advocacy), value from the brand (how well the offering serves the job), reachability (can we get in front of them with our channels and budget), and evidence strength. Recommend 1 primary and 1–2 secondary segments, and name who is explicitly **not** the target and why.
4. **Ask the user** to confirm the primary segment, then the secondaries, one question at a time.
5. **Profile each chosen segment** (structure below). Write the core problem as a narrative that describes their world back to them. When they read it, they should nod.
6. **Personas (where helpful).** Within each segment, define 1–3 personas when different people inside it care about meaningfully different things (e.g. listener vs sponsor's marketing lead; buyer vs user). The research can't supply personas' inner lives. Ask the user for what only they know, and flag anything that's assumed.

## Segment profile structure

```markdown
### {Segment name}: primary | secondary
**Who they are:** {demographic/firmographic, specific enough to target an ad or a sales list}
**Why they're a priority:** {value to the brand + value they get}
**Their world (core problem):** {narrative paragraph}
**Jobs to be done:** functional · emotional · social
**What they do today instead:** {alternatives and workarounds, including doing nothing, and why those fall short}
**Triggers:** {the moments that make them look for something like this}
**Barriers:** {what stops them choosing or staying}
**Where they spend time:** {platforms, publications, communities, events, people they trust}
**Language they use:** {real phrases from reviews, comments or research, quoted}
**Evidence:** {observed vs assumed}
```

## Persona structure

```markdown
#### {Persona name}: {role or one-line description}
**Day to day:** {what they actually do}
**Influence:** decision-maker | influencer | champion | user {and how much of the decision they control}
**What they care about:** operational | commercial | strategic | personal {what would make them look or feel good}
**Switching or joining trigger:** {the specific tipping point, not generic pain}
```

## Output: `04-icp.md`

Open with a one-line ICP summary and a segment scoring table. Then the primary segment profile, the secondaries, personas, "Who we are not for", and a list of `[Gap: ...]` flags where evidence is thin, with the research that would close each one.
