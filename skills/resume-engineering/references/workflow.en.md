# STAR workflow for AI resumes

Apply STAR to every project, including work, internships, open-source contributions, and independent projects. Use four separate labeled bullets per project, in STAR order.

1. Extract **Background** (users, problem, constraints), **My responsibilities** (goal and personal ownership), **Action** (decisions, mechanisms, and tradeoffs), and **Result** (verified outcome, scope, and attribution). Use the supplied material as the source of truth. If the user supplies only a job description, ask up to three focused questions to gather relevant STAR material.
2. Choose and order projects by the work the target role actually does. Research and training may emphasize baselines and ablations. Application and platform roles may emphasize workflows, reliability, latency, or cost. Data, safety, and evaluation may emphasize dataset coverage, scoring criteria, and verified findings. Product, design, governance, and customer-facing roles may emphasize user research, acceptance criteria, adoption, or completed remediation.
3. Draft four separate lines labeled **Background**, **My responsibilities**, **Action**, and **Result**. Use the action line to explain the candidate’s most important decision or contribution. Shorten individual lines for a one-page resume.
4. Keep metrics tied to the known baseline, unit, measurement window, and environment. Distinguish offline evaluation, pilot outcomes, and production results. Attribute team results explicitly. Use qualitative evidence when a number is unavailable, and use causal wording only when the evidence supports it.
5. Deliver the copy-ready text first. Keep unresolved facts outside the resume and mention up to three only when they affect the wording. Remove confidential details from public-facing drafts.

## Project excerpts from the original resume

The examples below follow the original resume's headings. For a new draft, use Background, My Responsibilities, Action, and Result as described above.

### EC-Monica · E-commerce Operations Agent

**Douyin E-commerce · Marketing and Interactive Experiences | May–September 2025**

- **Background:** Built an e-commerce agent for product, operations, and engineering teams to analyze data, generate reports, investigate business changes, and interpret requirements documents.
- **Impact:** The agent averaged 600+ calls per month after launch. Reports accounted for about 55% of calls, and requirements analysis and attribution accounted for about 45%. A single analysis report took 1–2 hours to write manually and 5–15 minutes to generate with the agent. Using sample business reports as few-shot examples improved alignment with internal templates. Repeat usage and proactive recommendations continued to rise.
- **My responsibilities:** Owned the project from initial design through launch.
  - **Agentic Workflow:** Classified intent and routed requests to direct generation or tool execution. The Tool Registry loaded function schemas from `cfg.json`. For tool-based requests, the workflow selected tools iteratively, calculated year-over-year and period-over-period changes, and added those figures to the model context. The model generated intermediate findings and assembled them into a final report. The tool layer classified errors and retried timed-out calls, with direct generation as the fallback.
  - **Context Engineering:** Used sample business reports and operations templates as few-shot examples. Summarized tool observations and applied a sliding window so later reasoning steps could reuse the relevant findings.

### Thumbnail AI · Mountex

- **Product overview:** A multi-platform AI thumbnail tool built with MkSaaS and Next.js ([thumbnail-ai.com](https://www.thumbnail-ai.com/)). Creators publishing on YouTube, Instagram, Facebook, X, LinkedIn, or TikTok can select a platform size, choose a style reference, and upload a subject to produce a thumbnail in three steps. The tool is designed to help creators improve click-through rates.
- **My responsibilities:** Owned the project from the start. Built the Next.js frontend, payment and subscription flows, and platform size and style settings. Designed and integrated the image generation workflow, including prompts, batch generation in multiple sizes, and improvements to cost and usability.
