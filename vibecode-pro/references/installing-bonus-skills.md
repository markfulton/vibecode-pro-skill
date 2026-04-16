# Installing Bonus Skills in the Hosted Claude Code Agent

Use these patterns when the Vibecode build needs extra capability before coding starts.

## When to install bonus skills

Install extra skills when the project needs:
- premium UI polish
- better landing page composition
- repeatable domain-specific context
- richer design systems
- reusable operating rules across multiple prompts

## 1) Claude Code frontend-design skill

Use when:
- the user wants a more polished frontend
- the app needs stronger hierarchy and spacing
- the first pass needs to feel more premium

Install with:

```bash
# From the skills repo (recommended)
git clone https://github.com/anthropics/skills.git
cp -r skills/skills/frontend-design ~/.claude/skills/
```

Then instruct the agent:

> Use the frontend-design skill before building. Prioritize hierarchy, spacing, clarity, premium UI quality, responsive polish, and stronger visual consistency.

## 2) Cinematic site components skill

Use when:
- the user wants a cinematic landing page
- the brand needs more editorial or premium SaaS feel
- the page needs richer components or visual storytelling

Install with:

```bash
git clone https://github.com/robonuggets/cinematic-site-components.git
cd cinematic-site-components
```

If the hosted agent needs it inside `~/.claude/skills`, copy the relevant skill folder after cloning.

Then instruct the agent:

> Use the cinematic site components skill for premium page sections, richer composition, stronger visual storytelling, and high-end landing page polish.

## 3) skill-creator

This skill is already installed by default in many Claude Code environments.

Use it when:
- the project has repeatable rules
- the app will be refined across many prompts
- domain context should persist
- the same output format keeps coming up

Then instruct the agent:

> Use the skill-creator skill to create a project-specific skill for this app's recurring workflow, domain context, and output structure before continuing the build.

## How to pass this into the Vibecode build prompt

Add a short instruction block near the end of your build brief:

```text
Before building:
- install the frontend-design skill
- install any other required bonus skills
- create a project-specific skill if this app has repeated workflow or domain context
- then begin the build
```

## Notes

- Install only the skills that clearly help the project
- For client-facing premium work, prefer sandbox iteration after skill installation
- If a skill adds persistent value across many prompts, creating a project-specific skill is usually worth it
