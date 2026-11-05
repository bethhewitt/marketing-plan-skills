---
name: marketing-plan
description: Build a complete, hand-over-ready marketing plan / brand playbook for any brand, business, creator or offering by orchestrating eight specialist sub-skills (research, mission & vision, landscape & competitors, ICP, objectives, strategy & activation, messaging framework, tactics), then consistency-checking and compiling them into one playbook.md. Use when someone asks for a "marketing plan", "brand playbook", "go-to-market plan", "marketing strategy", "quarterly marketing plan", "campaign plan", wants to "refresh the marketing plan", or asks where a plan is up to. Also use to compile or check an existing plan folder.
---

# Marketing Plan (framework)

This skill is the conductor. It does not write strategy itself. It sets up the plan, runs the eight sub-skills in order, checks the sections agree with each other, and compiles a playbook: a tight summary of the plan that someone can read in one sitting and act on without having been in the room. The depth (research, evidence, reasoning) stays in the section files.

Read `references/conventions.md` (in this skill's folder) before doing anything. Every sub-skill follows it too.

## The plan

| # | Sub-skill | Output file | Needs |
|---|-----------|-------------|-------|
| 1 | `mp-research` | `00-brief.md`, `01-research-pack.md` | nothing |
| 2 | `mp-mission-vision` | `02-mission-vision.md` | 1 |
| 3 | `mp-competitors` | `03-landscape-competitors.md` | 1 |
| 4 | `mp-icp` | `04-icp.md` | 1 (3 helps) |
| 5 | `mp-objectives` | `05-objectives.md` | 1, 2 |
| 6 | `mp-strategy` | `06-strategy-activation.md` | 1, 3, 4, 5 |
| 7 | `mp-messaging` | `07-messaging-framework.md` | 3, 6 |
| 8 | `mp-tactics` | `08-tactics.md` | 3, 5, 6, 7 |

Every plan follows this order, outside in: the brand's own situation, why it exists, the market it's in, who it competes with, who it's for, then what it will achieve and how. The playbook keeps the same order, with section 3 split into "The landscape" and "Competitors".

The 90-day roadmap and backlog are **not** planned here; the playbook ends with next steps and leaves them to follow once the plan is signed off.

## Step 1: Locate or create the plan

1. Check the current project for `marketing-plan/`. If plan folders exist, list them with their status (from each `index.md`) and ask whether to continue one or start a new one.
2. For a new plan, ask for the plan name: a period (`2027-q1`) or campaign (`season-9-launch`). Recommend a period name if nothing suggests a campaign.
3. Create `marketing-plan/{plan-name}/index.md` from the status template in `references/conventions.md`.

## Step 2: Run the sub-skills

Run them in order, 1 to 8, invoking each with the Skill tool and passing the plan folder path as the argument. When these skills are installed as a plugin, their names carry the plugin prefix (for example `marketing-plan:mp-research`); use whichever form appears in the available skills list. After each one:

- Confirm the user approved the section (the sub-skill handles approval; check `index.md` shows it as `approved`).
- Give a one-line summary of what was decided and name the next skill.
- Let the user stop at any point. The plan resumes from `index.md` next time.

If the user wants to jump ahead or re-run a single section, allow it. The sub-skill does its own dependency check. When a section is re-run, mark every section that depends on it as `needs review` in `index.md` (use the "Needs" column above).

## Step 3: Consistency check

When all eight sections are `approved`, read them all and check:

| Check | Pass when |
|-------|-----------|
| Mission → objectives | Every objective plausibly advances the mission; nothing in the mission is unserved |
| Objectives → strategy | Each objective has a Brand, Land or Expand activation behind it |
| ICP → strategy | The targeted segments are the ICP segments, named the same way |
| Landscape → plan | Every market shift in 03 changes a decision somewhere (a channel, objective or tactic); none is contradicted by the plan |
| Competitors → positioning | The "unlike" framing and differentiators answer the competitors in 03; nothing claimed is something a competitor already owns more credibly |
| Positioning → messaging | Messaging pillars and differentiators express the chosen positioning route; the tagline would not fit a competitor |
| Messaging → tactics | Every content pillar traces to a value pillar or differentiator; every channel reaches a named ICP segment |
| Constraints | Nothing exceeds the budget, capacity or timeframe in `00-brief.md` |
| Gaps | All `[Gap: ...]` flags are listed |

Present the result as a table (check, status, issue, fix). Contradictions are put to the user one at a time with AskUserQuestion, recommended fix first. Fixing a contradiction means re-running or editing the relevant section, then rechecking.

Open gaps don't block compilation. The playbook's "What we still need" section lists only the 5–8 that most affect the plan; the full list stays in the section files.

## Step 4: Sign-off and compile

Ask for explicit sign-off. Then write `marketing-plan/{plan-name}/playbook.md` using the structure in `references/playbook-structure.md`. Update `index.md` to `compiled` with the date.

The playbook is a **tight summary of the plan, not an in-depth analysis**, and it reads as decided, not as a record of deciding. **Summarise each approved section down to its decisions and the direction they set**, following the template, length guide (3,000 to 4,500 words) and "What stays out of the playbook" list in `references/playbook-structure.md`. Keep the exact approved wording for the lines that matter (mission, vision, positioning statement, tagline, objectives, key results), and condense everything else. Leave out the research pack and all analysis, evidence, profiles, decision records and working material; they stay in the section files and `working/`, which remain the full record. Say each thing once. Run the checks at the end of the structure file before saving.

Finish by telling the user where the playbook is and listing the open gaps.
