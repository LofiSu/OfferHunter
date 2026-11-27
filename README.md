# OfferHunter

简体中文 | [English](README.en.md)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

OfferHunter 是一款开源 Agent Skill，用 STAR 将真实项目经历写成可投递的 AI 岗位简历。支持中文、英文和双语输出。

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

## 许可

[MIT](LICENSE)
