---
name: resume-engineering
description: Writes, reviews, and tailors resumes for AI-related technical and nontechnical roles using STAR. Use for AI research, engineering, infrastructure, data, evaluation, product, design, deployment, governance, and adjacent roles, or when users request AI 岗位整份简历、简历结构调整、LaTeX 简历、按 JD 定制、项目经历改写、转岗简历、一页压缩或 STAR 要点。
license: MIT
---

# 用 STAR 法则写 AI 求职简历

把工作和项目素材写成招聘方能快速读懂、面试时能深入追问的简历。默认用用户要求的语言呈现。保留源材料中的英文技术名词，首次出现的内部缩写用通用术语交代。

## 在不同 Agent 中使用

此技能以随附的 Markdown 指令和参考资料为基础。能读取项目文件时，按需打开链接所指的文件。在聊天中只能看到附件或粘贴内容时，直接按本页写作。需要特定示例或模板时，使用用户已提供的文件。

## 整份简历与结构重组

- 用户要求从零写整份简历、改整份简历或调整栏目顺序时，读取 [整份简历结构](references/resume-structure.md)。先整理页首、工作、实习、独立项目和适用的其他栏目，再为其中的项目写 STAR。交付完整成稿。
- 用户要求 LaTeX、PDF 或论文风格排版时，按结构说明选用 [单栏 LaTeX 模板](templates/resume.tex)。首选一页、黑白和清晰标题层级。排版要求本身无需把聊天正文转换成 LaTeX，除非用户需要源文件或 PDF。

## 每个项目写成四行 STAR

无论是整份简历还是单个项目，成稿中的每个项目都用以下四行，顺序固定。工作、实习、开源和独立项目都适用。一页稿可以缩短每行。

- **情境（S）**：说明服务对象和实际问题，必要时补充约束。
- **任务（T）**：说明项目目标和本人承担的交付。
- **行动（A）**：用一到两句话说明本人做了什么、用了什么关键办法。
- **结果（R）**：写可核对的交付、采纳或验证结果。涉及指标时保留基线、单位、环境和已知的统计范围。注明团队成果的归属。

英文使用 **Situation / Task / Action / Result**，同样各占一行。Markdown 用四条列表项，HTML 用四个列表项，LaTeX 用四个 `item`。正文里的项目只展示一组 STAR。只有 JD 时，围绕实际职责提出最多三个取材问题。缺乏量化数据时可用已实现的功能或验证发现。结果尚未核实时写清已确认的阶段，将待补资料放在成稿外。

见 [项目示例](references/examples.md)。

## AI 岗位适配

- 根据 JD 的主要交付挑选最相关的 STAR 经历。只有岗位名称时，可参考 [各类 AI 岗位的取材方向](references/ai-roles.md)。岗位也未知时，优先使用职责最清楚、结果最扎实的经历。
- 多个 JD 共用一份 STAR 素材库，为每个 JD 单独选材、排序和改写。可以复用同一事实的不同切面，保留原有职责、工具、验证环境和归属。
- 转岗素材写清原场景以及被验证的能力。模型表现注明评测范围和对照条件，业务表现注明观测范围，产品、设计及治理交付可用采纳记录、验证发现和整改闭环。

## 交付前核对

- 招聘方能在第一次扫读时看懂做了什么、候选人负责什么、结果如何。
- 每条核心经历都能用素材回答「为什么这样做」「结果怎么知道」。素材薄弱时保留能确定的动作和交付。
- 数字与单位一致，团队成果有明确主语，正文没有待确认占位符。面向公开场合时移除未获准公开的指标、内部项目标识和私人链接。
- 用户要求成稿时先给可直接粘贴的文本。只在确实影响措辞时，附最多三个按优先级排序的待确认项。用户要求直接给稿时，用简短陈述说明影响最大的证据缺口。做原稿审阅时先指出最影响判断的几处，并给出替换文案。

## English requests

For English requests, read the [English STAR workflow and examples](references/workflow.en.md) and deliver the resume in English. For bilingual requests, write both drafts from the same verified facts, maintaining ownership, scope, and metric definitions across languages.
