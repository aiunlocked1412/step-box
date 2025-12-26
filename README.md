# Step Box 📦

> Visualize your project workflow with beautiful ASCII box diagrams

[![Claude Code Plugin](https://img.shields.io/badge/Claude%20Code-Plugin-blue)](https://claude.ai/claude-code)
[![Version](https://img.shields.io/badge/version-1.0.0-green)](https://github.com/aiunlocked1412/step-box)
[![License](https://img.shields.io/badge/license-MIT-blue)](LICENSE)
[![GitHub Actions](https://github.com/aiunlocked1412/step-box/workflows/Validate%20Plugin/badge.svg)](https://github.com/aiunlocked1412/step-box/actions)

## Overview

**Step Box** is a Claude Code plugin that analyzes your project structure and generates a visual workflow documentation in ASCII box format. Perfect for understanding complex projects at a glance!

## Features

- 🔍 **Automatic Analysis** - Scans your project structure and identifies workflow steps
- 📦 **ASCII Box Visualization** - Beautiful box diagrams using Unicode characters
- 📝 **Detailed Documentation** - Generates comprehensive STEP-BOX.md file
- 🔄 **Easy Updates** - Refresh documentation with a single command
- ⏰ **Timestamp Tracking** - Always know when docs were last updated

## Installation

### Method 1: Add Marketplace & Install

```bash
# Add the marketplace
/plugin marketplace add aiunlocked1412/step-box

# Install the plugin
/plugin install step-box@aiunlocked1412
```

### Method 2: Direct Install from GitHub

```bash
/plugin marketplace add https://github.com/aiunlocked1412/step-box.git
/plugin install step-box
```

### Method 3: Local Development

```bash
# Clone the repository
git clone https://github.com/aiunlocked1412/step-box.git

# Test locally
claude --plugin-dir ./step-box
```

## Usage

### Generate Workflow Documentation

```
/step-box:step
```

This will analyze your project and create a `STEP-BOX.md` file with:
- Project overview
- Visual workflow diagram with ASCII boxes
- Detailed step descriptions
- File structure tree

### Update Documentation

```
/step-box:update
```

Refresh the existing documentation to reflect any changes in your project.

## Example Output

```
┌─────────────────────────────────────────────────────────────┐
│                     MY-WEB-APP                               │
│                   [Node.js + Express]                        │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│  STEP 1: Application Entry                                  │
├─────────────────────────────────────────────────────────────┤
│  📁 File: src/index.js                                      │
│  📝 Description: Initialize Express server                  │
│  🔗 Dependencies: express, dotenv                           │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│  STEP 2: Route Configuration                                │
├─────────────────────────────────────────────────────────────┤
│  📁 File: src/routes/index.js                               │
│  📝 Description: Define API endpoints                       │
│  🔗 Dependencies: express.Router                            │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
                           (...)
```

## Commands Reference

| Command | Description |
|---------|-------------|
| `/step-box:step` | Generate new workflow documentation |
| `/step-box:update` | Update existing documentation |

## Customization

Add custom sections that won't be overwritten during updates:

```markdown
<!-- CUSTOM START -->
## My Custom Notes
This section will be preserved when running /step-box:update
<!-- CUSTOM END -->
```

## Supported Project Types

- Node.js / JavaScript / TypeScript
- Python
- Go
- Rust
- Java / Kotlin
- Ruby
- PHP
- And more...

## Plugin Structure

```
step-box/
├── .claude-plugin/
│   └── plugin.json       # Plugin manifest
├── commands/
│   ├── step.md           # /step-box:step command
│   └── update.md         # /step-box:update command
├── README.md
├── LICENSE
└── CHANGELOG.md
```

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

MIT License - see [LICENSE](LICENSE) for details.

---

Created by **[AI UNLOCKED](https://aiunlock.co)** ❤️
