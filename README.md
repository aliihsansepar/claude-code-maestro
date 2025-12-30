# 🤖 Claude Framework

> **A comprehensive AI-assisted development framework** that transforms Claude into a powerful development team with specialized agents, intelligent skills, and automated workflows.

[![Agents](https://img.shields.io/badge/Agents-14-blue)](#-agents)
[![Skills](https://img.shields.io/badge/Skills-34-green)](#-skills)
[![Commands](https://img.shields.io/badge/Commands-9-orange)](#-commands)
[![Python](https://img.shields.io/badge/Python-3.10+-yellow)](#-scripts)

---

## ✨ Features

- 🤖 **14 Specialized Agents** - Expert AI personas for frontend, backend, mobile, DevOps, and more
-  **34 Skills** - Domain knowledge resources with patterns, best practices, and templates
- ⚡ **9 Slash Commands** - Quick actions for creating apps, debugging, testing, and deploying
- 🐍 **8 Python Scripts** - Automation hooks for error learning, session management, and progress tracking
- 🎭 **6 Behavioral Modes** - Adaptive AI behavior: Brainstorm, Implement, Debug, Review, Teach, Ship
- 🔄 **Error Learning System** - Automatically learns from past mistakes and prevents recurring issues

---

## 🚀 Quick Start

### Create an Application

```bash
/create e-commerce site with product listing and cart
```

The framework will:
1. Analyze your request
2. Plan the project structure
3. Coordinate specialized agents
4. Generate production-ready code
5. Start a preview server

### Add Features

```bash
/enhance add dark mode
/enhance build admin panel
```

### Other Commands

```bash
/brainstorm authentication options    # Explore ideas
/debug login not working              # Investigate issues
/test user service                    # Generate tests
/deploy production                    # Deploy safely
```

---

## 📁 Project Structure

```
claude-framework/
├── agents/              # 12 specialized AI agents
│   ├── frontend-specialist.md
│   ├── backend-specialist.md
│   ├── mobile-developer.md
│   ├── devops-engineer.md
│   └── ...
├── skills/              # 31 knowledge resources
│   ├── app-builder/
│   ├── behavioral-modes/
│   ├── react-patterns/
│   ├── templates/
│   │   ├── nextjs-fullstack/
│   │   ├── express-api/
│   │   ├── react-native-app/
│   │   └── nextjs-static/
│   └── ...
├── commands/            # 8 slash commands
│   ├── create.md
│   ├── enhance.md
│   ├── debug.md
│   └── ...
├── scripts/             # 7 Python automation scripts
│   ├── session_hooks.py
│   ├── pre_bash.py
│   ├── track_error.py
│   └── ...
├── data/                # Runtime state and error database
├── settings.json        # Hook configuration
├── CLAUDE.md           # AI behavior configuration
└── README.md           # This file
```

---

## 🤖 Agents

Specialized AI agents that handle different aspects of development:

| Agent | Expertise | Lines |
|-------|-----------|-------|
| **explorer-agent** | Codebase exploration, dependency research | 210 |
| **debugger** | Root cause analysis, systematic debugging | 250+ |
| **api-designer** | REST/GraphQL, OpenAPI, API security | 521 |
| **mobile-developer** | React Native, Flutter, Expo, App Store | 354 |
| **devops-engineer** | PM2, deployment, CI/CD, rollback | 275 |
| **test-engineer** | Testing strategies, TDD, coverage | 268 |
| **security-auditor** | Security review, vulnerabilities | 229 |
| **orchestrator** | Multi-agent coordination | 209 |
| **database-architect** | Schema design, Prisma, migrations | 189 |
| **backend-specialist** | Node.js, Express, FastAPI | 187 |
| **frontend-specialist** | React, Next.js, Tailwind | 149 |
| **project-planner** | Task breakdown, planning | 140 |
| **performance-optimizer** | Performance profiling | 132 |
| **documentation-writer** | README, API docs | 98 |

Each agent includes:
- Domain expertise and best practices
- Code patterns and examples
- Review checklists
- Trigger keywords for automatic selection

---

## 📚 Skills

Knowledge resources that agents reference for domain expertise:

### 🏗️ Architecture & Patterns
- `api-patterns` - REST/GraphQL design patterns
- `react-patterns` - React component patterns
- `mobile-patterns` - Mobile development patterns
- `nodejs-best-practices` - Node.js 23 patterns (Native TS, SQLite)
- `nextjs-best-practices` - Next.js 15 App Router & React 19 patterns
- `frontend-design` - 2025 Design Precision (8-point grid, Golden Ratio)

### 🎨 Templates
| Template | Description | Tech Stack |
|----------|-------------|------------|
| **nextjs-fullstack** | Full-stack web app | Next.js, Prisma, TypeScript, Tailwind |
| **express-api** | REST API | Express, JWT, Zod, Prisma |
| **react-native-app** | Mobile app | Expo, React Query, Zustand |
| **nextjs-static** | Landing page | Next.js, Framer Motion, Tailwind |

### 🛠️ Operations
- `server-management` - Server administration
- `deployment-procedures` - Safe deployment
- `performance-profiling` - Performance analysis
- `systematic-debugging` - Debugging methodology
- `mobile-ux-patterns` - Touch gestures, haptics, accessibility

---

## ⚡ Commands

| Command | Description | Mode |
|---------|-------------|------|
| `/create` | Create new application from natural language | IMPLEMENT |
| `/enhance` | Add features to existing app | IMPLEMENT |
| `/preview` | Start/stop preview server | UTILITY |
| `/status` | Show project and agent status | UTILITY |
| `/brainstorm` | Structured idea exploration | BRAINSTORM |
| `/debug` | Systematic problem investigation | DEBUG |
| `/test` | Generate and run tests | IMPLEMENT |
| `/deploy` | Production deployment with safety checks | SHIP |

---

## 🐍 Scripts

Python automation scripts that provide intelligent hooks:

### Hook Scripts (Automatic)
| Script | Hook | Purpose |
|--------|------|---------|
| `session_hooks.py` | SessionStart/End | Project detection, session tracking |
| `pre_bash.py` | PreToolUse | Error learning - warns about known issues |
| `check_prevention.py` | PreToolUse | Blocks dangerous commands |
| `track_error.py` | PostToolUse | Records errors for learning |

### Utility Scripts (Manual)
| Script | Purpose |
|--------|---------|
| `progress_reporter.py` | Agent status board with rich UI |
| `session_manager.py` | Project state management |
| `auto_preview.py` | Preview server control |
| `explorer_helper.py` | Proactive codebase discovery |
| `track_error.py` | Systematic error tracking |

### Dependencies

```bash
pip install rich pydantic
```

---

## 🎭 Behavioral Modes

The framework adapts its behavior based on context:

| Mode | Trigger Keywords | Behavior |
|------|------------------|----------|
| **BRAINSTORM** | "ideas", "options", "what if" | Explore alternatives, ask questions |
| **IMPLEMENT** | "build", "create", "add" | Fast execution, production code |
| **DEBUG** | "error", "not working", "bug" | Systematic investigation |
| **REVIEW** | "review", "check", "audit" | Thorough constructive analysis |
| **TEACH** | "explain", "how does" | Educational explanations |
| **SHIP** | "deploy", "production" | Pre-flight checks, safety first |

---

## 🔄 Error Learning System

The framework learns from mistakes to prevent recurring issues:

1. **Track** - Errors are automatically recorded with command context
2. **Learn** - Patterns are extracted and stored in error database
3. **Warn** - Similar commands trigger warnings with past error info
4. **Suggest** - Solutions from resolved errors are recommended

```
⚠️ Warning: Similar command failed before
   Command: npm install broken-package
   Error: npm ERR! 404 Not Found
   Suggestion: Check package name spelling or try npm cache clean
```

---

## ⚙️ Configuration

Hooks are configured in `settings.json`:

```json
{
  "hooks": {
    "SessionStart": [
      { "command": "python scripts/session_hooks.py start" }
    ],
    "PreToolUse": [
      { "command": "python scripts/pre_bash.py \"$TOOL_INPUT\"" },
      { "command": "python scripts/check_prevention.py \"$TOOL_INPUT\"" }
    ],
    "PostToolUse": [
      { "command": "python scripts/track_error.py ..." }
    ],
    "SessionEnd": [
      { "command": "python scripts/session_hooks.py end" }
    ]
  }
}
```

---

## � Statistics

| Category | Count |
|----------|-------|
| Agents | 14 |
| Skills | 34 |
| Commands | 9 |
| Scripts | 8 |
| Templates | 12 |
| Behavioral Modes | 6 |

---

## 🛠️ Requirements

- Python 3.10+
- Node.js 23+ (for native TypeScript & SQLite support)
- Claude Code or compatible AI assistant

---

## 📄 License

MIT License - See [LICENSE](LICENSE) for details.

---

## 🤝 Contributing

Contributions are welcome! Please read the documentation in each directory's README.md for specific guidelines.

---

<p align="center">
  <b>Built with ❤️ for AI-assisted development</b>
</p>
