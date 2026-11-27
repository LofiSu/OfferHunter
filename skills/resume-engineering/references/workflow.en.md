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

## Real project example · EC-Monica, an e-commerce operations agent

### STAR notes

- **Situation** — E-commerce product, operations, and engineering teams needed to analyze business data, draft reports, interpret requirements, and investigate changes in business metrics.
- **Task** — Own the project from initial design through launch and build an agent for those workflows.
- **Action** — Route requests by intent to tool execution or direct generation. Select tools from a registry, calculate year-over-year and period-over-period changes, and inject the results into context. Generate intermediate findings and synthesize them into a report. Handle tool timeouts and errors with retries and a fallback path. Use sample reports and operations templates as few-shot examples, and manage multi-turn context with summaries and a sliding window.
- **Result** — Shipped to product, operations, and engineering teams with support for analysis reports, requirements interpretation, and business attribution. Include measurement scope and comparison conditions when reporting quantitative outcomes.

### Resume-ready entry

**EC-Monica · E-commerce Operations Agent | Project Owner**

- **Context and goal** — Designed and launched an agent for e-commerce product, operations, and engineering teams, covering data analysis, report generation, requirements interpretation, and business attribution.
- **Agent workflow** — Implemented intent routing and registry-based tool selection. Injected year-over-year and period-over-period calculations into context, generated intermediate findings, and synthesized them into reports. Added retry, error classification, and fallback handling for tool calls.
- **Context engineering** — Added business reports and operations templates as few-shot examples. Used summaries and a sliding window to carry forward observations and findings during multi-step analysis.
- **Launch** — Delivered report generation, requirements interpretation, and attribution workflows to product, operations, and engineering users.

For AI application engineering, lead with routing, failure handling, and context management. For AI product roles, lead with users, the workflows delivered, and verified usage evidence.
