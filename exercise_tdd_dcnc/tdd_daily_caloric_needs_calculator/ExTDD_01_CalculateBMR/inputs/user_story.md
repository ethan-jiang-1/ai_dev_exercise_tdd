# 用户故事：基础代谢率(BMR)计算器

## 背景
作为一个关注健康的用户，我需要知道自己的基础代谢率（BMR），这样我可以更好地规划我的饮食和运动计划。基础代谢率是指人体在完全静息状态下，维持生命所需的最低能量消耗。

## 用户需求
作为普通用户，我希望：
1. 能够输入我的基本身体信息：
   - 性别（男/女）
   - 年龄
   - 身高（厘米）
   - 体重（公斤）
2. 系统能够根据我的输入信息，计算出我的基础代谢率（BMR）
3. 得到的结果以千卡(kcal)为单位，便于我理解和使用

## 验收标准
1. 必须支持输入以下信息：
   - 性别：必须是"男"或"女"
   - 年龄：必须是有效的正整数
   - 身高：必须是有效的正数，单位是厘米(cm)
   - 体重：必须是有效的正数，单位是公斤(kg)

2. 当输入无效数据时：
   - 系统应该给出清晰的错误提示
   - 错误提示应该指明具体是哪个输入有问题

3. 计算结果要求：
   - 结果必须是整数（四舍五入）
   - 单位必须是千卡(kcal)
   - 结果必须是正数

4. 使用场景示例：
   示例1：
   - 输入：男性，25岁，175cm，70kg
   - 预期：得到一个合理的BMR值（约1700-1900kcal）

   示例2：
   - 输入：女性，30岁，160cm，55kg
   - 预期：得到一个合理的BMR值（约1200-1400kcal） 