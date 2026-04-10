<div align="center">

# 女娲.skill (Nuwa Skill)

> *「抟土造人，炼石补天。蒸馏智慧，构建认知。」*

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Manus](https://img.shields.io/badge/Manus-Skill-blueviolet)](https://manus.im)

<br>

**认知操作系统生成器。不是简单的语录收集，而是可运行的思维框架。**

<br>

输入一个名字，通过 6 个 Agent 并行调研、交叉验证、构建 SKILL.md、质量验证等完整工作流程，<br>
将该人物的公开言论、著作、经历蒸馏为可运行的思维框架。

[安装](#安装) · [工作流](#核心工作流-the-nuwa-protocol) · [目录结构](#目录结构)

</div>

---

## 什么是女娲.skill？

女娲.skill 是一个元级 Skill（Meta-Skill），专门用于自动化生成特定人物的「认知操作系统」Skill。它通过深度的多维度调研，提炼出该人物的核心心智模型、决策启发式和表达 DNA，最终生成一个可运行的、具备 Agentic Protocol 的角色扮演 Skill。

## 安装

将此仓库克隆到你的 skills 目录下：

```bash
cd ~/skills
git clone https://github.com/yewubin-jpg/nuwa-skill.git
```

然后在 Manus 中：

```
> 蒸馏一个乔布斯
> 帮我创建一个马斯克的Skill
> 提取叶武滨的思维框架
```

---

## 核心工作流 (The Nuwa Protocol)

当触发蒸馏任务时，女娲.skill 会严格执行以下 5 个阶段：

### 阶段一：初始化与目标确认
确认目标人物的姓名及核心领域，创建目标目录结构。

### 阶段二：6 维度并行调研 (Parallel Research)
使用 6 个 Agent 并行搜集信息：
1. **著作与系统思考**：搜集出版书籍、核心论点体系、自创术语。
2. **深度采访与对谈**：搜集权威媒体采访、长篇对谈记录。
3. **表达风格 DNA**：搜集金句、口头禅、幽默方式、辩论策略。
4. **他者视角与批评**：搜集外界评价、争议事件、学术界/行业批评。
5. **重大决策分析**：搜集人生关键节点的决策及其言行一致性。
6. **完整人生时间线**：梳理出生、求学、职业转折等关键时间点。

### 阶段三：交叉验证与提炼 (Synthesis)
综合调研结果，提炼出核心心智模型、决策启发式、表达 DNA 和内在张力。

### 阶段四：构建 SKILL.md (Generation)
基于提炼出的核心要素，生成目标人物的 `SKILL.md` 文件，并确保包含「Agentic Protocol」（先查数据再开口）。

### 阶段五：质量验证与测试 (Validation)
进行 3 个已知场景测试、1 个边缘场景测试和风格测试，确保生成的 Skill 准确且符合人物特征。

---

## 目录结构

```
nuwa-skill/
├── README.md                         # 项目说明
├── SKILL.md                          # 核心入口，定义完整工作流
├── LICENSE                           # 开源协议
└── references/
    ├── agent-prompts.md              # 6个调研维度的Prompt模板
    ├── skill-template.md             # 目标人物SKILL.md的生成模板
    └── validation-guide.md           # 质量验证与测试指南
```

## 版权声明与致谢

**特别声明**：本仓库是基于原创者 **花叔 (Huashu / alchaincyf)** 的创意复刻版本。
- **原创作者**：[花叔 Huashu](https://github.com/alchaincyf)
- **原创仓库**：[alchaincyf/nuwa-skill](https://github.com/alchaincyf/nuwa-skill)

本复刻版本仅用于学习和交流，所有核心创意和架构设计均归原创者所有。

## 许可证

MIT License - 自由使用、修改和分发。
