# Marketing plan conventions

Every `mp-*` sub-skill and the `marketing-plan` framework follow these rules.

## Generic language

These skills work for any offering: a product, a service, a media brand or podcast, a creator, a venue, a charity. Use "offering" for the thing being marketed and "audience" for the people it's for. Use "customer", "listener", "member" or "client" only once the brief tells you which applies. Never assume B2B SaaS. A podcast's "competitors" include other shows, other media and the listener's other uses of that hour. A charity's "conversion" might be a donation or a volunteer sign-up.

## Plan folder

All files live in `marketing-plan/{plan-name}/` in the current project. If the project's CLAUDE.md or README defines conventions (voice rules, banned punctuation, filename style, where drafts go), those win over anything here.

```
marketing-plan/{plan-name}/
  index.md                      status tracker
  00-brief.md                   mp-research
  01-research-pack.md           mp-research
  02-mission-vision.md          mp-mission-vision
  03-landscape-competitors.md   mp-competitors
  04-icp.md                     mp-icp
  05-objectives.md              mp-objectives
  06-strategy-activation.md     mp-strategy
  07-messaging-framework.md     mp-messaging
  08-tactics.md                 mp-tactics
  working/                      longlists, interview notes, monitoring check-ins, parked ideas
  playbook.md                   compiled by marketing-plan
```

Plans created before October 2026 may use the older numbering (`03-icp.md`, `04-competitor-analysis.md`, no landscape). Keep their files as they are; the compiled playbook still follows the current order.

If a sub-skill is invoked with no plan folder given, look for `marketing-plan/*/index.md`. If there's one, use it. If there are several, ask which one. If there are none, offer to run `marketing-plan` to set one up.

## index.md template

```markdown
# Marketing plan: {plan name}

Brand / offering: {name}
Plan owner: {name}
Created: {date}
Status: in progress | ready to compile | compiled

| # | Section | File | Status | Updated | Notes |
|---|---------|------|--------|---------|-------|
| 1 | Brief & research pack | 00-brief.md, 01-research-pack.md | not started | | |
| 2 | Mission & vision | 02-mission-vision.md | not started | | |
| 3 | Landscape & competitors | 03-landscape-competitors.md | not started | | |
| 4 | ICP | 04-icp.md | not started | | |
| 5 | Objectives | 05-objectives.md | not started | | |
| 6 | Strategy & activation | 06-strategy-activation.md | not started | | |
| 7 | Messaging framework | 07-messaging-framework.md | not started | | |
| 8 | Tactics | 08-tactics.md | not started | | |
```

Status values: `not started`, `draft`, `approved`, `needs review` (an upstream section changed).

## Dependency check (start of every sub-skill)

1. Read `index.md`, `00-brief.md` and `01-research-pack.md`. These are always read first.
2. Check that the sections this skill needs (see the "Needs" column in the framework's table) are `approved`.
3. If a needed section is missing or still a draft, say which one and use AskUserQuestion to offer: run it first (recommended), proceed anyway and flag the assumption, or stop.
4. Never re-ask anything that's already answered in the brief, the research pack or an approved section.

## Interviewing

- Draft from evidence first. Only ask about genuine decisions and missing facts.
- Facts you can look up (files, websites, web search) are your job, not the user's.
- Ask one question at a time with AskUserQuestion. Give 2–4 concrete options, put the recommendation first with "(Recommended)" in its label, and explain the reasoning in each description.
- Present options with a steer: "strong opinions, loosely held".

## Writing standards

- Be specific over clever. Every claim should be traceable to the research pack, a source or a user decision.
- Flag gaps honestly rather than papering over them: `[Gap: what is missing and what would close it]`.
- Write in the brand's voice where the output is customer-facing (messaging, campaign lines). Read the project's tone-of-voice or brand guidelines file if one exists.
- Use British English unless the brand is American.
- Write it to be used, not admired: no meta-commentary or filler. Every section should earn its place.
- Write for a reader who wasn't in the room. Someone new should be able to act on it.

## Approval and saving

1. Show the draft section to the user.
2. Revise until they approve.
3. Save the file with a header block:

```markdown
# {Section title}
Plan: {plan name} · Version: v{n} · Status: approved · Updated: {date}
Inputs: {files and sources this section drew on}
```

4. Update the section's row in `index.md`. If this was a re-run of an approved section, set every downstream dependant to `needs review`.

**Decision records vs the plan.** Section files are the audit trail, so they can hold the reasoning (options considered, scoring, routes, objection tests, implications for later sections). Put that reasoning under its own clearly named headings, after the decided content, so the compiled playbook can leave it out cleanly. Write the decided content itself as the plan ("The mission is…"), not as a record of choosing ("We chose M3b because…"). See "What stays out of the playbook" in `playbook-structure.md`.
