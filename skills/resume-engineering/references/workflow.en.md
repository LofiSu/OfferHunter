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

### How the resume entry evolved

The earliest draft introduced A/B experiments, dashboards, and requirements documents under business context, then established end-to-end ownership. Later versions split the implementation into the agent workflow, tool registry, and context engineering. The current resume puts adoption and report turnaround before the technical details.

### STAR notes

- **Situation** — E-commerce product, operations, and engineering teams needed to interpret experiments and dashboards, write reports, investigate metric changes, and analyze requirements.
- **Task** — Own EC-Monica from initial design through launch.
- **Action** — Route requests by intent, register tools through configuration, calculate year-over-year and period-over-period metrics in Python, and synthesize intermediate findings into reports. Add tool failure handling and use examples, summaries, and a sliding window to guide multi-turn analysis.
- **Result** — The resume records 600+ calls per month on average. About 55% were reporting tasks and 45% were requirements or attribution tasks. A single report took 1–2 hours to write manually and 5–15 minutes to generate with the agent. The source does not specify the observation period or sample size.

### Resume-ready entry

**EC-Monica · E-commerce Operations Agent**

- **Business context** — Built an agent for e-commerce product, operations, and engineering teams to analyze A/B experiments and dashboards, produce reports, investigate metric changes, and interpret requirements.
- **Adoption and impact** — Averaged 600+ calls per month after launch. About 55% were reporting tasks and 45% were requirements or attribution tasks. A single report took 1–2 hours to write manually and 5–15 minutes to generate with the agent.
- **My contributions** — Owned the project from design through launch.
  - **Agentic workflow** — Routed requests by intent to tool calls or direct generation. Executed tools iteratively, produced intermediate findings, and synthesized reports. Added timeouts, retries, error classification, and a direct-generation fallback.
  - **Tool registry** — Registered function schemas through configuration across user behavior, GMV, acquisition channels, and product analysis. Added analysis tools by extending the configuration.
  - **Context engineering** — Calculated year-over-year and period-over-period metrics in Python, added report examples and operations templates, and carried forward key findings with summaries and a sliding window.

For AI application engineering, retain the three implementation headings. For AI product roles, lead with users, task mix, and report turnaround, and compress the implementation into one bullet.
