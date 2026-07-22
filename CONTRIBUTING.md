# Contributing to Andy Investment Skill

## 欢迎贡献

感谢你对 Andy Investment Skill 的关注。这是一个个人投资决策支持系统，旨在帮助投资者建立纪律、控制风险、复盘改进。

---

## 贡献原则

### ✅ 欢迎的贡献

1. **Bug 修复**
   - 工具功能错误
   - 文档错误或不清晰的说明
   - 计算逻辑问题

2. **功能改进**
   - 更好的数据可视化
   - 更清晰的风险提示
   - 更完善的复盘分析框架

3. **教育内容**
   - 投资方法论补充
   - 风险控制案例
   - 复盘思路分享

4. **工具集成**
   - 与券商 API 的标准化对接
   - 数据导入/导出格式支持
   - 与现有投资工具的兼容性

### ❌ 不接受的贡献

1. **具体股票推荐**
   - "买入 XX 股票"功能
   - 自动荐股系统
   - 保证收益的承诺

2. **自动交易执行**
   - 无人工确认的自动下单
   - 跟单系统
   - 算法交易策略（除非明确用于教育目的）

3. **监管灰色地带**
   - 规避监管的功能
   - 未经授权的数据爬取
   - 违反证券法规的工具

4. **过度复杂化**
   - 不必要的抽象层
   - 过度工程化的框架
   - 与核心目标无关的功能

---

## 贡献流程

### 1. 讨论 (Discussion First)

在开始编码前，请先：
- 在相关子项目的 Issues 中描述你的想法
- 说明为什么这个改进有价值
- 等待维护者反馈

**避免**：直接提交大型 PR 而不事先讨论

### 2. Fork & Branch

```bash
# Fork the repository on GitHub
# Clone your fork
git clone https://github.com/YOUR_USERNAME/PROJECT_NAME.git
cd PROJECT_NAME

# Create a feature branch
git checkout -b feature/your-feature-name
```

### 3. 开发 & 测试

- 遵循项目现有代码风格
- 添加必要的注释（英文）
- 确保功能可验证
- 更新相关文档

### 4. 提交 PR

```bash
git add .
git commit -m "feat: add feature description"
git push origin feature/your-feature-name
```

在 GitHub 上创建 Pull Request，并：
- 清楚描述改动内容
- 说明测试方法
- 链接相关 Issue

---

## 代码规范

### 通用原则

1. **简洁优于复杂** - 能用 10 行实现不要写 100 行
2. **可读优于聪明** - 让下一个维护者能快速理解
3. **安全优于便利** - 涉及资金数据时谨慎处理

### 命名规范

- 变量/函数：`camelCase`
- 常量：`UPPER_SNAKE_CASE`
- 类型/接口：`PascalCase`
- 文件名：`kebab-case.ts`

### 注释规范

```typescript
// Good: Explain WHY, not WHAT
// Cap position at 20% to prevent over-concentration risk
const maxPositionSize = portfolioValue * 0.2;

// Bad: Redundant comment
// Set max position size to 20% of portfolio
const maxPositionSize = portfolioValue * 0.2;
```

---

## 安全与隐私

### 必须遵守

1. **不提交敏感数据**
   - 个人交易记录
   - API 密钥
   - 账户信息

2. **数据仅本地存储**
   - 投资数据默认不上传云端
   - 如需云存储，必须加密且用户明确同意

3. **API 调用透明**
   - 明确告知用户哪些数据会发送到外部服务
   - 提供本地处理选项

---

## 文档要求

### README 更新

如果你的改动影响用户使用方式，需要更新：
- README.md 的相关章节
- 必要时补充示例

### CHANGELOG

在 `CHANGELOG.md` 中记录改动（如果项目有此文件）：
```markdown
## [Unreleased]
### Added
- New risk analysis feature (#123)

### Fixed
- Incorrect return calculation (#124)
```

---

## 测试要求

### 功能验证

- 关键计算逻辑需要测试用例
- 数据导入/导出需要验证正确性
- 风险提示需要覆盖边界情况

### 手动测试清单

提交 PR 前请确认：
- [ ] 功能在本地环境运行正常
- [ ] 没有引入新的错误或警告
- [ ] 文档已同步更新
- [ ] 敏感数据已移除

---

## 行为准则

### 尊重与包容

- 尊重不同的投资理念和风格
- 理性讨论技术方案
- 避免人身攻击和情绪化争论

### 诚实与透明

- 不夸大功能效果
- 如实报告测试结果
- 承认不确定性和局限性

### 责任与风险意识

- 记住这是投资决策工具，错误可能导致财务损失
- 在不确定时保守处理
- 优先考虑用户资金安全

---

## 法律合规

### 免责声明

所有贡献者需理解并同意：
1. 本项目不构成投资建议
2. 贡献者不对用户投资损失承担责任
3. 用户需自行判断并承担投资风险

### 开源协议

- 所有贡献自动采用 MIT License
- 贡献即表示你拥有代码版权或已获授权
- 不得提交侵权代码

---

## 子项目贡献指引

### ai-invest-agent
- 专注于组合管理和复盘分析
- 欢迎改进数据可视化和归因分析

### youzi-trading-skill
- 专注于短线交易纪律和风险控制
- 欢迎补充市场情绪指标和止损机制

### changying-index-fund-skill
- 专注于长期投资和资产配置
- 欢迎补充指数基金选择方法和再平衡策略

### FIREClaw
- 专注于财务自由规划
- 欢迎改进目标追踪和支出优化功能

---

## 联系方式

- GitHub Issues: 在各子项目仓库提 Issue
- 商业合作: 见 [andy-ip-skill](https://github.com/AIPMAndy/andy-ip-skill)

---

## 感谢

感谢每一位贡献者帮助完善这个投资决策系统。

记住：**好的投资工具让人更理性，而不是更冲动。**

Good investment tools make people more rational, not more impulsive.
