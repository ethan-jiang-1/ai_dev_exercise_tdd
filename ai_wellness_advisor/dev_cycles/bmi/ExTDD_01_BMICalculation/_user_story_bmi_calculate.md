# 用户故事：BMI 值计算 (ExTDD_01_BMICalculation)

**特性名称**: `bmi_calculate`
**模块名称**: `bmi`
**TDD周期**: ExTDD_01_BMICalculation

## 1. 用户故事

> 作为一名普通用户，我希望能方便地输入我的身高（以米为单位）和体重（以千克为单位），然后系统能帮我算出我的身体质量指数（BMI）。如果我输错了数字（比如不是有效的身高体重值），希望能得到一个友好的提示。我最主要就是想知道计算出来的BMI结果。

## 2. 验收标准 (Acceptance Criteria)

*   **AC1**: 当用户提供有效的身高（正数，单位：米）和体重（正数，单位：千克）时，系统应能正确计算BMI值。BMI 计算公式为：`体重（kg） / (身高（m）^ 2)`。
*   **AC2**: 计算结果应四舍五入到小数点后两位。
*   **AC3**: 如果用户输入的身高不是一个有效的正数（例如，零、负数、非数字），系统应返回一个明确的错误提示，例如：“身高必须是有效的正数”。
*   **AC4**: 如果用户输入的体重不是一个有效的正数（例如，零、负数、非数字），系统应返回一个明确的错误提示，例如：“体重必须是有效的正数”。
*   **AC5**: 如果同时输入了无效的身高和体重，系统应能针对两者都给出提示，或者按特定优先级给出提示（例如，优先提示身高无效）。（此处的具体行为可在设计阶段进一步明确）
*   **AC6**: 成功计算后，系统应清晰地展示计算出的BMI值。

## 3. 备注与约束

*   身高单位固定为米（m）。
*   体重单位固定为千克（kg）。
*   错误提示信息应友好且易于理解。
*   此特性仅关注BMI值的计算和基本输入验证，不涉及BMI分类。