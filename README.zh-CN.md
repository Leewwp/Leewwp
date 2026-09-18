<div align="center">

[![English](https://img.shields.io/badge/English-d0d7de?style=flat-square)](README.md)
[![简体中文](https://img.shields.io/badge/简体中文-2f81f7?style=flat-square)](README.zh-CN.md)

# 李伟培 · Leewwp

**后端工程师 —— Go & Java。** 我做大模型应用里那些必须在上线环境扛住的部分：
检索质量、Agent 编排、失败降级、可观测性，以及安全边界。

<sub>坐标香港</sub>

</div>

---

## 关注方向

| 方向 | 具体在做什么 |
| --- | --- |
| **检索与 RAG** | pgvector / Elasticsearch / Qdrant 混合检索 · 引用溯源 · 可见性过滤 · 后端不可用时的可降级链路 |
| **Agent 工程** | 工具编排 · MCP 服务端与客户端 · Prompt 生命周期与版本管理 · 结构化输出契约 |
| **生产加固** | 全链路追踪 · LLM 成本核算 · 租户与权限边界 · CI 质量门禁 |

## 主要项目

**[OmniCraft（万象工坊）](https://github.com/Leewwp/OmniCraft)** · Go · Next.js · PostgreSQL/pgvector · Redis Streams
内容分享平台，核心是服务端收口的单 Agent RAG 工作台：引用复核、可见性过滤、可降级混合检索、Transactional Outbox 异步链路。带离线评测、安全门禁与全链路追踪。

**[polyu-agent](https://github.com/Leewwp/polyu-agent)** · Spring Boot 3 · pgvector / Elasticsearch · React · [polyuguide.com](https://polyuguide.com)
面向理大校园信息的双语问答 Agent（非官方）。分域知识库、引用溯源、定时资讯刷新，落在一条确定性抓取链路上。

**[health_agent](https://github.com/Leewwp/health_agent)** · Java · Spring Boot
三品类统一健康助手。以显式状态机驱动的多角色确定性工作流编排、契约化降级、混合检索 RAG、MCP 服务端能力，配套 900+ 自动化测试。

**[ppp-rpc](https://github.com/Leewwp/ppp-rpc)** · Java · Netty · ZooKeeper
从协议层写起的轻量 RPC 框架：Netty 传输、ZooKeeper 注册发现、三种负载均衡策略、重试机制。

<details>
<summary><b>其他项目</b></summary>

- **[jewel-ar-tryon](https://github.com/Leewwp/jewel-ar-tryon)** —— 微信小程序 AR 首饰试戴技术 PoC。
- **[Proactive-Diet-Shopping-Assistant](https://github.com/Leewwp/Proactive-Diet-Shopping-Assistant)** —— Expo / React Native 智能购物助手：条码与视觉识别、过敏原冲突检测、购物车营养合规评分。
- **[ADA_Project](https://github.com/Leewwp/ADA_Project)** —— 香港空气质量短期预测：多变量时序 ETL、特征工程、多模型对比（Open-Meteo API）。
- **[ppp-blog](https://github.com/Leewwp/ppp-blog)** —— Halo 2.x 博客系统：Docker Compose 部署、GitHub Actions CI/CD、监控告警。

</details>

## 开源贡献

给我自己在用的项目提的改动：

- **[docling-project/docling-core #766](https://github.com/docling-project/docling-core/pull/766)** —— Markdown 表格序列化：行头行不再误入表头块。
- **[elastic/beats #53159](https://github.com/elastic/beats/pull/53159)** —— filebeat / winlogbeat 面向用户的报错文案修正。
- **[nageoffer/ragent #131](https://github.com/nageoffer/ragent/pull/131) [#132](https://github.com/nageoffer/ragent/pull/132) [#133](https://github.com/nageoffer/ragent/pull/133) [#136](https://github.com/nageoffer/ragent/pull/136)** —— 文档抓取链路加固（出站校验、响应体积上限、错误体不回显）、上传端点限流、解析器模块清理，以及 trace 场景测试的 CI 偶发失败修复。

## 技术栈

- **语言** —— Go · Java · TypeScript · Python
- **后端** —— Spring Boot 3 · Gin · Netty
- **LLM / Agent** —— RAG（pgvector · Elasticsearch · Qdrant）· Agent 编排 · MCP · DashScope / MiniMax / DeepSeek
- **数据** —— PostgreSQL · MySQL · Redis / Redis Streams
- **前端** —— Next.js / React · React Native
- **工程化** —— Docker · GitHub Actions · OpenTelemetry

## 联系方式

- **线上产品** —— [polyuguide.com](https://polyuguide.com)

<div align="center">
<sub>欢迎交流 Agent 工程、检索质量与生产环境的大模型基础设施。</sub>
</div>
