---
name: xianyu-ecommerce-pack
description: |
  闲鱼电商副业全流程方法论包（蒸馏自《2026 年闲鱼电商副业保姆级教程》），含 10 个子技能：店铺搭建、选品、标题SEO、商品图、详情文案、定价利润、无货源代发、运营推流（含补单）、销售话术售后、订单盈亏管理。
  何时调用：用户提到闲鱼卖货、闲鱼开店、闲鱼副业、无货源、一件代发、闲鱼选品、闲鱼标题/主图/详情、闲鱼补单、闲鱼话术、闲鱼订单管理等任何闲鱼运营话题时。
  trigger 信号：闲鱼、出闲置、无货源、代发、想要数、擦亮、补单、静默单、爆单。
  不适用于：淘宝/拼多多/抖音等平台运营（仅闲鱼逻辑）、闲鱼账号申诉解封、二手回收估价。
  调用后先按「路由表」选择 1 个子技能执行，需要多环节时按旅程顺序组合。
source_book: 《2026 年闲鱼电商副业保姆级教程》 海底桃
tags: [xianyu, ecommerce, skill-pack]
---

# 闲鱼电商副业技能包（路由层）

本包由 cangjie-skill 流水线蒸馏自海底桃《2026 年闲鱼电商副业保姆级教程》，10 个子技能覆盖从开店到复盘的完整旅程。**本文件是路由层：先选子技能，再读对应的 SKILL.md 执行。**

## 路由表

| 用户情形 | 子技能 |
|---|---|
| 新号注册/账号设置/防限流/多开号/人设包装 | [xianyu-shop-setup](./xianyu-shop-setup/SKILL.md) |
| 卖什么/选品/测品/类目决策 | [xianyu-product-selection](./xianyu-product-selection/SKILL.md) |
| 标题怎么写/没曝光/搜索不到 | [xianyu-title-seo](./xianyu-title-seo/SKILL.md) |
| 主图/商品图/图源/修图/去重/标签 | [xianyu-product-images](./xianyu-product-images/SKILL.md) |
| 详情文案/文案结构/静默单 | [xianyu-listing-copy](./xianyu-listing-copy/SKILL.md) |
| 定价/毛利测算/低价引流SKU/发布城市 | [xianyu-pricing-profit](./xianyu-pricing-profit/SKILL.md) |
| 有人下单了/货源/1688下单/无痕发货/退货 | [xianyu-dropshipping](./xianyu-dropshipping/SKILL.md) |
| 没流量/冷启动/每日运营/补单 | [xianyu-growth-ops](./xianyu-growth-ops/SKILL.md) |
| 买家来问了/砍价/正品质疑/售后/差评 | [xianyu-sales-service](./xianyu-sales-service/SKILL.md) |
| 单多了乱/利润算不清/复盘/品去留 | [xianyu-order-dashboard](./xianyu-order-dashboard/SKILL.md) |

## 全局原则（所有子技能共享）

1. **选品是 1，运营是 0**——坏选品怎么运营都不出单，先质疑品再优化动作
2. **平台规则优先**——0.6% 手续费、30 字标题、堆砌判定等规则随时间变动，执行前先核对最新规则
3. **两条红线**——不做站外引流（话术红线，sales-service）；不卖有版权的虚拟资料，防钓鱼执法（选品红线，product-selection）
4. **补单是灰色操作**——涉及补单的输出必须附带风险声明（过度补单=限流）
5. **承诺可兑现**——话术/文案不写超出履约能力的承诺

## 旅程顺序（新手完整走一遍）

```
shop-setup → product-selection → title-seo + product-images + listing-copy + pricing-profit
           → dropshipping → growth-ops → sales-service → order-dashboard
```

## 审计信息

- 子技能 10/10 通过 validate_skill_pack.py（0 errors, 0 warnings）
- 触发测试用例：[test-prompts.json](./test-prompts.json)
- 源文本：完整抓取版留存本地工作区，未随仓库分发（版权考虑）
- 蒸馏时间：2026-10-04
