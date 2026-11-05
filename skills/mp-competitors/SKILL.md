---
name: mp-competitors
description: Step 3 of the marketing-plan framework. Sets out the market landscape (the shifts in the category, platforms and audience behaviour that shape the plan) and runs competitive intelligence for any brand, analysing how competitors and alternatives position themselves, what they emphasise, where they are heading, and where the whitespace is. Two modes, deep landscape and monitoring check-in. Use for "market landscape", "industry trends", "competitor analysis", "competitive landscape", "analyse [competitor]", "what are [competitor] doing", "whitespace analysis", "run CI on", "check on [competitor]", or when running the marketing-plan framework.
---

# Landscape & competitors (mp-competitors)

Read `../marketing-plan/references/conventions.md` (the shared conventions file in the `marketing-plan` skill, a sibling of this skill's folder) first, then run its dependency check. This skill needs: 1.

This section looks outside the brand, from wide to narrow: first the market it's in, then the competitors within it. Section 4 (ICP) comes after it and builds on both.

The competitor analysis is a positioning input, not a feature-comparison table or a battlecard. It answers four questions: how do competitors describe themselves, what do they emphasise, where are they heading, and what does that leave open for us?

## Two modes

- **Deep landscape** (the default inside the marketing plan): first-time mapping, positioning refresh, annual review. Covers the market landscape and several competitors together, and ends with whitespace and positioning implications. Writes `03-landscape-competitors.md`.
- **Monitoring:** a lighter check-in on one competitor, monthly or when something catches your eye. Writes `working/competitors/{competitor}-check-in-{date}.md`. It doesn't change the approved section unless the user asks.

Multiple competitors or "landscape" means deep mode. One competitor or "check on" means monitoring. If it's ambiguous, ask.

## Step 1: The market landscape (deep mode)

Start from the "Market and category" desk research in the research pack. Fill gaps with web search: category size and direction, audience behaviour, platform and channel shifts, format trends, and anything changing how people discover or choose offerings like this one.

1. Pick the **4–6 shifts that change a decision** for this brand. A trend that doesn't affect a channel, objective, audience or tactic doesn't make the cut, however interesting it is.
2. For each shift, give:
   - **What's happening:** one line, with one specific, sourced fact (source and date). Prefer national or category data to vendor claims; label vendor data as directional.
   - **What it means for us:** one line connecting it to the brand's own numbers or situation, and to the decision it points to.
3. Be honest where the market and the brand's experience disagree (e.g. a platform is growing nationally but hasn't worked for the brand yet). Say so, rather than letting the trend overrule the evidence.
4. Confirm the shortlist with the user before moving on to competitors.

## Step 2: Build the competitor set (deep mode)

Competition is whatever the audience would do instead. Propose a set across four types, using the research pack, the audience's alternatives described in the brief and research pack, and web search:

| Type | Example (podcast) | Example (B2B tool) |
|------|-------------------|--------------------|
| Direct: same offering, same audience | Other travel-interview podcasts | Like-for-like platforms |
| Indirect: different offering, same job | Travel magazines, YouTube travel creators | Agencies, consultants |
| Substitute: a DIY or manual alternative | Scrolling TikTok for destination ideas | Spreadsheets, in-house work |
| Status quo: doing nothing | Not listening; sticking with what they know | Not solving the problem |

Recommend 4–8 to analyse in depth: mostly direct, plus the most important indirect one or two. Confirm the set with the user (AskUserQuestion). Get URLs or handles for each.

## Step 3: Profile each competitor

Visit their website and main channels (homepage, about page, the main platform profiles; for media, the show page and episode titles too). Extract:

- **Who they say they're for:** the audience language, and whether the audience they actually seem to serve differs (the logos, guests, comments and case studies often tell a different story from the headline).
- **Value drivers:** the outcomes and benefits they lead with, functional vs emotional, and in what order.
- **Category and self-description:** their exact words ("platform" vs "tool"; "podcast" vs "show" vs "community"). Note any attempt to own a new category. Quote headlines and subheads verbatim.
- **Claimed differentiators:** substantive (exclusive access, unique format, proprietary data, talent) or generic ("best-in-class").
- **Proof points:** numbers, awards, notable names, testimonials, press, chart positions. The absence of proof is also a data point.
- **Notable elements:** voice and copy approach, format, content strategy, pricing or monetisation, calls to action that reveal their model.
- **Channel footprint:** where they're active, approximate audience size, posting cadence, the formats that seem to work for them.

## Step 4: Strategic intent

Search recent coverage: the past 12–24 months for deep mode, 3–6 months for monitoring. Adapt these queries to the sector:

```
"{name}" interview  ·  "{name}" funding OR investment OR acquisition
"{name}" launch OR new  ·  "{name}" partnership OR sponsor
"{name}" expansion  ·  "{name}" hiring OR jobs
"{name}" {sector trade press}
```

Extract their strategic direction, recent launches, shifts in positioning (upmarket, downmarket, new segments), what their hiring signals, and funding or growth signals. If you can't find signals, say so.

## Step 5: Competitive analysis (deep mode)

- **Positioning patterns:** the language, benefits and category claims that keep recurring. When everyone says it, it's noise.
- **Self-description table:** every competitor's category label, headline and the three claims they lead with, side by side. Mark which labels are contested, which are unclaimed, and what nobody is saying.
- **Differentiation map:** the axes they compete on (breadth vs depth, price vs premium, access vs expertise, entertainment vs utility). Mark which are crowded and which are open.
- **Whitespace:** underserved audiences, jobs, formats or messages. Whitespace isn't automatically opportunity. Note whether there's a reason nobody is there.
- **Positioning implications:** observations and questions for `mp-strategy`, framed as "given this landscape, the angles worth exploring are...". These are not recommendations yet.

## Output

Deep mode (`03-landscape-competitors.md`):

```markdown
# Landscape & competitors
{header block}
Competitors analysed: {list with type and URL}

## Market landscape
| What's happening | Evidence (source, date) | What it means for us |

## Competitors at a glance
{self-description table}

## Competitor profiles
### {Name} ({type})
**Who they're for** · **Core value proposition** · **How they describe themselves** · **Claimed differentiators** · **Proof points** · **Channel footprint** · **Strategic intent** · **Notable elements**

## Competitive analysis
### Common positioning patterns
### Differentiation map
### Whitespace and gaps
### Positioning implications

## Sources
```

Monitoring mode: Positioning snapshot · Strategic signals (what has changed) · Notable elements · So what? (observations for our positioning, not recommendations).

## Quality checks

1. **Specific, not general.** "They focus on luxury" is weak. "Their last 20 episodes feature 14 hotel GMs and the sponsor is a five-star group" is useful.
2. **Positioning lens, not feature list.** Features matter only as signals of positioning choices.
3. **Honest gaps.** Say what you couldn't find.
4. **Proportionate depth.** Monitoring is short. Deep mode is thorough but not bloated.
