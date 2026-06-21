<p align="center">
  <a href="https://github.com/xuebadi/code">
    <picture>
      <source srcset="packages/console/app/src/asset/logo-ornate-dark.svg" media="(prefers-color-scheme: dark)">
      <source srcset="packages/console/app/src/asset/logo-ornate-light.svg" media="(prefers-color-scheme: light)">
      <img src="packages/console/app/src/asset/logo-ornate-light.svg" alt="学霸帝Code Logo" width="400">
    </picture>
  </a>
</p>

<p align="center">
  <strong>中文 AI 编程助手 - 本地运行，数据安全</strong>
</p>

<p align="center">
  <a href="https://github.com/xuebadi/code/releases/download/v0.1.0/xuebadi-code-desktop-win-x64.exe">
    <img alt="Windows下载" src="https://img.shields.io/badge/Windows-下载-blue?style=flat-square&logo=windows">
  </a>
  <a href="https://github.com/xuebadi/code/blob/main/LICENSE">
    <img alt="License" src="https://img.shields.io/github/license/xuebadi/code?style=flat-square">
  </a>
</p>

<p align="center">
  <a href="#安装">安装</a> •
  <a href="#功能特性">功能特性</a> •
  <a href="#支持的-llm">支持的 LLM</a> •
  <a href="#构建">构建</a> •
  <a href="#开源协议">开源协议</a>
</p>

---

## 学霸帝Code

**学霸帝Code** 是基于 [OpenCode](https://github.com/anomalyco/opencode) 二次开发的中文 AI 编程助手。它能在本地运行，保护你的代码数据安全，支持多种主流 LLM 提供商。

### ✨ 功能特性

- 🤖 **智能代码补全** - 支持多种编程语言的智能代码建议
- 💬 **自然语言编程** - 用中文描述需求，AI 自动生成代码
- 🔧 **代码重构** - 智能优化代码结构和性能
- 📖 **代码解释** - 帮助理解复杂代码逻辑
- 🐛 **Bug 修复** - 自动检测和修复代码问题
- 🔒 **本地运行** - 数据不出本地，安全可控
- 🌐 **多 LLM 支持** - 支持 OpenAI、Anthropic、Google、阿里通义、百度文心等

### 📥 安装

#### Windows 桌面版

直接下载安装包：

```powershell
# 下载最新版本
https://github.com/xuebadi/code/releases/latest
```

或使用命令行：

```bash
# 使用 npm
npm install -g opencode-ai@latest

# 使用 bun
bun install -g opencode-ai@latest

# 使用 scoop (Windows)
scoop install opencode
```

#### macOS

```bash
# Homebrew
brew install anomalyco/tap/opencode
```

#### Linux

```bash
# Arch Linux
sudo pacman -S opencode

# AUR
paru -S opencode-bin

# 通用安装脚本
curl -fsSL https://xuebadi-code.ai/install | bash
```

### 🎯 快速开始

1. **启动应用**
   ```bash
   # 命令行启动
   xuebadi-code
   
   # 或在应用菜单中找到"学霸帝Code"
   ```

2. **配置 LLM 提供商**
   - 打开设置 (Ctrl+, / Cmd+,)
   - 选择你喜欢的 LLM 提供商
   - 输入 API Key

3. **开始编程**
   - 在对话框输入自然语言描述
   - AI 会自动生成代码或修改建议

### 🤖 支持的 LLM

| 提供商 | 模型 | 说明 |
|--------|------|------|
| OpenAI | GPT-4, GPT-4o | 需要 API Key |
| Anthropic | Claude 3.5/4 | 需要_API Key |
| Google | Gemini Pro | 需要 API Key |
| 阿里云 | 通义千问 | 需要 API Key |
| 百度 | 文心一言 | 需要 API Key |
| DeepSeek | DeepSeek V3/R1 | 需要 API Key |
| Ollama | 本地模型 | 无需 API Key |

### 🏗️ 构建

#### 环境要求

- Node.js 18+ 或 Bun 1.3.14+
- Git
- Windows: Visual Studio Build Tools (可选)

#### 构建步骤

```bash
# 克隆仓库
git clone https://github.com/xuebadi/code.git
cd code

# 安装依赖
bun install

# 构建桌面应用
cd packages/desktop
bun run build

# 打包 Windows 安装包
bun run package:win

# 产物位置
# packages/desktop/dist/xuebadi-code-desktop-win-x64.exe
```

### 📝 开发

```bash
# 开发模式
cd packages/desktop
bun run dev

# 运行测试
bun test

# 类型检查
bun run typecheck
```

### 🤝 贡献

欢迎提交 Issue 和 Pull Request！

1. Fork 本仓库
2. 创建特性分支 (`git checkout -b feature/AmazingFeature`)
3. 提交更改 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 创建 Pull Request

### 📄 开源协议

本项目基于 MIT 协议开源，详见 [LICENSE](LICENSE) 文件。

### 🙏 致谢

- 感谢 [OpenCode](https://github.com/anomalyco/opencode) 团队的开源贡献
- 感谢所有贡献者的付出

---

<p align="center">
  Made with ❤️ by 学霸帝团队
</p>
