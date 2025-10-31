# BambiSleep™ Church - AI Agent Instructions

_🌸 MCP Control Tower Planning Repository 🌸_

## Project Overview

**CRITICAL**: This is a **planning/documentation repository** - NOT an implemented codebase.

**What EXISTS**:

- `package.json` - Minimal package manifest with placeholder scripts (`echo 'not yet implemented'`)
- `BUILD.md` (408 lines) - Detailed implementation roadmap with architecture decisions
- `TODO.md` (143 lines) - Task breakdown for implementation phases
- `MCP_SETUP_GUIDE.md` (330 lines) - Guide for setting up 8 MCP servers
- `UNITY_SETUP_GUIDE.md` - Unity 6.2 installation guide
- `cspell.json` - Spell checker config with 169 technical terms

**What DOES NOT EXIST** (referenced in docs but unimplemented):

- ❌ No `.vscode/` directory (MCP server configs are aspirational)
- ❌ No `src/` directory (despite BUILD.md referencing `src/mcp/orchestrator.js`)
- ❌ No `public/docs/` directory structure
- ❌ No actual test files or implementation code
- ❌ No Unity project in this repository

**Actual Implementation**: See `/mnt/f/bambisleep-chat-catgirl` for the **production codebase** with:

- Complete Unity 6.2 project (6 C# systems, 1,950+ lines)
- Working Node.js IPC bridge
- Configured MCP servers (8/8 operational)
- Real tests and CI/CD pipeline

**This repository's purpose**: Architecture planning, setup guides, design decisions for future implementation.

## Critical Architecture Patterns (Planned, Not Yet Implemented)

### MCP Server Infrastructure (0/8 Active - .vscode/ Doesn't Exist)

**Planned Location**: `.vscode/settings.json` should contain MCP server registry
**Target Servers**: `filesystem`, `git`, `github`, `mongodb`, `stripe`, `huggingface`, `azure-quantum`, `clarity`

When implementing `.vscode/settings.json`, use this pattern:

```jsonc
// Pattern for adding MCP servers to .vscode/settings.json
"mcp.servers": {
  "servername": {
    "command": "npx",
    "args": ["-y", "@modelcontextprotocol/server-name", "/mnt/f/bambisleep-church-catgirl-control-tower"]
  }
}
```

### Development Workflow (Currently Non-Functional)

**All npm scripts echo placeholders** - need real implementations:

- `npm run dev` → `echo 'Development server not yet implemented'`
- `npm run test` → `echo 'Tests not yet implemented'`
- `npm run build` → `echo 'Build process not yet implemented'`
- `npm run start` → `echo 'Production server not yet implemented'`

**No VS Code tasks exist yet** - `.vscode/tasks.json` needs to be created with emoji-prefixed tasks

### Test Infrastructure (Aspirational)

**Referenced but Missing**: Documentation mentions Jest coverage reports at ~79%, but:

- No `coverage/` directory exists
- No `src/` directory exists
- No test files exist
- **Goal**: 100% coverage enforcement when implementation begins

## Essential Development Knowledge

### Emoji-Driven Development System

This project uses emoji prefixes for **machine-readable commit patterns**:

```javascript
// From RELIGULOUS_MANTRA.md - CI/CD automation patterns
"🌸"; // CHERRY_BLOSSOM - Package management, npm operations
"👑"; // CROWN - Architecture decisions, major refactors
"💎"; // GEM - Quality metrics, test coverage enforcement
"🦋"; // BUTTERFLY - Transformation processes, migrations
"✨"; // SPARKLES - Server operations, MCP management
"🎭"; // PERFORMING_ARTS - Development lifecycle, deployment
```

### Critical File Locations (Planned Structure)

```
# Files that EXIST:
/mnt/f/bambisleep-church-catgirl-control-tower/
├── package.json          # Package manifest with placeholder scripts
├── cspell.json          # Spell checker config with 169 technical terms
├── README.md            # Project overview (minimal)
├── BUILD.md             # 408-line implementation roadmap
└── TODO.md              # 143-line task breakdown

# Directories that DON'T EXIST YET (referenced in docs):
public/docs/             # Planned documentation location
├── RELIGULOUS_MANTRA.md    # Development philosophy & emoji mappings
├── MCP_SETUP_GUIDE.md      # Complete 8-server setup instructions
├── CATGIRL.md             # Unity avatar specs (683 lines referenced)
└── UNITY_SETUP_GUIDE.md   # Unity 6.2 installation on Linux

.vscode/                 # NOT CREATED YET
├── settings.json          # MCP server registry (planned)
├── tasks.json            # Emoji-prefixed task definitions (planned)
└── launch.json           # Browser debugging setup (planned)

src/                     # NOT CREATED YET
├── mcp/                   # MCP orchestrator implementation needed
├── utils/                 # Logger and utilities needed
└── ui/                    # Control Tower dashboard needed
```

### Organization Requirements

- **Always** use "BambiSleep™" trademark symbol
- Reference BambiSleepChat organization in GitHub operations
- Follow MIT license with proper attribution

## Dual-Platform Architecture

### Node.js MCP Control Tower

**Current State**: Package structure ready but implementation missing

- `src/` directory doesn't exist yet - needs to be created with `mcp/`, `utils/`, `ui/` subdirectories
- All npm scripts are placeholders - need real implementations before use
- Coverage reports mentioned in docs are aspirational targets, not actual files
- Missing source files: `src/mcp/orchestrator.js`, `src/utils/logger.js`, `src/index.js`

### Unity CatGirl Avatar System

**Specifications**: Referenced in `BUILD.md` and `TODO.md` (683-line spec planned)

- Unity 6.2 LTS with XR Interaction Toolkit
- Eye/hand tracking, RPG inventory, universal banking system
- Separate project from Node.js MCP codebase
- Documentation files (`CATGIRL.md`, `UNITY_SETUP_GUIDE.md`) not yet created

### VS Code Integration Patterns

**MCP Servers**: Will auto-register in AI assistant when `.vscode/settings.json` is created
**Tasks**: Need to create `.vscode/tasks.json` with emoji-prefixed tasks (🌸, 💎, 🌀)
**Problem Matchers**: ESLint integration via `$eslint-stylish` (when configured)
**Zero-Config**: No default formatter set (intentional design choice)

## MCP Server Configuration Guide

### Adding Missing Servers (5/8 Need Setup)

To add the remaining MCP servers to `.vscode/settings.json`:

```jsonc
// MongoDB - requires connection string
"mongodb": {
  "command": "npx",
  "args": ["-y", "@modelcontextprotocol/server-mongodb", "--connection-string", "mongodb://localhost:27017"]
},

// Stripe - requires API keys (set STRIPE_SECRET_KEY env var)
"stripe": {
  "command": "npx",
  "args": ["-y", "@modelcontextprotocol/server-stripe"]
},

// HuggingFace - requires token (set HUGGINGFACE_HUB_TOKEN env var)
"huggingface": {
  "command": "npx",
  "args": ["-y", "@modelcontextprotocol/server-huggingface"]
},

// Azure Quantum - requires workspace config
"azure-quantum": {
  "command": "npx",
  "args": ["-y", "@modelcontextprotocol/server-azure-quantum"]
},

// Microsoft Clarity - requires project ID
"clarity": {
  "command": "npx",
  "args": ["-y", "@modelcontextprotocol/server-microsoft-clarity"]
}
```

### Unity Development Patterns

**Architecture**: Component-based XR system with Unity 6.2
**Key Systems**: Eye/hand tracking, RPG inventory, multi-currency economy
**Implementation**: Separate Unity project following `CATGIRL.md` specifications

## Development Workflows

### Testing & Coverage (Priority: Reach 100%)

- **Current**: No actual tests or coverage yet - referenced in `BUILD.md` as targets
- **Command**: Use "💎 Run Tests (100% Coverage)" task (currently placeholder)
- **Philosophy**: "100% test coverage or suffer in callback hell eternal"

### Formatter Configuration (Zero-Config Approach)

- **Prettier**: Pre-installed but no default formatter set (intentional)
- **ESLint**: Problem matcher configured for `$eslint-stylish`
- **JSON**: Uses built-in `vscode.json-language-features`
- **Tailwind**: CSS validation disabled to prevent conflicts
- **Spell Check**: Code Spell Checker with `cspell.json` for technical terms

### Adding MCP Servers (5 Missing)

1. Install: `npm install @modelcontextprotocol/server-{name}`
2. Configure in `.vscode/settings.json`:
   ```jsonc
   "{name}": {
     "command": "npx",
     "args": ["-y", "@modelcontextprotocol/server-{name}", "/mnt/f/bambisleep-church-catgirl-control-tower"]
   }
   ```
3. Test via VS Code MCP integration

### MCP Server Integration Patterns

**Server Lifecycle Management**:

```javascript
// MCP servers auto-start with VS Code via npx -y pattern
// No local installation conflicts - each server runs independently
// Workspace-specific configuration in .vscode/settings.json
// Error handling via VS Code MCP extension logs
```

**VS Code Integration Hooks**:

- **Auto-registration**: MCP servers appear in VS Code AI assistant tools
- **Context Awareness**: All servers have workspace path context (`/mnt/f/bambisleep-church-catgirl-control-tower`)
- **Error Diagnostics**: Use VS Code MCP extension for debugging server issues
- **Environment Variables**: Set required API keys/tokens before server activation

**Server Communication Patterns**:

- **Filesystem Server**: Direct file operations, no authentication required
- **Git Server**: Repository operations using local Git config and SSH keys
- **GitHub Server**: Requires `GITHUB_TOKEN` environment variable
- **External APIs**: MongoDB, Stripe, HuggingFace, Azure, Clarity need credentials
- **Concurrent Access**: Multiple servers can operate simultaneously without conflicts

## Critical Patterns for AI Agents

### Organization Compliance Requirements

- **Always** include BambiSleep™ trademark symbol in documentation
- **GitHub operations** should reference BambiSleepChat organization context

### Dual Platform Development Workflow

**Node.js MCP Stack**:

1. Use VS Code tasks (Ctrl+Shift+P → "Run Task") for all npm operations
2. All scripts currently echo placeholders - need real implementations
3. Test coverage infrastructure exists but source code is missing
4. MCP server configuration via `.vscode/settings.json`

**Unity Avatar Development**:

1. Follow `UNITY_SETUP_GUIDE.md` for Unity 6.2 installation
2. CatGirl avatar specs in `CATGIRL.md` (683 lines of detailed requirements)
3. XR Interaction Toolkit for eye/hand tracking
4. Separate Unity project structure from Node.js MCP codebase

### Development Priority Order

1. **Complete MCP server configuration** (5 missing servers: mongodb, stripe, huggingface, azure-quantum, clarity)
2. **Achieve 100% test coverage** (coverage infrastructure exists but needs source code)
3. **Implement actual src/ code** (UI directory empty, but package.json structure ready)
4. **Set up proper npm scripts** (currently all echo placeholders - replace with real implementations)
5. **Unity CatGirl avatar system** (follow CATGIRL.md specifications for implementation)

### VS Code Integration Patterns

- Use **emoji-prefixed tasks** for all operations (matches RELIGULOUS_MANTRA.md)
- **MCP servers** auto-register in VS Code for AI assistant integration
- **Problem matchers** configured for ESLint integration
- **Zero-config approach**: No default formatter set (intentional design choice)
- **GitHub Copilot** configured for BambiSleepChat organization context

### Git Workflow (Emoji-Driven Commits)

**Standard Development Workflow**:

```bash
git add .
git commit -m "🌸💎 <commit_message>"
git push
```

**Emoji Commit Patterns** (from RELIGULOUS_MANTRA.md):

```bash
# Package management, npm operations
git commit -m "🌸 Add missing dependencies for MCP server integration"

# Architecture decisions, major refactors
git commit -m "👑 Restructure MCP server configuration for scalability"

# Quality metrics, test coverage enforcement
git commit -m "💎 Implement Jest tests to achieve 100% coverage"

# Transformation processes, migrations
git commit -m "🦋 Migrate documentation to public/docs/ structure"

# Server operations, MCP management
git commit -m "✨ Configure MongoDB and Stripe MCP servers"

# Development lifecycle, deployment
git commit -m "🎭 Set up production deployment pipeline"

# Combined patterns for complex changes
git commit -m "🌸👑 Update package.json and refactor MCP orchestrator architecture"
git commit -m "💎🦋 Add comprehensive tests and migrate legacy code patterns"
```
