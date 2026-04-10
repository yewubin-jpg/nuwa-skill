---
name: nuwa-skill
description: |
  女娲.skill - 认知操作系统生成器。
  用于自动化生成特定人物的「认知操作系统」Skill。
  当用户要求「蒸馏一个XXX」「帮我创建一个XXX的Skill」「提取XXX的思维框架」时触发。
  通过6个Agent并行调研、交叉验证、构建SKILL.md、质量验证等完整工作流程，
  将一个人物的公开言论、著作、经历蒸馏为可运行的思维框架。
license: MIT
---

# 女娲.skill (Nuwa Skill)

> 「抟土造人，炼石补天。蒸馏智慧，构建认知。」

女娲.skill 是一个元级 Skill（Meta-Skill），专门用于自动化生成特定人物的「认知操作系统」Skill。它不是简单地收集语录，而是通过深度的多维度调研，提炼出该人物的核心心智模型、决策启发式和表达 DNA，最终生成一个可运行的、具备 Agentic Protocol 的角色扮演 Skill。

## 核心工作流 (The Nuwa Protocol)

当用户请求蒸馏一个人物（如：「蒸馏一个乔布斯」）时，必须严格按照以下 5 个阶段执行：

### 阶段一：初始化与目标确认
1. 确认目标人物的姓名及核心领域（如：张雪峰-教育/职业规划，乔布斯-产品/设计/战略）。
2. 创建目标目录结构：`/home/ubuntu/skills/{name}-skill/` 及其子目录 `references/research/` 和 `examples/`。

### 阶段二：6 维度并行调研 (Parallel Research)
必须使用 `search` 工具进行广泛而深入的调研，分别从 6 个维度收集信息，并将结果保存到 `references/research/` 目录下：
- **维度 1：著作与系统思考** (`01-writings.md`) - 搜集出版书籍、核心论点体系、自创术语。
- **维度 2：深度采访与对谈** (`02-conversations.md`) - 搜集权威媒体采访、长篇对谈记录。
- **维度 3：表达风格 DNA** (`03-expression-dna.md`) - 搜集金句、口头禅、幽默方式、辩论策略。
- **维度 4：他者视角与批评** (`04-external-views.md`) - 搜集外界评价、争议事件、学术界/行业批评。
- **维度 5：重大决策分析** (`05-decisions.md`) - 搜集人生关键节点的决策及其言行一致性。
- **维度 6：完整人生时间线** (`06-timeline.md`) - 梳理出生、求学、职业转折等关键时间点。

*注：详细的调研指南和 Prompt 模板请参考 [references/agent-prompts.md](references/agent-prompts.md)。*

### 阶段三：交叉验证与提炼 (Synthesis)
综合 6 个维度的调研结果，提炼出以下核心要素：
1. **核心心智模型 (3-5个)**：该人物观察世界、分析问题的底层逻辑。
2. **决策启发式 (5-8条)**：该人物在面临选择时使用的具体规则或追问框架。
3. **表达 DNA**：句式特点、高频词汇、节奏感、幽默方式。
4. **内在张力与矛盾**：该人物言行不一之处或思想的局限性（避免脸谱化，增加真实感）。

### 阶段四：构建 SKILL.md (Generation)
基于提炼出的核心要素，生成目标人物的 `SKILL.md` 文件。
**关键要求**：生成的 Skill 必须包含「Agentic Protocol」（即：在回答前必须先查阅相关数据或事实，而不是凭空捏造）。
*注：SKILL.md 的标准结构模板请参考 [references/skill-template.md](references/skill-template.md)。*

### 阶段五：质量验证与测试 (Validation)
在交付前，必须进行以下测试，并将结果记录在 `examples/demo-conversation.md` 中：
1. **3 个已知场景测试**：针对该人物擅长的典型问题进行提问。
2. **1 个边缘场景测试**：针对新事物（如 AI 时代的影响）进行提问，测试心智模型的泛化能力。
3. **风格测试**：检查回答是否符合该人物的表达 DNA（如：是否使用了口头禅、是否具备相应的幽默感或压迫感）。

## 交付标准
完成上述流程后，向用户交付：
1. 完整的 `{name}-skill` 目录结构。
2. 核心的 `SKILL.md` 文件。
3. 包含 6 个调研文档的 `references/research/` 目录。
4. 包含测试对话的 `examples/demo-conversation.md`。

## 辅助资源
- 调研指南与 Prompt：[references/agent-prompts.md](references/agent-prompts.md)
- SKILL.md 生成模板：[references/skill-template.md](references/skill-template.md)
- 质量验证指南：[references/validation-guide.md](references/validation-guide.md)
