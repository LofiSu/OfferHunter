# STAR workflow for AI resumes

1. Extract **Situation** (users, problem, constraints), **Task** (goal and personal ownership), **Action** (decisions, mechanisms, and tradeoffs), and **Result** (verified outcome, scope, and attribution). Use the supplied material as the source of truth. If the user supplies only a job description, ask up to three focused questions to gather relevant STAR material.
2. Choose and order projects by the work the target role actually does. Research and training may emphasize baselines and ablations. Application and platform roles may emphasize workflows, reliability, latency, or cost. Data, safety, and evaluation may emphasize dataset coverage, scoring criteria, and verified findings. Product, design, governance, and customer-facing roles may emphasize user research, acceptance criteria, adoption, or completed remediation.
3. Draft **Context and goal**, then **My contributions**. Start each contribution with a short heading and describe one decision or delivery. Explain the mechanism or workflow when it clarifies the contribution. Use ownership verbs that reflect the candidate's actual responsibility. For a short resume, combine context, action, and result in a single bullet.
4. Keep metrics tied to the known baseline, unit, measurement window, and environment. Distinguish offline evaluation, pilot outcomes, and production results. Attribute team results explicitly. Use qualitative evidence when a number is unavailable, and use causal wording only when the evidence supports it.
5. Deliver the copy-ready text first. Keep unresolved facts outside the resume and mention up to three only when they affect the wording. Remove confidential details from public-facing drafts.

## Example adapted from a real project

- **Situation** — Creators publishing across multiple platforms needed thumbnails in different sizes.
- **Task** — Build a tool that takes creator assets and a platform choice through to preview and download.
- **Action** — Build platform presets and subject and style-reference inputs in Next.js. Turn platform context and style keywords into prompts and integrate an image generation API.
- **Result** — The tool supports thumbnail generation and download in multiple platform sizes. Subscribers can generate in batches and export high-resolution images.

**AI Thumbnail Generator**

- **Context and goal** — Built a thumbnail generation workflow for creators publishing across multiple platforms, from selecting a platform size and submitting assets to generating a cover.
- **My contributions · Image generation** — Implemented platform presets, subject uploads, and style-reference inputs in Next.js. Combined platform context and style keywords into prompts and integrated an image generation API for previewing and downloading thumbnails in multiple sizes.
- **My contributions · Subscription features** — Built a free usage allowance and a paid subscription flow with batch generation and high-resolution export.

The source describes shipped capabilities and provides no measured change in click-through rate.

## Fictional practice example

Fictional notes — A support team piloted a knowledge assistant. The candidate selected 60 questions from historical tickets, grouped failures, and retested two versions. They also interviewed five agents and defined a citation-confirmation acceptance criterion. Engineers implemented the workflow. The team completed an internal pilot.

- **AI evaluation · Offline regression** — Curated 60 evaluation questions from historical support tickets, classified failures by citation errors, incomplete answers, and cases requiring refusal, and retested two assistant versions.
- **AI product · Workflow validation** — Interviewed five support agents and defined citation confirmation as an acceptance criterion for the assistant workflow. The team completed an internal pilot.
