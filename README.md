# OpenClaw-RS: Build an AI Agent from Scratch

[English](#english) | [中文](#中文)

---

<a name="english"></a>

## English

### What is OpenClaw-RS?

OpenClaw-RS is a progressive Rust course that teaches you how to build a production-grade AI Agent from scratch. Starting with just **100 lines of code**, you'll incrementally develop a full-featured AI assistant that rivals commercial solutions.

This course is based on reverse-engineering [OpenClaw](https://github.com/openclaw/openclaw.git), a TypeScript-based personal AI assistant platform with 400,000+ lines of code. We rebuild it in Rust, teaching you real-world software architecture along the way.

### Course Philosophy

**Agent-First Design**: Unlike traditional tutorials that start with "Hello World", we start with a working AI Agent. From day one, you'll have a functional AI assistant that gets more powerful with each version.

**Doubling Complexity**: Each version roughly doubles the code size and capabilities:

```
v0.1 (100 lines)  → v0.2 (200 lines)  → v0.3 (400 lines)  → ...  → v1.0 (50,000 lines)
    Single Q&A        Multi-turn          Tool Calling              Production Agent
```

### Version Roadmap

| Version | Lines | Core Feature | Agent Capability |
|---------|-------|--------------|------------------|
| v0.1 | ~100 | Minimal Agent | Single-turn Q&A |
| v0.2 | ~200 | Conversations | Context Memory |
| v0.3 | ~400 | Tool System | Function Calling |
| v0.4 | ~800 | Streaming | Real-time Output |
| v0.5 | ~1,600 | Persistence | SQLite Sessions |
| v0.6 | ~3,200 | Gateway | WebSocket Server |
| v0.7 | ~6,400 | Telegram | Bot Integration |
| v0.8 | ~12,800 | Multi-Channel | Discord/Slack + Browser |
| v0.9 | ~25,600 | Plugins | Dynamic Extensions |
| v1.0 | ~50,000 | Production | Multi-Agent + Long-term Memory |

### Agent Evolution

```
v0.1  ┌─────────────────┐
      │  Single Q&A     │  CLI interaction
      └────────┬────────┘
               │
v0.2  ┌────────▼────────┐
      │  Multi-turn     │  Context memory
      └────────┬────────┘
               │
v0.3  ┌────────▼────────┐
      │  Tool Calling   │  Calculator/DateTime
      └────────┬────────┘
               │
v0.4  ┌────────▼────────┐
      │  Streaming      │  Real-time + Web Search
      └────────┬────────┘
               │
v0.5  ┌────────▼────────┐
      │  Persistence    │  SQLite storage
      └────────┬────────┘
               │
v0.6  ┌────────▼────────┐
      │  Network        │  WebSocket gateway
      └────────┬────────┘
               │
v0.7  ┌────────▼────────┐
      │  Messaging      │  Telegram Bot
      └────────┬────────┘
               │
v0.8  ┌────────▼────────┐
      │  Multi-Channel  │  Discord/Slack + CDP
      └────────┬────────┘
               │
v0.9  ┌────────▼────────┐
      │  Extensible     │  Plugin system
      └────────┬────────┘
               │
v1.0  ┌────────▼────────┐
      │  Production     │  Multi-Agent + Memory
      └─────────────────┘
```

### Four Learning Phases

| Phase | Versions | Focus | Hours | Target Audience |
|-------|----------|-------|-------|-----------------|
| Phase 1 | v0.1-0.3 | Agent Basics + Tools | 8-10 | Rust beginners |
| Phase 2 | v0.4-0.5 | Streaming + Persistence | 8-10 | Developers with basics |
| Phase 3 | v0.6-0.8 | Networking + Channels | 14-18 | Intermediate developers |
| Phase 4 | v0.9-1.0 | Plugins + Production | 18-24 | Advanced developers |

### What You'll Learn

- **Rust Async Programming** - tokio, futures, streams
- **LLM Integration** - OpenAI/Anthropic APIs, Function Calling
- **Database Operations** - SQLite, migrations, connection pooling
- **Network Services** - WebSocket, HTTP/REST, JSON-RPC
- **Bot Development** - Telegram, Discord, Slack integrations
- **Browser Automation** - Chrome DevTools Protocol (CDP)
- **Plugin Architecture** - Dynamic loading, ABI stability
- **Production Deployment** - Docker, monitoring, observability

### Quick Start

```bash
# Clone the repository
git clone https://github.com/your-org/openclaw-rs.git
cd openclaw-rs

# Start with v0.1
cd versions/v0.1
cargo run

# Set your API key
export OPENAI_API_KEY=sk-your-key

# Start chatting!
> Hello, who are you?
Agent: Hello! I'm OpenClaw Agent v0.1...
```

### Prerequisites

- Rust 1.75+ (install via [rustup](https://rustup.rs))
- Basic programming knowledge
- OpenAI or Anthropic API key

### Course Structure

Each version includes:
- **Working Code** - Complete, runnable project
- **README** - Setup and usage instructions
- **Tests** - Unit and integration tests
- **Documentation** - API docs and architecture notes
- **Exercises** - 2-3 challenges to extend the project

### License

MIT License - feel free to use this for learning and teaching!

---

<a name="中文"></a>

## 中文

### OpenClaw-RS 是什么？

OpenClaw-RS 是一个渐进式 Rust 课程，教你从零开始构建一个生产级 AI Agent。从仅 **100 行代码** 开始，你将逐步开发一个功能完整的 AI 助手，达到商业解决方案的水平。

本课程基于对 [OpenClaw](https://github.com/openclaw/openclaw.git) 的逆向工程，OpenClaw 是一个基于 TypeScript 的个人 AI 助手平台，拥有超过 40 万行代码。我们用 Rust 重新实现它，同时教授真实世界的软件架构。

### 课程理念

**Agent-First 设计**：不同于传统教程从 "Hello World" 开始，我们从一个可用的 AI Agent 开始。从第一天起，你就拥有一个功能性的 AI 助手，它会随着每个版本变得更强大。

**倍增式复杂度**：每个版本的代码量和能力大约翻倍：

```
v0.1 (100 行)  → v0.2 (200 行)  → v0.3 (400 行)  → ...  → v1.0 (50,000 行)
    单轮问答        多轮对话          工具调用              生产级 Agent
```

### 版本路线图

| 版本 | 代码行数 | 核心功能 | Agent 能力 |
|------|----------|----------|------------|
| v0.1 | ~100 行 | 最小 Agent | 单轮问答 |
| v0.2 | ~200 行 | 多轮对话 | 上下文记忆 |
| v0.3 | ~400 行 | Tool 系统 | 工具调用 |
| v0.4 | ~800 行 | 流式输出 | 实时响应 |
| v0.5 | ~1,600 行 | 持久化 | SQLite 会话 |
| v0.6 | ~3,200 行 | 网关 | WebSocket 服务 |
| v0.7 | ~6,400 行 | Telegram | Bot 集成 |
| v0.8 | ~12,800 行 | 多频道 | Discord/Slack + 浏览器 |
| v0.9 | ~25,600 行 | 插件 | 动态扩展 |
| v1.0 | ~50,000 行 | 完整版 | 多 Agent + 长期记忆 |

### Agent 能力演进

```
v0.1  ┌─────────────────┐
      │  单轮问答       │  CLI 交互
      └────────┬────────┘
               │
v0.2  ┌────────▼────────┐
      │  多轮对话       │  上下文记忆
      └────────┬────────┘
               │
v0.3  ┌────────▼────────┐
      │  Tool 调用      │  计算器/时间
      └────────┬────────┘
               │
v0.4  ┌────────▼────────┐
      │  流式输出       │  实时响应 + 网页搜索
      └────────┬────────┘
               │
v0.5  ┌────────▼────────┐
      │  持久化会话     │  SQLite 存储
      └────────┬────────┘
               │
v0.6  ┌────────▼────────┐
      │  网络服务化     │  WebSocket 网关
      └────────┬────────┘
               │
v0.7  ┌────────▼────────┐
      │  即时通讯       │  Telegram Bot
      └────────┬────────┘
               │
v0.8  ┌────────▼────────┐
      │  多频道+浏览器  │  Discord/Slack + CDP
      └────────┬────────┘
               │
v0.9  ┌────────▼────────┐
      │  插件化 Agent   │  动态扩展
      └────────┬────────┘
               │
v1.0  ┌────────▼────────┐
      │  生产级 Agent   │  多 Agent 协作 + 长期记忆
      └─────────────────┘
```

### 四个学习阶段

| 阶段 | 版本 | 核心 Agent 能力 | 建议学时 | 适合人群 |
|------|------|----------------|----------|----------|
| 阶段一 | v0.1-0.3 | 基础对话 + Tool 调用 | 8-10 小时 | Rust 初学者 |
| 阶段二 | v0.4-0.5 | 流式输出 + 持久化 | 8-10 小时 | 有基础的开发者 |
| 阶段三 | v0.6-0.8 | 网络化 + 多频道 | 14-18 小时 | 中级开发者 |
| 阶段四 | v0.9-1.0 | 插件化 + 生产部署 | 18-24 小时 | 高级开发者 |

### 你将学到

- **Rust 异步编程** - tokio、futures、streams
- **LLM 集成** - OpenAI/Anthropic API、Function Calling
- **数据库操作** - SQLite、数据迁移、连接池
- **网络服务** - WebSocket、HTTP/REST、JSON-RPC
- **Bot 开发** - Telegram、Discord、Slack 集成
- **浏览器自动化** - Chrome DevTools Protocol (CDP)
- **插件架构** - 动态加载、ABI 稳定性
- **生产部署** - Docker、监控、可观测性

### 快速开始

```bash
# 克隆仓库
git clone https://github.com/your-org/openclaw-rs.git
cd openclaw-rs

# 从 v0.1 开始
cd versions/v0.1
cargo run

# 设置 API 密钥
export OPENAI_API_KEY=sk-your-key

# 开始对话！
> 你好，你是谁？
Agent: 你好！我是 OpenClaw Agent v0.1...
```

### 前置要求

- Rust 1.75+ (通过 [rustup](https://rustup.rs) 安装)
- 基本编程知识
- OpenAI 或 Anthropic API 密钥

### 课程结构

每个版本包含：
- **可运行代码** - 完整的独立项目
- **README** - 安装和使用说明
- **测试** - 单元测试和集成测试
- **文档** - API 文档和架构说明
- **练习** - 2-3 个扩展项目的挑战

### Agent 能力成长路径

| 版本 | Agent 能做什么 |
|------|---------------|
| v0.1 | 回答问题 |
| v0.2 | 记住对话上下文 |
| v0.3 | 调用工具 (计算、查时间) |
| v0.4 | 实时流式响应，搜索网页 |
| v0.5 | 记住历史对话，跨会话使用 |
| v0.6 | 通过网络远程访问 |
| v0.7 | 在 Telegram 中对话 |
| v0.8 | 多平台对话，操作浏览器 |
| v0.9 | 安装插件扩展能力 |
| v1.0 | 多 Agent 协作，长期记忆，生产部署 |

### 技术栈

```toml
[dependencies]
# 异步运行时
tokio = { version = "1", features = ["full"] }

# HTTP 客户端
reqwest = { version = "0.12", features = ["json", "stream"] }

# 序列化
serde = { version = "1", features = ["derive"] }
serde_json = "1"
serde_yaml = "0.9"

# 数据库
rusqlite = { version = "0.31", features = ["bundled"] }

# WebSocket
tokio-tungstenite = "0.21"
axum = "0.7"

# CLI
clap = { version = "4", features = ["derive"] }

# Telegram
teloxide = "0.12"

# Discord
serenity = "0.12"

# 浏览器
chromiumoxide = "0.6"
```

### 许可证

MIT License - 欢迎用于学习和教学！

---

## Contributing

Contributions are welcome! Please feel free to submit issues and pull requests.

欢迎贡献！请随时提交 issue 和 pull request。

## Acknowledgments

This course is inspired by [OpenClaw](https://github.com/openclaw/openclaw.git). We thank the original authors for creating such a comprehensive AI assistant platform.

本课程灵感来自 [OpenClaw](https://github.com/openclaw/openclaw.git)。感谢原作者创建了如此完善的 AI 助手平台。
