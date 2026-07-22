# Andy Investment Skill - 项目架构

## 投资系列项目关系图

### 核心定位

Andy Investment Skill 是投资决策的**统一入口和方法论中枢**，不是所有投资工具的代码集合。

各子项目保持独立仓库、独立传播能力，但在理念和工作流上形成协同。

---

## 项目分层

### 1. 核心中枢层 (Core Hub)

**ai-invest-agent** ⭐ 20-49 Stars
- 角色：投资记录、组合管理与复盘中枢
- 功能：交易记录、收益归因、投资复盘、风险评估、个股分析
- 状态：已验证，保持独立
- 链接：https://github.com/AIPMAndy/ai-invest-agent

---

### 2. 策略执行层 (Strategy Execution)

#### 长期投资体系
**changying-index-fund-skill**
- 角色：长期指数投资与资产配置
- 功能：指数基金选择、资产配置策略、再平衡纪律
- 理念：长期主义、低成本、分散风险
- 链接：https://github.com/AIPMAndy/changying-index-fund-skill

#### 短线交易体系
**youzi-trading-skill** ⭐ 10-19 Stars (v2.0)
- 角色：A股短线交易纪律系统
- 功能：输入契约、硬规则、风险优先、市场环境判断
- 理念：纪律第一、情绪隔离、止损严格
- 链接：https://github.com/AIPMAndy/youzi-trading-skill

---

### 3. 规划目标层 (Planning & Goals)

**FIREClaw**
- 角色：财务自由规划工具
- 功能：FIRE 目标设定、资产增长预测、支出优化
- 理念：长期财务目标管理
- 链接：https://github.com/AIPMAndy/FIREClaw

---

### 4. 情报研究层 (Intelligence & Research)

**andy-follows (Investment Module)**
- 角色：AI 产业与市场情报
- 功能：AI 产业趋势、资本流向、市场情绪、投资机会发现
- 理念：信息优势、趋势识别
- 链接：https://github.com/AIPMAndy/andy-follows

---

## 工作流整合

```
情报层: andy-follows
    ↓ 发现机会
    
策略层: changying (长期) + youzi (短线)
    ↓ 制定计划
    
执行层: 实际交易
    ↓ 记录追踪
    
中枢层: ai-invest-agent
    ↓ 复盘分析
    
优化层: 识别模式 → 改进纪律
    ↓
    
目标层: FIREClaw
    ↓ 进度追踪
    
循环: 反馈 → 情报层
```

---

## 设计原则

### 1. 各司其职，不做合并
- ai-invest-agent：记录与复盘
- changying：长期配置
- youzi：短线纪律
- FIREClaw：财务规划
- andy-follows：市场情报

**每个项目解决不同问题**，强行合并会损失独立传播价值。

### 2. 保持独立仓库
- 已验证项目（有 Star、有用户反馈）必须保持独立
- 独立 README 便于单点传播
- 独立版本管理避免耦合风险

### 3. 统一理念表达
- 所有项目在 README 中标注"属于 Andy Investment Series"
- 链接回 andy-invest-skill 作为导航中枢
- 强调"研究、复盘、风险控制、投资教育"，避免荐股机器人印象

### 4. 商业定位清晰
- 公开项目：教育、工具、方法论
- 避免：具体买卖信号、无条件推荐、保证收益承诺
- 强调：风险自负、人类决策、AI 辅助

---

## 未来扩展方向

### 可能增加的模块
- 投资日志系统（投资决策记录与回顾）
- 风险压力测试（组合在极端情况下的表现）
- 投资心理追踪（情绪日志与纪律检查）
- 市场周期判断（宏观环境与资产轮动）

### 不应增加的功能
- 自动交易执行（违背"人类决策"原则）
- 实时荐股推送（监管风险 + 责任风险）
- 付费订阅信号（商业模式风险）
- 社区跟单功能（法律合规风险）

---

## 与其他两条主线的关系

### Andy Product Skill
- 投资系列本身是产品能力的体现
- 产品方法论指导投资工具的设计
- 用户反馈验证产品决策框架

### Andy IP Skill
- 投资复盘内容可作为 IP 素材
- IP 传播带来用户和反馈
- 商业转化可能在培训、陪跑、咨询

### 商业飞轮
```
Product (做出投资工具)
    ↓
Investment (验证判断能力)
    ↓
IP (放大影响力)
    ↓
收入、数据、反馈
    ↓
Product (改进工具)
```

---

## Star 数据参考 (截至 2026-07)

| 项目 | Star 区间 | 状态 |
|------|----------|------|
| ai-invest-agent | 20-49 | 已验证核心资产 |
| youzi-trading-skill | 10-19 | 已进入 v2.0 |
| changying-index-fund-skill | < 10 | 持续迭代 |
| FIREClaw | < 10 | 功能完整 |
| andy-follows | 包含投资模块 | 多功能项目 |

---

## 维护策略

### 高优先级
- ai-invest-agent：保持功能更新，响应用户反馈
- youzi-trading-skill：持续优化纪律规则

### 中优先级
- changying-index-fund-skill：补充长期投资案例
- FIREClaw：增加财务规划模板

### 低优先级
- andy-follows 投资模块：作为情报输入端，按需更新

---

## 总结

andy-invest-skill 不是"所有投资代码的大仓库"，而是：
1. **统一品牌入口** - 对外展示投资系列全貌
2. **方法论中枢** - 说明各项目如何协同工作
3. **理念传播平台** - 强调研究、纪律、复盘、风险控制
4. **导航路由系统** - 帮助用户找到适合自己的工具

各子项目保持独立，通过 README 交叉引用形成生态。
