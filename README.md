### 你好，我是 Li Weipei

PolyU MSc in IT 在读，坐标香港。写 Java 和 Go，主要做 LLM 应用与 Agent 工程化，关心的是让大模型在真实系统里可靠干活的问题：检索质量、失败降级、可观测性、安全边界。平时维护自己的开源项目，也给我在用的开源项目提 PR。

#### 技术栈

- **语言**：Java / Go / TypeScript / Python
- **后端**：Spring Boot 3 · Gin
- **LLM 应用**：RAG（pgvector / Elasticsearch / Qdrant）· Agent 编排 · MCP · DashScope / MiniMax / DeepSeek
- **数据与中间件**：PostgreSQL · MySQL · Redis / Redis Streams
- **前端**：Next.js / React · React Native
- **工程化**：Docker · GitHub Actions CI/CD · OpenTelemetry

#### 主要项目

**[OmniCraft（万象工坊）](https://github.com/Leewwp/OmniCraft)** — IP 二创内容社区平台，核心是服务端收口的单 Agent RAG 工作台：引用复核、可见性过滤、可降级混合检索、Transactional Outbox 异步链路。Go + Next.js + PostgreSQL/pgvector + Redis Streams，带离线评测、安全门禁和全链路追踪。

**[polyu-agent](https://github.com/Leewwp/polyu-agent)** — 香港理工校园信息问答 Agent（非官方，线上 [polyuguide.com](https://polyuguide.com)），基于 [nageoffer/ragent](https://github.com/nageoffer/ragent) 二次开发：分域知识库、引用溯源、定时资讯更新、中英双语问答。Spring Boot 3 + pgvector/Elasticsearch + React。

#### 开源贡献

- **[docling-project/docling-core #766](https://github.com/docling-project/docling-core/pull/766)**（已合并）— 修复 Markdown 表格序列化时行头误入表头的问题
- **[elastic/beats #53159](https://github.com/elastic/beats/pull/53159)** — filebeat / winlogbeat 面向用户的报错文案修正
- **[nageoffer/ragent](https://github.com/nageoffer/ragent/pulls?q=is%3Apr+is%3Aopen+author%3ALeewwp) #131 #132 #133 #136** — 文档抓取链路出站校验与响应上限、上传端点限流、解析器加固、CI 偶发失败修复
