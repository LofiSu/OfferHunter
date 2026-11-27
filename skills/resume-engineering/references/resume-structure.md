# 整份简历的结构

页首先交代求职方向和基本信息，正文按经历分组。每组先写公司或团队、岗位和时间，再列本人参与的项目。

1. **页首**。姓名正下方先写个人亮点，接着写目标岗位和联系方式。把「GitHub｜作品链接」单列在页首，作品链接直接指向可公开核验的代表作。确认链接无需登录即可查看。随后写学校、专业和毕业时间。开源身份、代表奖项或贡献高度相关时，可在页首加一行。熟练或资深候选人可把教育移到末尾。
2. **工作经历**。按最近到最早排列。每段先写公司、岗位、时间，再在其下放本人参与的项目。项目标题写清交付对象或产品。每个项目按「背景、我的职责、行动、结果」写四行。行动写本人做过的关键工作，结果使用可核对的指标、交付或验证。篇幅紧张时缩短每行。
3. **实习经历**。沿用工作经历结构。简历主要靠实习经历说明能力时，可以省去空的工作栏目，直接从实习写起。相关的长期兼职和独立接单可按真实身份放在此处或单列。
4. **项目经历**。放自己参与、且能说明目标岗位所需能力的项目，注明角色、交付阶段和可公开的演示或成果。避免与工作经历重复。
5. **开源、研究与奖项**。页首用一行提示最相关的可信信号。需要展开时放到独立栏目，补上项目或论文名称、具体贡献、奖项和年份。技能栏按需添加，仅保留与目标工作直接相关且有素材支撑的能力。

整份起草时，按上述顺序用已提供事实写齐可用栏目，省略空栏目。先给可以投递的草稿，待确认事实列在稿外。重组旧简历时，优先调整顺序、拆合栏目、移动重复内容和压缩低相关条目，沿用原有事实与语言，在成稿之后简述影响最大的结构变动。用户只要求调结构时，保留原句，必要的衔接可小改。

## 页首亮点

先问候选人自己最想被记住什么，再问哪份作品、哪项交付或哪个结果能证明。结合他实际擅长的工作和目标 JD，选一个能说清的亮点放在姓名下方。需要参考招聘趋势时，用近期岗位或可靠来源核实，并把正在探索的方向留给自我介绍。

- **中文示例**：从零设计并上线电商分析 Agent，负责工具编排和报告生成。
- **English example**: Owned the design and launch of an e-commerce analytics agent, including tool orchestration and report generation.

## 一句话自我介绍

写在页首作品链接下面，用一句话交代「做过什么 → 代表作 → 接下来想做什么」。过去的经历写清团队或岗位与主要工作。选一项能直接点开的作品，把链接放在作品名上。当前方向用「正在探索」或「希望转向」等符合实际阶段的说法。需要解释动机时，用半句把过去遇到的问题和未来想做的事连起来。

**中文示例（假设求职方向为 Agent 评测）**

> 我在电商团队实习时负责过数据分析 Agent 的设计和上线，也做过 [Thumbnail AI](https://www.thumbnail-ai.com/)；现在想做 Agent 评测，因为上线后我更关心怎样判断它在哪些任务上可靠。

**English example (for someone pursuing agent evaluation)**

> I designed and launched an analytics agent during an e-commerce internship and built [Thumbnail AI](https://www.thumbnail-ai.com/), and I now want to work on agent evaluation because shipping an agent made me want to understand where users can rely on it.

## 排版与交付

参考学术论文的单栏和清晰标题层级。正文以黑色为主，统一日期格式，给栏目之间留出空白。LaTeX 模板用黑白，HTML 模板用蓝色区分栏目和项目标题。姓名和栏目名足够醒目。直接使用可复制的文本和链接，省去照片、图标、技能进度条、彩色背景、侧栏和论文式双栏。默认优先用一页呈现高相关经历，材料较多时可用两页保持可读字号。

用户明确要 LaTeX 或 PDF 时，使用 [LaTeX 模板](../templates/resume.tex)。写入完整的可编译源文件，按正文或链接所在语境正确处理 LaTeX 特殊字符。用 XeLaTeX 编译，检查分页、溢出、中文字体、链接和文本复制。缺少编译环境时，交付源文件并说明 PDF 尚未生成。英文简历可将文档类改为 `article` 并翻译栏目名。

For English resumes, use the same structure with **Work Experience**, **Internships**, **Project Experience**, and optionally **Open Source, Research & Awards**. For each project, write four separate lines in this order: **Background**, **My responsibilities**, **Action**, and **Result**.
