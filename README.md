# Vibecode Pro Skill

**A Reinventing.AI bonus skill for stronger Vibecode builds with Claude Code or OpenClaw.**

This repo gives Vibecode users a reusable skill they can install into the hosted Claude Code agent so it produces:
- better project briefs
- better build prompts
- better judgment on when to use `yolo` vs sandbox iteration
- better use of bonus skills for frontend polish and repeatable workflows

It is designed for builders using the Vibecode CLI from **OpenClaw** or **Claude Code** who want better output quality from the virtual container agent.

## Why this exists

A lot of Vibecode builds fail for a simple reason:

The agent gets a vague prompt.

This skill helps fix that.

It teaches the agent how to:
- turn a rough request into a compatible Vibecode project brief
- choose the right build workflow
- pass skill-install instructions into the hosted Claude Code environment when needed
- improve design quality with proven bonus skills
- create project-specific skills when a pattern should persist across builds

## Best use cases

Use this when you want Vibecode to build:
- premium landing pages
- polished SaaS marketing sites
- internal tools
- client apps
- micro-SaaS MVPs
- projects that need reusable styling, workflows, or domain context

## Included in this repo

```text
vibecode-pro/
├── SKILL.md
└── references/
    ├── brief-template.md
    └── installing-bonus-skills.md
```

## Install the skill

### 1) Clone this repo

```bash
git clone https://github.com/markfulton/reinventingai-vibecode-pro-skill.git
cd reinventingai-vibecode-pro-skill
```

### 2) Copy the skill into Claude Code skills

```bash
cp -r vibecode-pro ~/.claude/skills/
```

After that, the hosted Claude Code agent can use the skill when it sees relevant build requests.

## How to use it with Vibecode

Once installed, prompt your agent naturally, for example:

- "Use Vibecode Pro Skill to build a premium landing page for my SaaS"
- "Use Vibecode Pro Skill and install the frontend design skill before building"
- "Use Vibecode Pro Skill to create a strong project brief, iterate in sandbox first, and only deploy when approved"
- "Use Vibecode Pro Skill and create a reusable project-specific skill for this CRM workflow"

## Bonus skill support

This skill includes guidance for installing and leveraging bonus skills like:
- **Anthropic frontend-design**
- **Robonuggets cinematic-site-components**
- **skill-creator** for project-specific repeatable context

That means you can tell the agent not just what to build, but what extra capabilities to install before building.

## Recommended workflow

1. Install `vibecode-pro`
2. Ask OpenClaw or Claude Code to create the project brief
3. Tell it whether to use `yolo` or sandbox iteration
4. Tell it to install bonus skills if the build needs better design or reusable project context
5. Let Vibecode build from a stronger brief and richer environment

## Reinventing.AI training

Want the full workflow behind this skill?

See the training session landing page:

**https://agentappbuilder.reinventing.ai/**

## Vibecode referral link

If you need a Vibecode account, use this referral link:

**https://www.vibecodeapp.com/sign-up?code=ref-3ckyb6h3dwal**

## Who this helps most

This is especially useful for:
- founders who want higher-quality first-pass builds
- operators building internal tools
- agencies building faster client deliverables
- builders who want the hosted Claude Code agent to produce more polished work
- anyone who wants more leverage out of OpenClaw + Vibecode

## License

MIT
