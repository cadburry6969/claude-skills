# Claude Rules & Skills for FiveM Development

A modular set of rules and guidelines tailored for Claude Code when developing FiveM resources (Lua, TypeScript, React UI, SQL/OxMySQL, performance, and security).

---

## What's Included

The `.claude/rules/` directory contains guidelines organized by category:

| Rule File | Description |
|---|---|
| [`database.md`](file:///.claude/rules/database.md) | Database practices, OxMySQL guidelines, and query optimization |
| [`fivem.md`](file:///.claude/rules/fivem.md) | FiveM native conventions, resource design, and state management |
| [`general.md`](file:///.claude/rules/general.md) | Code styling, commenting, folder layout, and refactoring practices |
| [`lua.md`](file:///.claude/rules/lua.md) | Lua coding standards, scoping, table handling, and idioms |
| [`performance.md`](file:///.claude/rules/performance.md) | FiveM performance tips (ticks, thread optimization, caching) |
| [`react.md`](file:///.claude/rules/react.md) | NUI frontend guidelines with React |
| [`security.md`](file:///.claude/rules/security.md) | Server/client security, exploit prevention, and event validation |
| [`testing.md`](file:///.claude/rules/testing.md) | Testing, edge case validation, and troubleshooting rules |
| [`typescript.md`](file:///.claude/rules/typescript.md) | TypeScript configuration and typing conventions for FiveM |
| [`ui.md`](file:///.claude/rules/ui.md) | NUI design, styling, and postMessage communication patterns |

---

## How to Install

You can install these rules either **per project** (recommended) or **globally** across all Claude sessions.

### Option 1: Per-Project Installation (Recommended)

Copy the `.claude` folder directly into the root directory of your target FiveM project/resource.

#### Windows (PowerShell)
```powershell
# From this repository directory, copy to your project:
Copy-Item -Path ".\.claude" -Destination "C:\path\to\your\fivem-resource\" -Recurse -Force
```

#### macOS / Linux / Bash
```bash
# From this repository directory, copy to your project:
cp -r .claude /path/to/your/fivem-resource/
```

**Project Structure Example:**
```text
my-fivem-resource/
├── .claude/
│   └── rules/
│       ├── database.md
│       ├── fivem.md
│       ├── general.md
│       └── ...
├── fxmanifest.lua
├── client/
│   └── main.lua
└── server/
    └── main.lua
```

---

### Option 2: Global Installation (All Claude Sessions)

To make these rules apply to every project opened with Claude Code on your system, copy the rules into your user-level Claude directory:

#### Windows (PowerShell)
```powershell
New-Item -ItemType Directory -Force -Path "$HOME\.claude\rules"
Copy-Item -Path ".\.claude\rules\*" -Destination "$HOME\.claude\rules\" -Recurse -Force
```

#### macOS / Linux / Bash
```bash
mkdir -p ~/.claude/rules
cp -r .claude/rules/* ~/.claude/rules/
```

---

### Option 3: Git Submodule (For Multi-Repo setups)

If you maintain multiple FiveM resources in separate git repositories, you can link this repository as a submodule:

```bash
git submodule add <REPO_URL> .claude-rules
# Symlink or copy .claude into place
```

---

## Recommended Plugins / Skills Setup

Inside Claude Code, run the following commands to add the marketplace repository and install the recommended plugins:

```text
/plugin marketplace add johnnyvizz/claude-kit
/plugin install savvy-flow@claude-kit
/plugin install savvy-progress@claude-kit
```

---

## Verification

To verify that Claude is using your rules:
1. Open your project folder in your terminal.
2. Launch Claude Code (`claude`).
3. Claude automatically discovers `.claude/rules/*.md` files and includes their context in your sessions.
