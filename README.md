# 袁逢春简历

本目录只保留**一版简历**：[index.html](index.html)，A4 三页，直接作为 GitHub Pages 首页。

对应 PDF：`袁逢春-Node.js-Agent后端工程师-2026.11.pdf`（2026.11 版，随本次项目更新重新生成）。

## 结构

- 头部：姓名、岗位、**求职意向（期望岗位 / 期望城市：苏州、上海、杭州、扬州）**、联系方式
- 核心能力：Node.js 后端 / AI Agent / 任务与事件流 / 数据与一致性 / 异步与集成 / 交付与稳定性
- 工作经历：启信宝核心服务、Express → NestJS 迁移、128 亿次稳定性治理、数据导出服务、CI/CD
- 项目经历：每个项目按「项目简介 / 技术栈 / 个人职责 / 项目业绩」展开
  - agent-v8：NestJS 网关 + Agent Worker 服务框架（个人项目，生产化设计已落地：MySQL 事件日志 / 队列 / 账本 / 故障接管，附自检与压测数据）
  - ai-coding：Claude Code 风格 Agent 内核与服务化（个人项目）
  - 数据导出服务：统一导出管线重构（工作项目，主导重构）
  - bug-track：NestJS + gRPC 双栈微服务（个人项目）
- 个人优势、教育背景

## 重新生成 PDF

```powershell
# 本机用 Edge（Chrome 同理）
& "C:\Program Files (x86)\Microsoft\Edge\Application\msedge.exe" `
  --headless=new --disable-gpu --no-pdf-header-footer `
  --print-to-pdf="袁逢春-Node.js-Agent后端工程师-2026.11.pdf" `
  "file:///D:/YWJL/project/About/index.html"
```

打印样式来自 `resume.css` 的 `@media print`：A4、页边距 11mm/13mm，`项目经历` 前强制分页，单个项目不跨页。

## 内容口径

- `agent-v8` 已按生产化标准落地：MySQL 单一事实源（事件日志 / 队列 / checkpoint / 账本）、会话分区队列、粘性路由、故障接管；
  项目业绩里的数字来自本地自检（51 项端到端 + 50 项数据层）与压测，个人项目不计入线上经历。
- 数据导出服务只声称主导统一导出管线重构；消费与通知链路用“重构中统一”表述，不额外夸大独立负责范围。
- `ai-coding`、`bug-track` 是个人项目，均已在标题处标注。
- 早期两版简历（`backend.html`、`agent-platform.html`）已删除；目录中 11 月 13 日生成的旧 PDF 未动，
  内容早于本次项目更新，如需使用请按上面的命令重新生成。
