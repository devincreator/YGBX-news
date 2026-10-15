# YGBX-news

《每周信息参考》保险资讯编辑仓库。

本仓库包含可复用的 **weekly-insurance-news** Skill，用于检索、核验、筛选并撰写每周国内资讯，遵循“先提交备选、用户确认后再更新 Word”的流程。

## 快速入口

- Skill：[`.agents/skills/weekly-insurance-news/SKILL.md`](.agents/skills/weekly-insurance-news/SKILL.md)
- 四板块边界与负面清单：[`references/editorial-policy.md`](.agents/skills/weekly-insurance-news/references/editorial-policy.md)
- 原文核实和质量门槛：[`references/verification.md`](.agents/skills/weekly-insurance-news/references/verification.md)
- v3 写作与 Word 规则：[`references/v3-format.md`](.agents/skills/weekly-insurance-news/references/v3-format.md)
- 每周操作流程：[`workflows/weekly-run.md`](.agents/skills/weekly-insurance-news/workflows/weekly-run.md)
- OpenSpec 稳定需求：[`openspec/specs/weekly-news/spec.md`](openspec/specs/weekly-news/spec.md)

## 使用方式

在支持项目级 Agent Skills 的代理环境中打开本仓库，说“按《每周信息参考》标准，找上周五至本周四四大板块的新闻”，即可调用 Skill。若当前客户端无法自动发现该目录，直接要求代理阅读上面的 SKILL.md 再执行。

默认仅做 **国内四个板块**：保险行业、监管动态、经济与社会、同业动态。先提供有来源链接的候选清单，确认序号后才制作最终内容。原则上每板块 5–7 条候选，最终目标约 3/3/4/5 条；如果有效新闻不足，不凑数。

## 状态与边界

- 本仓库初始化时并未提供实际 **v3 定稿 DOCX 模板**，因此规范已经写入，但具体封面、目录、编号、页眉页脚样式仍需以用户提供的真实模板为准，**不得假称已完成像素级排版适配**。
- Skill 不自带联网检索能力；它规定如何使用运行环境内可用的检索、网页读取和文档编辑工具，不绑定名为 google 的专有工具。
- 只有用户确认后才更新终稿；不擅自发送、公开发布或上传含内部内容的周报。
- OpenSpec 仅用于管理 **规则变化**，不是每次周报制作都要执行的额外审批流程。

编辑与变更请遵循 [AGENTS.md](AGENTS.md) 和 [OpenSpec 变更约定](openspec/changes/README.md)。
