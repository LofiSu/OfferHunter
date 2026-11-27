# OfferHunter

English | [简体中文](README.md)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

OfferHunter is an open-source Agent Skill that turns real project experience into STAR resumes for AI roles, in English or Chinese.

## One-Line Agent Setup

```text
Clone https://github.com/LofiSu/OfferHunter and install skills/resume-engineering into .agents/skills/ in my current Codex project.
```

## Quick Start

```sh
git clone https://github.com/LofiSu/OfferHunter.git /path/to/OfferHunter
mkdir -p .agents/skills
cp -R /path/to/OfferHunter/skills/resume-engineering .agents/skills/
```

Invoke `$resume-engineering` in that project with your resume or project notes and, if available, the target job description.

## Write with STAR

- **Situation** — Identify the users, the problem, and the constraints.
- **Task** — State the goal and the part you owned.
- **Action** — Use short headings for key contributions. Describe what you did, how it worked, and the tradeoffs that mattered.
- **Result** — Attach verified outcomes to the relevant action. Attribute team outcomes to the team. When metrics are unavailable, describe a delivered capability, documented adoption, or a validated finding.

A project entry can open with **Context and goal**, then list **My contributions**, with outcomes attached where they can be attributed. For a one-page resume, compress those elements into a bullet.

Use OfferHunter for research, training, applications, infrastructure, data, evaluation, safety, product, design, governance, and customer-facing deployment. The target role guides which experiences to highlight.

## Example

“Rewrite these two projects for an AI evaluation role. Keep the offline test scope and distinguish my work from the team's results.”

See how an AI thumbnail generator project becomes a copy-ready resume entry. [English STAR workflow and examples](skills/resume-engineering/references/workflow.en.md)

See the [EC-Monica e-commerce operations agent case study](skills/resume-engineering/references/workflow.en.md) for a full STAR breakdown and resume-ready entry.

## License

[MIT](LICENSE)
