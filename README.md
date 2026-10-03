# 闲鱼电商副业技能包 (xianyu-ecommerce-pack)

> 10 个子技能覆盖闲鱼副业完整旅程：**开店 → 选品 → 链接制作 → 履约发货 → 运营推流 → 话术售后 → 订单复盘**
>
> 蒸馏自海底桃《2026 年闲鱼电商副业保姆级教程》（飞书知识库），由 [cangjie-skill](https://github.com/88lin/cangjie-skill) 方法论蒸馏流水线生成。

## 这是什么

一套可直接挂载到 Claude Code / AgentSkills 兼容环境的闲鱼运营技能包。每个子技能都是独立的方法论卡片，统一结构：

- **R** 原文（Reading）— 关键原文引用
- **I** 方法论骨架（Interpretation）— 提炼后的方法
- **A1** 应用示例 — 具体案例的输入/动作/产出
- **A2** 触发场景 — 何时激活、与相邻技能怎么区分
- **E** 可执行步骤 — 带完成标准和判停条件的操作清单
- **B** 边界 — 不适用场景、失败模式、原作者盲点

根目录 `SKILL.md` 是路由层：按用户情形自动分发到对应子技能，也可按旅程顺序组合调用。

## 技能清单

| 技能 | 管什么 | 核心方法 |
|---|---|---|
| `xianyu-shop-setup` | 店铺基建 | 一机一卡一号一网防限流 + 专业卖家人设四件套 |
| `xianyu-product-selection` | 选品 | 同行的选品就是我的选品 + 3 天 10 单测品漏斗 |
| `xianyu-title-seo` | 标题 | 产品词+关联词+辅助词组合，前缀词定点击 |
| `xianyu-product-images` | 商品图 | 9 图规划，实拍感 > 精修，合规图源 |
| `xianyu-listing-copy` | 详情文案 | 七段结构，低客单冲静默单 |
| `xianyu-pricing-profit` | 定价利润 | 真实净利公式（含 0.6% 手续费）+ 低价引流 SKU |
| `xianyu-dropshipping` | 履约代发 | 1688/拼多多一件代发 + 无痕发货 + 痕迹消除 |
| `xianyu-growth-ops` | 运营推流 | 每日运营四件套 + 补单体系（灰色操作，强制风险声明） |
| `xianyu-sales-service` | 话术售后 | 中高客单 Q&A 话术 + 售后三件套 + 两条红线 |
| `xianyu-order-dashboard` | 订单数据 | 出单表 8 字段 + 每周 SKU 盈亏/盈亏周表复盘 |

## 安装

```bash
# Claude Code
git clone https://github.com/88lin/xianyu-ecommerce-pack.git ~/.claude/skills/xianyu-ecommerce-pack

# 其他 AgentSkills 兼容环境：把本目录放进对应 skills 目录即可
```

## 质量验证（v1.0.1，2026-10-04）

| 检查项 | 结果 |
|---|---|
| validate_skill_pack.py（官方校验器） | 0 errors, 0 warnings |
| 结构完整性（模板六段 × 10 技能） | 10/10 |
| 内容覆盖度（源书关键概念） | 70/70 |
| 触发路由盲测（真实场景问题） | 10/10 |

## 目录结构

```
xianyu-ecommerce-pack/
├── SKILL.md            # 根路由（按用户情形分发）
├── INDEX.md            # 索引 + 快速路由 + 引用关系图
├── BOOK_OVERVIEW.md    # 整书理解（7 大论点 + 任务映射）
├── GLOSSARY.md         # 14 条术语词典（作者用法 vs 常识用法）
├── test-prompts.json   # 触发路由测试用例
└── xianyu-*/SKILL.md   # 10 个子技能
```

## 重要说明

- 本包是**个人学习用途的方法论蒸馏笔记**（含少量原文引用与出处署名）。完整源文本未随仓库分发——请支持原作者。
- 补单等属于平台灰色操作，相关技能的所有输出均强制附带风险声明，是否采用请自行判断。
- 方法论仅适用于闲鱼平台，不适用于淘宝/拼多多/抖音等。
- 平台规则（手续费、字数限制、判定阈值）随时间变动，执行前请核对最新规则。

## License

MIT
