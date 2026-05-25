# CHANGELOG

## 0.1.1 (2026-05-25)

### 仓库维护

- 新建子模块 `docs/report` — `quanttide-report-of-software-engineering`
- `examples/default` 同步远程最新变更
- `apps/qtcloud-code` 子模块 Cargo.toml repository URL 修复为 `qtcloud-code.git`
- `qtcloud-devops` 更新至 v0.4.3

---

## v0.1.0 (2026-05-25)

### 项目初始化

- 新建仓库，配置 `apps/qtcloud-code` 和 `examples/default` 两个 git 子模块
- 添加 `README.md` 说明项目定位

### CodeAgent 架构（examples/default）

- 从线性流水线（Scan→Plan→Execute→Verify）重构为 Review→Reflect→Refactor 智能体循环
- 删除 `session.py`，拆分出 `agent.py` / `reviewer.py` / `reflector.py`
- 新增增量坏味道检测、无限循环保护、失败自动回滚
- `main.py` 支持命令行参数传入文件/目录路径，支持 `--help`

### 文档

- 用户指南 `docs/user-guide.md` + AI 集成指南 `docs/ai-integration.md`
- 更新 ROADMAP、CHANGELOG、TODO 与当前架构对齐

### 仓库维护

- `apps/qtcloud-code` 子模块 deinit（防止误操作）
- `examples/default` 远程仓库重命名为 `quanttide-laboratory-of-software-engineering`
- 首次正式发布 (`v0.1.0`)
