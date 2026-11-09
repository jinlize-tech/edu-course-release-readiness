# 课程版本发布检查示例

## 典型场景

新版数学课更换了试卷，但教师培训仍引用旧评分标准。

## 具体示例

系统将评分标准不一致标为阻断项，要求同步培训和答案材料后才可放行。

## 脱敏输入示例

```json
{
  "contract_version": "1.2.0",
  "data_status": "confirmed",
  "contains_sensitive_data": false,
  "requested_output_language": "zh-CN",
  "course_version": "课程版本已核对（脱敏示例）",
  "learning_objectives": [
    {}
  ],
  "syllabus": "课程大纲已核对（脱敏示例）",
  "materials": [
    {}
  ],
  "assessments": [
    {}
  ],
  "teacher_training": "教师培训准备已核对（脱敏示例）",
  "system_configuration": "系统配置已核对（脱敏示例）",
  "pricing_contracts": "价格与合同已核对（脱敏示例）",
  "marketing_assets": [
    {}
  ],
  "launch_date": "2026-11-10"
}
```

## 预期处理

1. 运行输入契约校验。
2. 逐项核对输入来源、版本和口径。
3. 按`references/PROFESSIONAL_PLAYBOOK.md`完成专业分析。
4. 输出发布就绪报告、阻断项、上线批准单等核心成果。
5. 由业务负责人确认输入事实、关键假设和最终成果适用范围后才可作为正式业务结论。

## 不应出现的输出

- 虚构政策、价格、人员、课程或客户事实。
- 以“暂无”“待完善”等占位文本冒充完成。
- 无依据的确定性判断或伪造人工签批。
