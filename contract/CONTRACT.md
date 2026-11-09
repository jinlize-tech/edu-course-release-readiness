# 输入输出契约

## 输入字段

| 键 | 名称 | 类型 | 必填 |
|---|---|---|---|
| `course_version` | 课程版本 | string | 是 |
| `learning_objectives` | 学习目标 | array | 是 |
| `syllabus` | 课程大纲 | string | 是 |
| `materials` | 课件与练习材料 | array | 是 |
| `assessments` | 测评与答案 | array | 是 |
| `teacher_training` | 教师培训准备 | string | 是 |
| `system_configuration` | 系统配置 | string | 否 |
| `pricing_contracts` | 价格与合同 | string | 是 |
| `marketing_assets` | 营销素材 | array | 是 |
| `launch_date` | 计划上线日期 | string | 是 |

## 状态

- `completed`：核心成果完整，关键结论人工确认要求满足。
- `completed_with_limits`：至少一项实质成果，说明限制、已完成和受阻范围。
- `needs_input`：必填字段缺失。
- `needs_confirmation`：资料冲突或人工确认未完成。
- `failed`：计算或工具失败。

## 输出

- `发布就绪报告`：结构化条目数组，不允许空壳或占位文本。
- `阻断项`：结构化条目数组，不允许空壳或占位文本。
- `证据清单`：结构化条目数组，不允许空壳或占位文本。
- `责任人`：结构化条目数组，不允许空壳或占位文本。
- `回退方案`：结构化条目数组，不允许空壳或占位文本。
- `上线批准单`：结构化条目数组，不允许空壳或占位文本。

完整机器契约见`contract/input.schema.json`、`contract/output.schema.json`和`contract/runtime_contract.json`。
