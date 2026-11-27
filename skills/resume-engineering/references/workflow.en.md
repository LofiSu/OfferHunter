# STAR workflow for AI resumes

Apply STAR to every project, including work, internships, open-source contributions, and independent projects. Use four separate labeled bullets per project, in STAR order.

1. Extract **Background** (users, problem, constraints), **My responsibilities** (goal and personal ownership), **Action** (decisions, mechanisms, and tradeoffs), and **Result** (verified outcome, scope, and attribution). Use the supplied material as the source of truth. If the user supplies only a job description, ask up to three focused questions to gather relevant STAR material.
2. Choose and order projects by the work the target role actually does. Research and training may emphasize baselines and ablations. Application and platform roles may emphasize workflows, reliability, latency, or cost. Data, safety, and evaluation may emphasize dataset coverage, scoring criteria, and verified findings. Product, design, governance, and customer-facing roles may emphasize user research, acceptance criteria, adoption, or completed remediation.
3. Draft four separate lines labeled **Background**, **My responsibilities**, **Action**, and **Result**. Use the action line to explain the candidate’s most important decision or contribution. Shorten individual lines for a one-page resume.
4. Keep metrics tied to the known baseline, unit, measurement window, and environment. Distinguish offline evaluation, pilot outcomes, and production results. Attribute team results explicitly. Use qualitative evidence when a number is unavailable, and use causal wording only when the evidence supports it.
5. Deliver the copy-ready text first. Keep unresolved facts outside the resume and mention up to three only when they affect the wording. Remove confidential details from public-facing drafts.

## EC-Monica · E-commerce Operations Agent

- **Background** — E-commerce product, operations, and engineering teams needed to query business data, investigate metric changes, and prepare reports.
- **My responsibilities** — Owned the project from design through launch, including tool orchestration and model context.
- **Action** — Routed each request to direct generation or a tool. For data queries, calculated year-over-year and period-over-period changes, then combined intermediate findings into a report. Added timeouts, retries, and fallback handling. Used sample reports to guide formatting and summaries with a sliding window to retain relevant context.
- **Result** — Averaged 600+ calls per month after launch. About 55% were reporting tasks and 45% were requirements or attribution tasks. One report took 1–2 hours to write manually and 5–15 minutes to generate with the agent.

## AI Thumbnail Generator

- **Background** — Creators publishing across platforms needed thumbnails in different sizes.
- **My responsibilities** — Owned the project, including the frontend, payments and subscriptions, and the workflow from asset upload to image generation.
- **Action** — Implemented platform size presets and subject and style inputs in Next.js. Integrated an image generation API with platform and style prompts, and built free usage and subscription flows.
- **Result** — Shipped thumbnail generation, preview, and download for multiple platforms, with batch generation and high-resolution export for subscribers.
