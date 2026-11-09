# 使用说明

## 适用任务

新版数学课更换了试卷，但教师培训仍引用旧评分标准。

## 准备输入

课程版本、目标与大纲、课件/练习/答案、教师培训、系统配置、价格/合同、营销物料、上线日期。使用前先脱敏姓名、联系方式和与任务无关的敏感信息。

## 操作步骤

1. 冻结版本范围
2. 核对产品契约
3. 检查内容与评估
4. 验证材料和培训
5. 检查系统与价格
6. 出放行/阻断结论

## 校验命令

```powershell
node scripts/validate_input.js examples/typical_input.json
node scripts/validate_output.js examples/typical_output.json
```

## 状态使用

- `completed`：核心成果完整。
- `completed_with_limits`：只完成可验证部分，并说明受阻范围。
- `needs_input`：缺少关键输入。
- `needs_confirmation`：资料冲突或需人工确认。
- `failed`：工具或计算失败，提供恢复动作。

## 人工确认

业务负责人复核输入事实、关键假设和最终成果适用范围后，成果才可进入正式业务使用。
