# 提问增强与思考路由 · Prompt Method Router

根据问题场景自动选择十二条完整原文 Prompt 模板，将用户背景和问题填入，展示可复制的完整改写，再按模板执行。需要追问或确认时，保留等待用户回答的步骤。

## 让 AI 帮你安装

把下面整段复制给支持技能安装的 AI：

```text
请帮我安装“提问增强与思考路由”技能：
https://github.com/LINYU19990730/prompt-method-router

技能目录：skills/prompt-method-router
技能名称：prompt-method-router
分支：main

请先检查技能内容，再按当前平台支持的方式完整安装整个技能目录，
包含 SKILL.md、agents、references 和 assets。
保留十二条完整原文 Prompt、具体问法和多轮等待规则，支持时开启自动调用。
安装后验证技能可加载、十二条参考模板齐全。
如果当前平台不支持安装，请如实说明，不要把阅读成功当成安装成功。
```

本仓库是独立技能项目。安装目录：[skills/prompt-method-router](skills/prompt-method-router)，默认分支为 `main`。

安装能力取决于客户端：支持联网和技能管理的 AI 才能实际安装。普通聊天窗口阅读这些文件，并不等于持久安装。本仓库也不代表已在官方公共插件目录上架。

- Codex 等支持 Agent Skills 的环境：请使用其官方技能安装方式，从本仓库 `main` 分支安装 `skills/prompt-method-router`。
- 提供账号端技能创建/导入能力的 ChatGPT 界面：请通过 skill-creator 完整导入并安装，确认出现在“已安装”中。具体可用性取决于账号及工作区权限。
- 本机安装与账号端安装的范围不同；需要跨设备使用时应确认目标平台实际保存到账号。
- 遇到同名技能，应先说明，不直接覆盖已有版本。

## 十二种完整模板

| 方法 | 原文模板 |
| --- | --- |
| 苏格拉底式提问 | [查看](skills/prompt-method-router/references/01-socratic.md) |
| 双层解释法 | [查看](skills/prompt-method-router/references/02-two-layer.md) |
| 反向拆解 | [查看](skills/prompt-method-router/references/03-reverse-engineer.md) |
| 横纵分析法 | [查看](skills/prompt-method-router/references/04-horizontal-vertical.md) |
| 事实核查 | [查看](skills/prompt-method-router/references/05-fact-check.md) |
| 专家会诊 | [查看](skills/prompt-method-router/references/06-expert-panel.md) |
| 第一性原理 | [查看](skills/prompt-method-router/references/07-first-principles.md) |
| 跨领域借解 | [查看](skills/prompt-method-router/references/08-cross-domain.md) |
| 双向钢人论证 | [查看](skills/prompt-method-router/references/09-steelman.md) |
| 用最小实验替代空想 | [查看](skills/prompt-method-router/references/10-minimum-experiment.md) |
| 挖掘隐藏天赋 | [查看](skills/prompt-method-router/references/11-hidden-talents.md) |
| 人生设计术 | [查看](skills/prompt-method-router/references/12-life-design.md) |

## 如何使用

安装后直接正常提问，例如：“我想学习函数这个概念。”
技能会匹配“双层解释法”，展示完整改写后的 Prompt，再给出通俗解释、专业解释、术语对应、误区和三个自检问题。

也可以明确说：“使用 prompt-method-router，按完整原文模板改写并执行我的问题：……”

- 苏格拉底问诊：最多六个主问题，一次一问；整理出新问题后先等待确认，再给建议。
- 双向钢人论证：先比较两方最强理由，再问关键问题，等待回答后给判断。
- 隐藏天赋与人生设计：保留多轮访谈和完整输出要求。
- 原文中的字数、数量和步骤默认保留；用户明确要求简短、停止或调整任务时优先遵从。
- 简单算术、翻译、快捷键和明确的单步操作直接回答。

## 文件组成

```text
skills/prompt-method-router/
  SKILL.md
  agents/openai.yaml
  references/（十二条完整原文 Prompt）
  assets/icon.svg
```

## 安装验收

1. 技能主文件可以加载。
2. 十二个参考模板文件齐全，相对链接有效。
3. 客户端支持时已启用按场景自动调用。
4. 在问诊场景中按原文一次一问、等待回答，不抢先给最终方案。

## 来源与署名

原文作者：卡兹克。
原文文章：《都Agent时代了，我还是想分享给你这12个我最常用的Prompt。》。

十二条原文 Prompt 从用户提供的文章正文提取，仅统一换行；不包含读者留言。
本项目整理了模板自动选择、提问改写和流程执行规则，不代表原文作者官方出品。
仓库没有为第三方原文另行授予开源许可。
