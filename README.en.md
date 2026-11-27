# OfferHunter · Open-source AI Resume Writer and STAR Resume Skill

English | [简体中文](README.md)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

**OfferHunter is an open-source AI resume writer and editing skill for Claude, ChatGPT, Codex, Grok, and other AI assistants.** Turn project notes, an existing resume or CV, and a target job description into a focused application. Draft a full resume, reorganize work and internship sections, or rewrite individual bullets using STAR. Write in English, Chinese, or both, with minimalist HTML and LaTeX templates.

- **Tailor the resume to the role.** Use it for LLM and AI agent engineering, machine learning research, model evaluation, AI product management, data, MLOps, inference infrastructure, and solutions engineering. [100 BOSS Zhipin job samples](skills/resume-engineering/references/ai-roles.md)
- **Learn from a real project.** The EC-Monica e-commerce agent example pairs business context and measurable impact with specific engineering contributions. [English STAR case study](skills/resume-engineering/references/workflow.en.md)
- **Edit the whole document.** Reorder sections, shorten low-relevance entries, and foreground evidence of ownership and delivery. [Full resume structure](skills/resume-engineering/references/resume-structure.md)

[Quick start](#quick-start) · [STAR method](#write-with-star) · [HTML template](#html-resume-template) · [FAQ](#faq)

## Quick Start

Clone into your project, then run the install command for your client.

```sh
git clone https://github.com/LofiSu/OfferHunter.git
```

```sh
# Claude Code
mkdir -p .claude/skills && cp -R OfferHunter/skills/resume-engineering .claude/skills/
# Codex
mkdir -p .agents/skills && cp -R OfferHunter/skills/resume-engineering .agents/skills/
# Grok CLI
mkdir -p .grok/skills && cp -R OfferHunter/skills/resume-engineering .grok/skills/
```

Start a new session and ask your agent to use `resume-engineering`.

**ChatGPT, Claude, and Grok on the web** — Attach or paste [SKILL.md](skills/resume-engineering/SKILL.md) with your resume or project notes and, if available, the target job description. For API integrations, see the [OpenAI Skills guide](https://developers.openai.com/api/docs/guides/tools-skills).

## Write with STAR

- **Situation** — Identify the users, the problem, and the constraints.
- **Task** — State the project goal, then name what you owned.
- **Action** — Use short headings for key contributions. Describe what you did, how it worked, and the tradeoffs that mattered.
- **Result** — Attach verified outcomes to the relevant action. Attribute team outcomes to the team. When metrics are unavailable, describe a delivered capability, documented adoption, or a validated finding.

Write each project as four labeled lines in this order: **Situation**, **Task**, **Action**, and **Result**. Keep the lines short for a one-page resume.

Use OfferHunter for research, training, applications, infrastructure, data, evaluation, safety, product, design, governance, and customer-facing deployment. The target role guides which experiences to highlight.

## Example

“Rewrite these two projects for an AI evaluation role. Keep the offline test scope and distinguish my work from the team's results.”

See how an AI thumbnail generator project becomes a copy-ready resume entry. [English STAR workflow and examples](skills/resume-engineering/references/workflow.en.md)

See the [EC-Monica e-commerce operations agent case study](skills/resume-engineering/references/workflow.en.md) for a full STAR breakdown and resume-ready entry.

## Full resumes and LaTeX

Draft a full resume from project notes, reorganize an existing resume, or rewrite one entry. The default structure is a compact header followed by work experience, internships, and independent AI projects. Education, open-source work, and awards appear where relevant. The LaTeX template uses a clean, single-column layout.

[Resume structure](skills/resume-engineering/references/resume-structure.md) · [LaTeX template](skills/resume-engineering/templates/resume.tex)

## HTML Resume Template

![Single-column resume preview with work experience, internships, and independent AI projects](assets/resume-preview-project-ownership-en.png)

Copy the code into `resume.html`, open it in a browser, and use the print menu to export an A4 PDF.

<details>
<summary>Show and copy the HTML source</summary>

```html
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Your Name</title>
  <style>
    @page { size: A4; margin: 17mm 19mm; }
    body {
      max-width: 172mm; margin: 2rem auto; padding: 0 1rem;
      color: #171717; background: #fff;
      font: 11pt/1.45 "Times New Roman", "Songti SC", "Noto Serif CJK SC", serif;
    }
    h1 { margin: 0 0 .2em; font-size: 25pt; }
    h2 { margin: 1em 0 .35em; border-bottom: 1px solid; font-size: 13pt; }
    h3, p { margin: .25em 0; }
    h3 { font-size: 11pt; }
    ul { margin: .25em 0; padding-inline-start: 1.2em; }
    li { margin: .2em 0; }
    a { color: inherit; }
    .contact { overflow-wrap: anywhere; }
    .resume-company-heading { margin: .4em 0; }
    .resume-project { margin: .4em 0 .6em; }
    .resume-project h4 { margin: .2em 0; font-size: 11pt; }
    ul ul { list-style-type: circle; }
    @media print {
      body { max-width: none; margin: 0; padding: 0; }
      h2, h3, h4 { break-after: avoid; }
      li { break-inside: avoid; }
    }
  </style>
</head>
<body>
  <header>
    <h1>Your Name</h1>
    <p class="contact"><a href="https://github.com/username">github.com/username</a> |
      <a href="tel:+12025550101">+1 202 555 0101</a> |
      <a href="mailto:hello@example.com">hello@example.com</a></p>
    <p>University · Degree (2022–2026)</p>
    <p><strong>Open Source &amp; Awards</strong> · Add one relevant contribution or award</p>
  </header>
  <main>
    <section>
      <h2>Work Experience</h2>
      <h3 class="resume-company-heading">Company | Role | Jul 2026–Present</h3>
      <!-- Copy a resume-project block below when adding work projects. -->
    </section>

    <section>
      <h2>Internships</h2>
      <h3 class="resume-company-heading">Company · E-commerce Team | AI Application Intern | Jun–Sep 2025 (example)</h3>
      <article class="resume-project">
        <h4>EC-Monica · E-commerce Operations Agent</h4>
        <ul>
          <li><strong>Situation</strong> · E-commerce teams needed to query data, investigate metric changes, and write reports.</li>
          <li><strong>Task | My role</strong> · As project owner, I was responsible for designing the e-commerce operations agent, orchestrating its tools, and taking it through launch.</li>
          <li><strong>Action</strong> · Built intent routing, retries, and fallback handling. Used Python to calculate year-over-year and period-over-period changes, and used operations templates to guide report generation.</li>
          <li><strong>Result</strong> · Averaged 600+ calls per month. Reports took 1–2 hours to write manually and 5–15 minutes to generate.</li>
        </ul>
      </article>
    </section>

    <section>
      <h2>Independent AI Projects</h2>
      <article class="resume-project">
        <h4>AI Thumbnail Generator</h4>
        <ul>
          <li><strong>Situation</strong> · Creators needed thumbnails in different sizes for different platforms.</li>
          <li><strong>Task | My role</strong> · I owned the generation workflow and subscription features, from platform selection and asset uploads through preview and download.</li>
          <li><strong>Action</strong> · Built platform presets, subject uploads, and style-reference inputs in Next.js. Used platform-specific prompts to call an image generation API and implemented free usage and subscriptions.</li>
          <li><strong>Result</strong> · Shipped multi-platform preview and download, with batch generation and high-resolution export for subscribers.</li>
        </ul>
      </article>
    </section>
  </main>
</body>
</html>
```

</details>

## FAQ

### Can I write a full AI resume without a target job description?

Yes. Start with an existing resume or project notes and prioritize entries with clear ownership and outcomes. Once you have a job description, reorder and shorten the draft around the work that role actually does.

### How do I use STAR on a one-page resume?

Write four brief lines per project: Situation, Task, Action, and Result. Attribute team outcomes. A shipped capability, documented adoption, or validated finding can also show impact.

### How do I export a resume to PDF?

Use your browser’s print menu to export the HTML version as A4 PDF. The LaTeX template is intended for XeLaTeX. Both use a single-column layout.

### Where do the job description examples come from?

The index uses public BOSS Zhipin recruiting lists. It records role titles, visible JD keywords, STAR prompts, and source links. See the [job reference](skills/resume-engineering/references/ai-roles.md) for collection dates and coverage.

## Contributing

Share traceable job postings, anonymized resume examples, or template improvements through [GitHub Issues](https://github.com/LofiSu/OfferHunter/issues). If OfferHunter helped you turn a project into a stronger resume entry, consider starring the repository.

## License

[MIT](LICENSE)
