# 宏观研究流程 · macro-research-pipeline

[English](README.md) · **简体中文**

新闻很快，传导过程值得慢慢问清楚。

将宏观事件和财经新闻整理为有来源、条件情景、交易表达和失效条件的研究记录，适用于 Codex。

## 研究流程

1. 确认事件、发布时间与市场此前的预期。
2. 识别与目标资产相关的关键变量。
3. 解释变量传导路径、成立条件与其他可能原因。
4. 查找有来源、可比较的历史案例。
5. 根据观察指标建立条件情景。
6. 形成与情景对应的交易想法，检查工具、成本和风险。
7. 定义逻辑失效、价格退出、时间到期和后续检查条件。

支持单个事件分析、每日研究、个人宏观框架建立和已有研究记录复查。

## 安装

需要 Git 和能够加载本地技能的 Codex 环境。在终端执行：

```bash
mkdir -p ~/.codex/skills
git clone https://github.com/Bill306/macro-research-pipeline.git ~/.codex/skills/macro-research-pipeline
```

安装后重新启动 Codex 或新建聊天，使技能列表更新。

## 使用

在 Codex 中输入技能名称和研究问题，例如：

```text
使用 $macro-research-pipeline 分析最近一次美联储利率决议，
研究未来一至三个月对美债和美股的影响，核验资料并生成研究记录。
```

```text
使用 $macro-research-pipeline 建立美股投资使用的个人宏观框架，
说明关键指标、数据来源、传导关系与更新条件。
```

```text
使用 $macro-research-pipeline 复查这份研究记录，
按照当时可获得的信息检查判断，并记录后续数据提供的证据。
```

涉及当前行情、政策、经济数据和历史表现时，运行技能的 AI 需要能够搜索并读取来源。资料缺失时，研究记录会说明缺口及其影响。

默认在回答中生成研究记录。要求保存时，可以指定目录；没有指定目录时，使用当前工作目录中的 `macro-research-notes/`。

## 文件说明

- [SKILL.md](SKILL.md)：触发说明、研究流程与完成检查。
- [references/research-record.md](references/research-record.md)：研究记录与后续复查模板。
- [agents/openai.yaml](agents/openai.yaml)：Codex 中显示的技能名称与调用提示。

## 研究要求

关键事实附带直接来源，区分已核验事实、因果推断和待验证假设。历史案例说明日期、比较窗口与适用限制。交易想法对应情景、成本、风险和退出条件；仓位计算需要资金规模、风险预算和工具参数。
