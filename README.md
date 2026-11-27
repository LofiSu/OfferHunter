# OfferHunter · AI 岗位简历写作与 STAR 改写

简体中文 | [English](README.en.md)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

**OfferHunter 是一款面向 AI 求职的开源简历写作 Agent Skill。** 用 Codex 把项目笔记、旧简历和岗位 JD 写成可投递的一页简历。可以从零写整份简历、重组工作与实习经历，也可以只改一条 STAR 项目要点。支持中文、英文和双语稿，附黑白单栏 HTML 与 LaTeX 简历模板。

- **按目标岗位选素材**。适用于 LLM 与 Agent 应用工程、机器学习研究与工程、模型评测、AI 产品、数据、MLOps、推理平台和解决方案等方向。[100 条 BOSS 直聘岗位索引](skills/resume-engineering/references/ai-roles.md)
- **用真实项目学习怎么写**。EC-Monica 电商 Agent 案例展示如何按「背景 → 指标与效果 → 我的职责」写清项目范围、技术链路和上线结果。[中文 STAR 案例](skills/resume-engineering/references/examples.md)
- **让整份稿子更好扫读**。调整栏目顺序，压缩低相关内容，保留能说明个人职责和交付的证据。[简历结构指南](skills/resume-engineering/references/resume-structure.md)

[快速开始](#快速开始) · [STAR 写法](#用-star-写项目经历) · [HTML 模板](#html-简历模板) · [常见问题](#常见问题)

## 一句话安装

```text
请克隆 https://github.com/LofiSu/OfferHunter，并把 skills/resume-engineering 安装到当前 Codex 项目的 .agents/skills/。
```

## 快速开始

```sh
git clone https://github.com/LofiSu/OfferHunter.git /path/to/OfferHunter
mkdir -p .agents/skills
cp -R /path/to/OfferHunter/skills/resume-engineering .agents/skills/
```

在该项目中调用 `$resume-engineering`，附上旧简历或项目笔记。有目标 JD 时一并提供。

## 用 STAR 写项目经历

- **S · 情境**：服务对象是谁，遇到了什么问题，有哪些约束。
- **T · 任务**：项目要达到什么目标，自己负责哪部分。
- **A · 行动**：用短标题拆开关键模块，写清自己做过的事、方案如何运转，以及有依据的取舍。
- **R · 结果**：把可验证的成效放在对应动作后，或在项目总览中注明团队成效。缺少数字时，可以写已交付的能力、采纳情况或验证发现。

成稿沿用「背景与目标」「我的职责」的结构，结果可以放在对应职责之后。一页简历可把这几部分压进一条要点。

适用于 AI 研究、模型训练、应用、基础设施、数据、评测、安全、产品、设计、治理和商业落地等方向。用目标岗位的实际工作挑选经历，同一段经历可按不同岗位突出不同动作。[AI 岗位取材参考](skills/resume-engineering/references/ai-roles.md) · [改写示例](skills/resume-engineering/references/examples.md)

## 可以这样用

- 「按这份 AI 应用工程 JD 改写我的两段项目经历。每段保留最能体现工程取舍的两个要点。」
- 「把这份项目复盘写成可投递的一页简历。上线效果是团队数据，我个人负责的是流程编排。」
- 「审一遍这份简历。找出说不清归因的数字，给我可以直接替换的写法。」

Skill 默认输出可复制的简历文本。项目级结果与个人职责各自注明主语，缺失的信息放在成稿之外。使用时只需提供你愿意交给客户端处理的素材。

查看 [EC-Monica 电商产运 Agent 的完整 STAR 改写](skills/resume-engineering/references/examples.md)。

## 整份简历与 LaTeX

可以从旧简历或项目笔记起草整份简历，也可以调整栏目顺序、压缩正文或只改一段经历。默认沿用「页首 → 工作经历 → 实习经历 → AI 创业／独立项目」的结构，按需呈现教育、开源和奖项。LaTeX 版采用简洁的黑白单栏排版。

[Resume structure](skills/resume-engineering/references/resume-structure.md) · [LaTeX template](skills/resume-engineering/templates/resume.tex)

## HTML 简历模板

复制下面的代码，保存为 `resume.html`，在浏览器中打开。填写后可用浏览器的打印功能导出 A4 PDF。

```html
<!doctype html>
<html lang="zh-CN">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>候选人姓名</title>
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
    time { white-space: nowrap; }
    .entry-heading { display: flex; justify-content: space-between; flex-wrap: wrap; gap: .25em 1em; }
    @media print {
      body { max-width: none; margin: 0; padding: 0; }
      h2, h3 { break-after: avoid; }
      li { break-inside: avoid; }
    }
  </style>
</head>
<body>
  <header>
    <h1>候选人姓名</h1>
    <p><a href="mailto:hello@example.com">hello@example.com</a> ·
       <a href="https://example.com">作品集</a></p>
    <p>学校 · 专业 · 毕业年份</p>
    <p>代表性开源贡献或奖项</p>
  </header>
  <main>
    <section>
      <h2>工作经历</h2>
      <div class="entry-heading">
        <h3>公司 · 岗位</h3>
        <span><time datetime="2025-01">2025.01</time>–<time datetime="2025-12">2025.12</time></span>
      </div>
      <p><strong>项目名称 · 项目角色</strong></p>
      <ul>
        <li><strong>背景</strong> — 服务对象、业务问题和项目目标。</li>
        <li><strong>指标与效果</strong> — 写可核对的交付、采纳情况或量化结果。</li>
        <li><strong>我的职责</strong> — 写清本人完成的关键动作、实现方式和交付。</li>
      </ul>
    </section>
    <section>
      <h2>实习经历</h2>
      <h3>公司 · 岗位</h3>
      <ul><li>写一条与目标岗位相关的个人贡献。</li></ul>
    </section>
    <section>
      <h2>AI 创业／独立项目</h2>
      <h3>项目名称 · 项目角色</h3>
      <ul><li>写明个人角色、已交付的功能和实际效果。</li></ul>
    </section>
  </main>
</body>
</html>
```

## 常见问题

### 没有目标 JD，能先写一整份 AI 简历吗？

可以。先用旧简历或项目笔记起草，优先写职责和结果最清楚的经历。拿到岗位 JD 后，再按该岗位的实际工作重排和精简。

### STAR 法则怎么用在一页简历里？

把情境和任务压成一句话，用动作写清个人贡献，再接上能核对的结果。团队数据写清归属。没有量化数据时，可以写已上线能力、实际采纳或验证发现。

### HTML 或 LaTeX 简历如何导出 PDF？

HTML 可用浏览器的打印菜单导出 A4 PDF。LaTeX 源文件可用 XeLaTeX 编译。两份模板都使用单栏布局，适合突出内容和阅读顺序。

### BOSS 直聘岗位索引是什么？

索引来自公开招聘列表，保留职位名、可见 JD 关键词、STAR 取材提示和来源。采集日期和访问限制见[岗位参考](skills/resume-engineering/references/ai-roles.md)。

## 贡献

欢迎通过 [Issues](https://github.com/LofiSu/OfferHunter/issues) 提交可追溯的公开 JD、脱敏案例或模板改进。如果 OfferHunter 帮你把一段经历写得更清楚，欢迎在 GitHub 点一颗 Star。

## 许可

[MIT](LICENSE)
