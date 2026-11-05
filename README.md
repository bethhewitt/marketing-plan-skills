# Marketing Plan skills for Claude

Nine Claude skills that take a brand from a blank page to a signed-off marketing playbook. They work for any offering: a product, a service, a podcast or media brand, a creator, a venue or a charity.

One orchestrator skill, `marketing-plan`, runs eight specialist steps in order. It then checks that the sections agree with each other and compiles everything into a single `playbook.md` that someone new can read in one sitting and act on.

| # | Skill | What it produces |
|---|-------|------------------|
| 1 | `mp-research` | The brief and a research pack built from your existing materials, data and desk research |
| 2 | `mp-mission-vision` | Mission, vision and beliefs, tested before you choose |
| 3 | `mp-competitors` | The market landscape and a positioning-focused competitor analysis |
| 4 | `mp-icp` | Ideal customer or audience segments and personas |
| 5 | `mp-objectives` | OKRs across Brand, Land and Expand, with baselines and targets |
| 6 | `mp-strategy` | Targeting, positioning statement and activation plan |
| 7 | `mp-messaging` | A messaging framework: tagline, value pillars, differentiators, campaign lines |
| 8 | `mp-tactics` | Content pillars, channel roles, a pillar × channel matrix and activity tiers |

Every step drafts from evidence first, asks you one question at a time, and saves its section only after you approve it. Plans live in `marketing-plan/{plan-name}/` inside your project, so you can stop and resume at any point.

## Install (Claude Code)

```
/plugin marketplace add bethhewitt/marketing-plan-skills
/plugin install marketing-plan@norso
```

Then ask Claude for a marketing plan, or run a single step directly, for example "run a competitor analysis" or "build our ICP".

To update later:

```
/plugin marketplace update norso
```

## Install without the plugin system

Copy the folders inside `skills/` into `~/.claude/skills/` (for you, across all projects) or into `.claude/skills/` in a project. Keep all nine together: the step skills read shared conventions from the `marketing-plan` folder.

For claude.ai or the Claude desktop app's chat, zip each skill folder and upload it under Settings → Capabilities → Skills.

## Repository layout

```
.claude-plugin/
  plugin.json          plugin metadata
  marketplace.json     lets this repo be added as a marketplace
skills/
  marketing-plan/      orchestrator + shared conventions and playbook template
  mp-*/                the eight step skills
```

## Credits

Created by Norso Creative. Released under the [MIT licence](LICENSE).
