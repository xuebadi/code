<p align="center">
  <a href="https://github.com/xuebadi/code">
    <picture>
      <source srcset="packages/console/app/src/asset/logo-ornate-dark.svg" media="(prefers-color-scheme: dark)">
      <source srcset="packages/console/app/src/asset/logo-ornate-light.svg" media="(prefers-color-scheme: light)">
      <img src="packages/console/app/src/asset/logo-ornate-light.svg" alt="学霸帝Code logo">
    </picture>
  </a>
</p>
<p align="center"><strong>中文 AI 编程助手 - 本地运行，数据安全</strong></p>
<p align="center">
  <a href="https://github.com/xuebadi/code/releases/latest"><img alt="GitHub release" src="https://img.shields.io/github/v/release/xuebadi/code?style=flat-square&label=最新版本" /></a>
  <a href="https://github.com/xuebadi/code/discussions"><img alt="Discussions" src="https://img.shields.io/github/discussions/xuebadi/code?style=flat-square" /></a>
  <a href="https://github.com/xuebadi/code/actions"><img alt="Build status" src="https://img.shields.io/github/actions/workflow/status/xuebadi/code/publish.yml?style=flat-square&branch=dev" /></a>
</p>

<p align="center">
  <a href="README.md">English</a> |
  <a href="README_CN.md">简体中文</a> |
  <a href="README.zh.md">详细中文</a>
</p>

[![学霸帝Code Terminal UI](packages/web/src/assets/lander/screenshot.png)](https://xuebadi-code.ai)

---

### 安装

```bash
# YOLO 风格一键安装
curl -fsSL https://xuebadi-code.ai/install | bash

# 包管理器安装
npm i -g opencode-ai@latest        # 或 bun/pnpm/yarn
scoop install opencode             # Windows
choco install opencode             # Windows
brew install anomalyco/tap/opencode # macOS 和 Linux (推荐，始终最新)
```

> [!TIP]
> 安装前请先卸载 0.1.x 之前的旧版本。

### 桌面应用 (BETA)

学霸帝Code 提供桌面版应用。直接从 [发布页面](https://github.com/xuebadi/code/releases) 下载。

| 平台                  | 下载文件                           |
| --------------------- | ---------------------------------- |
| macOS (Apple Silicon) | `xuebadi-code-desktop-mac-arm64.dmg`   |
| macOS (Intel)         | `xuebadi-code-desktop-mac-x64.dmg`     |
| Windows               | `xuebadi-code-desktop-win-x64.exe`     |
| Linux                 | `.deb`, `.rpm`, 或 `.AppImage`     |

```bash
# macOS (Homebrew)
brew install --cask xuebadi-code-desktop
# Windows (Scoop)
scoop bucket add extras; scoop install extras/xuebadi-code-desktop
```

#### 安装目录

安装脚本按以下优先级选择安装路径：

1. `$OPENCODE_INSTALL_DIR` - 自定义安装目录
2. `$XDG_BIN_DIR` - XDG 标准路径
3. `$HOME/bin` - 用户二进制目录（如存在）
4. `$HOME/.opencode/bin` - 默认备用

```bash
# 示例
OPENCODE_INSTALL_DIR=/usr/local/bin curl -fsSL https://xuebadi-code.ai/install | bash
XDG_BIN_DIR=$HOME/.local/bin curl -fsSL https://xuebadi-code.ai/install | bash
```

### Agents（智能代理）

学霸帝Code 内置两种 Agent，用 `Tab` 键切换：

- **build** - 默认模式，完整权限，适合开发
- **plan** - 只读模式，适合代码分析和规划
  - 默认拒绝文件修改
  - 运行 bash 命令前会询问权限
  - 适合探索陌生代码库或规划改动

另外还包含 **general** 子 Agent，用于复杂搜索和多步任务。可在消息中用 `@general` 调用。

了解更多 [Agents 文档](https://xuebadi-code.ai/docs/agents)。

### 文档

更多配置说明请查看 [**官方文档**](https://xuebadi-code.ai/docs)。

### 参与贡献

欢迎贡献代码！提交 PR 前请阅读 [贡献指南](./CONTRIBUTING.md)。

### 基于 学霸帝Code 开发

如果你在开发与学霸帝Code相关的项目，并在项目名中使用了 "xuebadi-code" 或 "opencode"，请在 README 中注明该项目非官方开发，与学霸帝Code团队无隶属关系。

---

**加入社区** [GitHub Discussions](https://github.com/xuebadi/code/discussions) | [Issues](https://github.com/xuebadi/code/issues)
