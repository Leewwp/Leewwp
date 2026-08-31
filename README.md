### 你好，我是 Li Weipei 👋

**大模型应用 / Agent 工程方向 · 2026 校招**

PolyU MSc in IT。我在做一件事：把 LLM 塞进**确定性工程边界**里——模型只负责语义理解与受约束表达，候选、数值、风险、状态全部由代码掌控。两个工程级个人项目从 0→1 独立构建与维护：可复现评测、真实 provider 差分验证、无 API Key 也能跑完整演示。

---

#### 🔥 重点项目

| 项目 | 一句话 | 技术栈 | 工程证据 |
| --- | --- | --- | --- |
| [**OmniCraft（万象工坊）**](https://github.com/Leewwp/OmniCraft) | IP 二创内容社区：单 Agent RAG 工作台——服务端引用复核、可见性过滤、可降级混合检索、可靠异步 | Go 1.25 / Gin · Next.js 16 · PostgreSQL 16 + pgvector · Redis Streams · OTel/Jaeger | 冻结语料真实 MiniMax 差分评测（63 cases）：Recall@10 **0.492**、MRR **0.437**（keyword baseline 0.370）、0 visibility leak；前端 464 测试 + 全量验证门 73/73 |
| [**health-agent**](https://github.com/Leewwp/health_agent) | 三品类统一健康助手：Java 状态机确定性编排多角色工作流，契约化降级 + 混合检索 RAG + MCP 服务端 | Java 21 / Spring Boot 3 · AgentScope + DashScope · MySQL + Flyway · Qdrant · MCP Java SDK | **910** 个自动化测试（0 失败，53 个环境门控跳过）+ 前端 43 契约测试；60 条标注查询集驱动出两段式检索路由（P95 延迟降为 Hybrid 的 40%、硬约束零违规） |

<details>
<summary><strong>🎬 前作：diet 三部曲演进主线</strong></summary>

```text
Proactive-Diet-Shopping-Assistant   →   diet-agent   →   health-agent
条码扫描购物助手（Expo/RN）              多Agent状态机+Trace      契约化三品类健康助手
验证产品命题                            验证架构判断             工程化重写升级
```

- [Proactive-Diet-Shopping-Assistant](https://github.com/Leewwp/Proactive-Diet-Shopping-Assistant) — 条码 + 视觉识别 + 过敏原冲突检测 + 购物车营养合规评分
- diet-agent — AgentScope 多角色状态机 + 全链路 Trace + 离线评估（架构判断被 health-agent 继承）
</details>

<details>
<summary><strong>🧰 其他项目</strong></summary>

- [ppp-rpc](https://github.com/Leewwp/ppp-rpc) — 轻量 Java RPC 框架：Netty + ZooKeeper 注册发现 / 三种负载均衡 / 重试策略
- [jewel-ar-tryon](https://github.com/Leewwp/jewel-ar-tryon) — AR 首饰试戴微信小程序 PoC：VisionKit 追踪 + three.js 屏幕空间叠加
- [ADA_Project](https://github.com/Leewwp/ADA_Project) — 香港空气质量短期预测：多变量时序 ETL + 多模型对比
- [SimCLR](https://github.com/Leewwp/SimCLR) — 对比学习课程项目：自监督预训练 + 冻结 backbone 线性评估 + 双基线对照
</details>

---

#### 🧭 我关心的工程命题

- **LLM 作为不可靠依赖**：契约化调用、失败分类（六类）、确定性降级——对话永远有回复，下次请求不残留脏状态
- **RAG 的边界**：向量只管候选召回，过敏原/权限等硬约束永远回查事实源二次校验；评测必须区分真实运行与降级运行，防止把降级误报成效果
- **Agent 的引用治理**：模型不能伪造引用——工具、citation DTO、可见性校验全部收口服务端，SSE 输出前复核
- **异步正确性**：Transactional Outbox + Inbox 幂等 + DLQ replay，明确 at-least-once，不吹 exactly-once
- **评测防自欺**：有效分母、语料 checksum 固化、单次运行不外推——「两轮实验不可比」的结论也是评测体系的产出

#### 🛠 技术栈

`Java` `Go` `Python` `TypeScript` · `Spring Boot 3` `Gin` · `AgentScope` `MCP` `DashScope/MiniMax` · `MySQL` `PostgreSQL/pgvector` `Qdrant` `Redis Streams` · `Next.js/React` `React Native` · `Docker` `GitHub Actions` `OpenTelemetry`

---

⭐ 如果我的项目对你有帮助，欢迎 Star；Issue 与讨论区永远开放，欢迎交流大模型应用与 Agent 工程化话题。
