# 课程版本发布检查

设置课程上线门禁，逐项检查内容、评估、材料、系统、培训、价格、版权和运营准备度。

## 适用用户

课程产品经理、教研负责人、质量审核员、运营负责人

## 主要输出

- 发布就绪报告
- 阻断项
- 证据清单
- 责任人
- 回退方案
- 上线批准单

## 安装

将包含`SKILL.md`的根目录导入支持的Skill环境。

本地验证：

```powershell
node scripts/validate_input.js examples/typical_input.json
node scripts/validate_output.js examples/typical_output.json
```

## 使用

1. 阅读`USAGE.md`。
2. 按`contract/input.schema.json`准备输入。
3. 调用产品或Agent完成专业处理。
4. 使用`scripts/validate_output.js`检查成果。
5. 高风险结论交由业务负责人确认。

## 边界

- 不使用外部收费API。
- 不依赖其他产品完成核心任务。
- 不自动执行正式审批、退款、人员处罚或系统变更。
- 客户可见内容不包含公司品牌推广或内部研发资料。

## 状态

- 版本：`1.0.0`
- 本地契约与自动化测试：见`test-results/`
- 生成式模型运行：`MODEL_RUNTIME_NOT_VERIFIED`
- WorkBuddy安装、调用、审核、上架：`NOT_EXECUTED`
- 安装包：`dist/edu-course-release-readiness-v1.0.0.zip`

## 许可证

Apache-2.0。详见`LICENSE`。
