# CHANGELOG

## [Unreleased]

### 新增

- 注册子模块：`docs/handbook`（软件工程工作手册，quanttide-handbook-of-software-engineering）
- 注册子模块：`data/profile`（软件工程档案，quanttide-profile-of-software-engineering）
- 注册子模块：`docs/bylaw`（软件工程章程，quanttide-bylaw-of-software-engineering）
- 注册子模块：`apps/qtcode`（量潮代码中心，qtcode）
- 注册子模块：`packages/quanttide-code-toolkit`（软件工程工具箱，quanttide-code-toolkit）
- 注册子模块：`data/intention`（软件工程意图，quanttide-intention-of-software-engineering）
- 注册子模块：`data/roadmap`（软件工程路线图，quanttide-roadmap-of-software-engineering）
- 注册子模块：`data/insight`（软件工程洞察，quanttide-insight-of-software-engineering）
- 注册子模块：`data/brochure`（软件工程宣传册，quanttide-brochure-of-software-engineering）
- 注册子模块：`data/library`（软件工程参考，quanttide-library-of-software-engineering）
- 注册子模块：`data/history`（软件工程历史，quanttide-history-of-software-engineering）
- 注册子模块：`data/archive`（软件工程归档，quanttide-archive-of-software-engineering）
- 注册子模块：`docs/specification`（软件工程标准，quanttide-specification-of-software-engineering）
- 注册子模块：`docs/tutorial`（软件工程教程，quanttide-tutorial-of-software-engineering）
- 注册子模块：`docs/essay`（软件工程札记，quanttide-essay-of-software-engineering）
- 注册子模块：`docs/gallery`（软件工程案例集，quanttide-gallery-of-software-engineering）
- README.md：新增子模块一览表

## [0.1.1] - 2026-05-25

### 仓库维护

- 新建子模块 `docs/report` — `quanttide-report-of-software-engineering`
- `examples/default` 同步远程最新变更
- `apps/qtcloud-code` 子模块 Cargo.toml repository URL 修复为 `qtcloud-code.git`
- `qtcloud-devops` 更新至 v0.4.3

---

## [0.1.0] - 2026-05-25

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
