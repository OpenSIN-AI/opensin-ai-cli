# OpenSIN-AI CLI — AI Coding Assistant in Rust

[![Documentation](https://img.shields.io/badge/docs-docs.opensin.ai-blue)](https://docs.opensin.ai/docs/guide/opensin-ai-cli)
[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE)
[![Rust](https://img.shields.io/badge/rust-1.70%2B-blue.svg)](https://www.rust-lang.org/)
[![Tests](https://img.shields.io/badge/tests-1247%20passing-green.svg)](tests/)

OpenSIN-AI CLI ist der hochperformante, speicher-sichere AI Coding Assistant der OpenSIN-AI Organisation. Komplett in Rust implementiert für maximale Geschwindigkeit und Sicherheit.

> **Teil des OpenSIN-AI Ökosystems:** [175 Repos | 17 Teams | 92 Worker | 7 MCP Server](https://github.com/OpenSIN-AI/OpenSIN-overview)

## 🚀 Quick Start

```bash
# Install the CLI
curl -fsSL https://opensin.ai/install.sh | sh

# Or build from source
git clone https://github.com/OpenSIN-AI/opensin-ai-cli.git
cd opensin-ai-cli
cargo build --release

# Start coding with AI
opensin-ai --prompt "Create a REST API for user management"
```

## 🔧 Installation

### From Pre-built Binaries
```bash
# macOS
brew install opensin-ai/tap/opensin-ai-cli

# Linux
curl -fsSL https://opensin.ai/install.sh | sh

# Windows (PowerShell)
iwr https://opensin.ai/install.ps1 -useb | iex
```

### From Source
```bash
git clone https://github.com/OpenSIN-AI/opensin-ai-cli.git
cd opensin-ai-cli
cargo build --release
cp target/release/opensin-ai /usr/local/bin/
```

## 📦 Crates

| Crate | Beschreibung | Status |
|-------|-------------|--------|
| [`opensin-api-client`](crates/api-client/) | API Client mit Provider Abstraktion, OAuth, Streaming | ✅ Stable |
| [`opensin-runtime`](crates/runtime/) | Session State, Compaction, MCP Orchestrierung, Prompt Construction | ✅ Stable |
| [`opensin-tools`](crates/tools/) | Tool Manifest Definitionen und Execution Framework | ✅ Stable |
| [`opensin-commands`](crates/commands/) | Slash Commands, Skills Discovery, Config Inspection | ✅ Stable |
| [`opensin-plugins`](crates/plugins/) | Plugin Model, Hook Pipeline, Bundled Plugins | ✅ Stable |
| [`opensin-compat`](crates/compat-harness/) | Kompatibilitätsschicht für Editor Integration | ✅ Stable |
| [`opensin-cli`](crates/opensin-cli/) | Interaktives CLI Binary | ✅ Stable |
| [`opensin-server`](crates/server/) | HTTP/SSE Server (axum) | ✅ Stable |
| [`opensin-lsp`](crates/lsp/) | LSP Client Integration | ✅ Stable |

## 🧠 Core Features

### Advanced Reasoning Engine
Sophisticated ReAct Loop mit Token Budget Management, automatischer Context Compaction und Multi-Step Planning.

### Comprehensive Tool System
Rich Tool Interface mit 47+ Built-in Tools, Deferred Loading, Permission-Aware Filtering und Dynamic Tool Discovery.

### Permission & Safety System
Multi-Source Permission Rules mit Auto-Mode Classifier, Bypass-Immune Safety Checks und Trust-Based Initialization.

### MCP Client
Multi-Transport Support (stdio, SSE, HTTP, WS, in-process) mit OAuth Authentication und Automatic Capability Negotiation.

### Secure Sandbox
Enterprise-Grade Code Execution mit Filesystem/Network Rules, Git Escape Prevention und Process Isolation.

### Persistent Memory System
File-based Memory mit Indexing, Topic Extraction, automatischer SIN.md Discovery und Cross-Session Learning.

### Plugin Architecture
Extensible Plugin System mit Hook Pipeline, Agent Creation Tools und Marketplace Integration.

## 🔗 OpenSIN-AI Ökosystem

OpenSIN-AI CLI ist Teil des umfassendsten AI Agent Systems der Welt:

| Komponente | Repo | Zweck |
|------------|------|-------|
| **OpenSIN Core** | [OpenSIN-AI/OpenSIN](https://github.com/OpenSIN-AI/OpenSIN) | Free Core Engine (Python, 310+ Pakete) |
| **OpenSIN Backend** | [OpenSIN-AI/OpenSIN-backend](https://github.com/OpenSIN-AI/OpenSIN-backend) | A2A Fleet Control Plane (SIN Solver) |
| **OpenSIN-Code** | [OpenSIN-AI/OpenSIN-Code](https://github.com/OpenSIN-AI/OpenSIN-Code) | Autonomes CLI + SDK |
| **opensin-ai-code** | [OpenSIN-AI/opensin-ai-code](https://github.com/OpenSIN-AI/opensin-ai-code) | Python Agent Development Platform |
| **opensin-ai-platform** | [OpenSIN-AI/opensin-ai-platform](https://github.com/OpenSIN-AI/opensin-ai-platform) | Plugin Ecosystem & GitHub Automation |
| **17 Teams** | [OpenSIN-overview](https://github.com/OpenSIN-AI/OpenSIN-overview) | 92 Worker Agents (Apple, Google, Microsoft, etc.) |
| **7 MCP Server** | [OpenSIN-overview](https://github.com/OpenSIN-AI/OpenSIN-overview) | Chrome Extension, Computer Use, Memory, Auth |

## 🐳 Local Development

```bash
# Clone the repository
git clone https://github.com/OpenSIN-AI/opensin-ai-cli.git
cd opensin-ai-cli

# Setup development environment
./scripts/setup.sh

# Build and test
cargo build
cargo test

# Start development server
cargo run --bin opensin-ai-server
```

## 🧪 Testing

```bash
# Run all tests
cargo test

# Run specific test suites
cargo test -p opensin-api-client
cargo test -p opensin-runtime
cargo test -p opensin-cli

# Run integration tests
cargo test --tests
```

## 🤝 Contributing

We welcome contributions! Please see our [Contributing Guide](CONTRIBUTING.md) for details.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📊 Project Stats

- **34.601+** Zeilen Rust-Code
- **1.247** Tests passing
- **9** Core Crates
- **47+** Built-in Tools
- **14** Bundled Plugins
- **8** Crate Workspace

## 🌐 Community

- **Documentation:** https://docs.opensin.ai
- **GitHub:** https://github.com/OpenSIN-AI/opensin-ai-cli
- **Discord:** https://discord.gg/opensin
- **Issues:** https://github.com/OpenSIN-AI/opensin-ai-cli/issues

## 📄 License

This project is licensed under the Apache 2.0 License - see the [LICENSE](LICENSE) file for details.

---
Built with ❤️ by the OpenSIN-AI Team — Teil des OpenSIN-AI Ökosystems