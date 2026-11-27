# OfferHunter

[简体中文](README.md)

OfferHunter is an open-source Agent Skill for writing, reviewing, and tailoring resumes for AI-related roles. It covers research, engineering, infrastructure, data, evaluation, safety, product, design, governance, and customer-facing deployment.

## Write with STAR

- **Situation** — Identify the users, the problem, and the constraints.
- **Task** — State the goal and the part you owned.
- **Action** — Use short headings for key contributions. Describe what you did, how it worked, and the tradeoffs that mattered.
- **Result** — Attach verified outcomes to the relevant action. Attribute team outcomes to the team. When metrics are unavailable, describe a delivered capability, documented adoption, or a validated finding.

A project entry can open with **Context and goal**, then list **My contributions**, with outcomes attached where they can be attributed. For a one-page resume, compress those elements into a bullet.

## Install in Codex

Clone this repository, then run the commands below in the project where you want to use the skill. Replace the source path with your clone's path.

```sh
mkdir -p .agents/skills
cp -R /path/to/OfferHunter/skills/resume-engineering .agents/skills/
```

Invoke `$resume-engineering` with your resume, project notes, or a job description. For example, “Rewrite these two projects for an AI evaluation role. Keep the offline test scope and distinguish my work from the team's results.”

[English workflow](skills/resume-engineering/references/workflow.en.md) · [MIT License](LICENSE)
