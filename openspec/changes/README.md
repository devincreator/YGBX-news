# OpenSpec change workflow

这里用于管理**长期采编规则变化**，不是每期周报的任务记录。正式每周执行步骤见 Skill 的 `workflows/weekly-run.md`。

## 触发条件

以下情况建议创建变更目录：新增国际板块；调整保险行业与同业动态界线；修改负面清单；改变默认周窗口；改变“先选后写”确认规则；新增自动归档/发送/发布能力；替换 v3 排版协议或引入真正的模板自动化。

日常查新闻、纠正单条报道、补充本期新闻、按用户选择输出 Word **无需** OpenSpec。

## 最小约定

每项变化新建 `openspec/changes/<YYYY-MM-DD>-<short-slug>/`，至少记录：

- `proposal.md`：原规则、要改变什么、为什么、对现有输出的影响
- `tasks.md`：需要修改的 SKILL、reference、workflow、模板或脚本，以及核验方式
- `specs/weekly-news/spec.md`：对上述稳定要求的增量（Added / Modified / Removed）

如变更涉及多个系统或实现取舍，可添加 `design.md`。用户确认后再执行变更；验证后将新规则合入 `openspec/specs/weekly-news/spec.md` 和 Skill 对应参考文件，并将变更目录归档/保留以供追溯。

## 验收

针对每次变更列举至少一个**应收录**、一个**应排除**或**应特殊处理**的例子；检查此前约定仍然成立；不得悄悄改变用户已经批准的文案或每周工作流程。

此目录使用 OpenSpec 的需求/提案/任务管理思想，**未宣称已安装 OpenSpec CLI 或配置可执行命令**。如需真正接入 CLI，请在实际开发环境确认版本和仓库配置，再补充其要求的配置文件与命令。
