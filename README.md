# AI 协作协议 (AI Collaboration Protocol)

> 一套轻量、可复用的 AI 协作规范模板，解决多 AI 协同中的**上下文失忆、标准不一致、成本不可控**三大痛点。
>
> 从 IAIBench 工业级项目实践中提炼，适用于任何有多个 AI agent 参与的项目。

---

## 📦 包含什么

```
ai-collab-protocol/
├── AI_ENTRY.md          ← AI 入口文件（告诉新 AI 怎么读项目）
├── DECISIONS.md         ← 设计决策记录（记录每个决策的"为什么"）
├── COLLAB.md            ← 协作规范（SoT、变更流程、验收标准、成本确认）
├── SESSION_HANDOFF.md   ← 会话交接（跨机器/跨 AI 接力时记录当前状态）
├── ROLLOUT_PLAN.md      ← 四步推广方案
├── FEISHU_SHARE.md      ← 飞书分享卡片
├── .gitignore
├── examples/
│   └── sanitized/        ← 脱敏的格式示例（占位内容，不涉及真实项目）
└── skill/
    └── install-ai-collab-rules.md  ← Reasonix 技能包
```

## 🚀 快速开始

```bash
# 1. 克隆或复制本仓库到你的项目
cp -r ai-collab-protocol/* your-project/

# 2. 按实际项目填空（替换 【占位符】 内容）
#    核心改动点：项目名、技术栈、目录结构、SoT 位置

# 3. 在 README.md 顶部加一行
#   > 任何 AI 在改动本仓库前，必须先读 AI_ENTRY.md

# 4. 写前 3 条决策记录作为"气候设定"
```

如果你在用 Reasonix（AI 协作平台），一行命令即可：

```bash
/install-ai-collab-rules <项目名>
```

## 🧠 核心理念

### 四个文件解决四个问题

| 文件 | 解决什么问题 | 类比 |
|---|---|---|
| `AI_ENTRY.md` | 新 AI 接入后不知从哪读起 | AI 版的 README |
| `DECISIONS.md` | 后来者不理解"为什么现在是这样的" | CHANGELOG 的决策版 |
| `COLLAB.md` | 多 AI 各自为政、标准不一致 | AI 版的 eslint 规则集 |
| `SESSION_HANDOFF.md` | 换机器/换人后对话上下文断了 | AI 对话的 git commit |

### 四条不可违反的铁律

1. **📝 文档留痕** — 任何设计决策都要记录理由
2. **💰 成本确认** — 任何付费/外部 API 动作必须先停下说明开销
3. **🎯 SoT 一致** — 改标准必同步决策记录和下游实现
4. **🔄 会话交接** — 收工前写 SESSION_HANDOFF.md 并提交到 Git

## 📖 使用场景

- **新项目启动** — 初始化时直接复制模板，建立 AI 协作基线
- **老项目改造** — 补上 AI_ENTRY.md 和 DECISIONS.md，对齐上下文
- **多机器开发** — 配合 SESSION_HANDOFF.md 实现跨机器 AI 对话无缝接力
- **团队标准化** — 统一所有项目的 AI 协作规范，减少沟通成本

## 🤝 贡献

欢迎提交 PR 改进模板！保持三个原则：
- 通用性：不绑定具体语言/框架/工具
- 轻量：每个文件尽量控制在 100 行以内
- 可操作：每条规则都是可检查的

## 🔗 仓库

https://github.com/feather100/ai-collab-patterns

## 📄 许可证

MIT - 随意使用、修改、分发
