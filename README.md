# 袁逢春简历

本目录只保留**一版简历**：[index.html](index.html)，A4 三页，直接作为 GitHub Pages 首页。

对应 PDF：`袁逢春-Node.js-Agent后端工程师-2026.11.pdf`（2026.11 版，随本次项目更新重新生成）。

## 结构

- 头部：姓名、岗位、**求职意向（期望岗位 / 期望城市：苏州、上海、杭州、扬州）**、联系方式
- 核心能力：Node.js 后端 / AI Agent / 任务与事件流 / 数据与一致性 / 异步与集成 / 交付与稳定性
- 工作经历：上海生腾（2021.06 - 2026.07，启信宝核心服务 / NestJS 迁移 / 128 亿次稳定性治理 / 数据导出 / CI/CD）、上海燮贤（高级全栈工程师，2026.09 - 2026.11，Apollo 多租户 SaaS）
- 项目经历：按时间从早到晚排列，每个项目按「项目简介 / 技术栈 / 个人职责 / 项目业绩」展开
  - 数据导出服务：统一导出管线重构（工作项目，主导重构）
  - bug-track：面向多租户 SaaS 的 Bug 管理系统（NestJS + gRPC，MySQL 多租户 + 文件服务持久化；2026.09 - 2026.11）
  - ai-coding：Claude Code 风格 Agent 内核与服务化（个人项目，2026.09.01 - 2026.09.30）
  - agent-v8：NestJS 网关 + Agent Worker 服务框架（个人项目，2026.10.09 - 至今；生产化已落地：MySQL 事件日志 / 队列 / 账本 / 故障接管，附自检与压测数据）
- 个人优势、教育背景

## 重新生成 PDF

```powershell
# 本机用 Edge（Chrome 同理）
& "C:\Program Files (x86)\Microsoft\Edge\Application\msedge.exe" `
  --headless=new --disable-gpu --no-pdf-header-footer `
  --print-to-pdf="袁逢春-Node.js-Agent后端工程师-2026.11.pdf" `
  "file:///D:/YWJL/project/About/index.html"
```

打印样式来自 `resume.css` 的 `@media print`：A4、页边距 11mm/13mm，`项目经历` 前强制分页；项目块允许跨页承接，避免 4 个项目被挤成 4 页。

## 内容口径

- `agent-v8` 已按生产化标准落地：MySQL 单一事实源（事件日志 / 队列 / checkpoint / 账本）、会话分区队列、粘性路由、故障接管；
  项目业绩里的数字来自本地自检（51 项端到端 + 50 项数据层）与压测，个人项目不计入线上经历。
- 数据导出服务只声称主导统一导出管线重构；消费与通知链路用“重构中统一”表述，不额外夸大独立负责范围。
- 工作经历按时间正序：上海生腾 2021.06 - 2026.07（后端开发工程师）；上海燮贤 2026.09 - 2026.11（高级全栈工程师，职责按 JD 总结为 Apollo 多租户 SaaS、NestJS/React、MySQL/Redis、RBAC 与 AI 辅助研发；RabbitMQ 未接触，不写入简历）。
- `ai-coding`、`agent-v8` 是个人项目，均已在标题处标注；`bug-track` 按工作项目展示（2026.09 - 2026.11，多租户 MySQL + 文件服务持久化）。
- 早期两版简历（`backend.html`、`agent-platform.html`）已删除；目录中 11 月 13 日生成的旧 PDF 未动，
  内容早于本次项目更新，如需使用请按上面的命令重新生成。
