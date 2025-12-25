# Contributing to Step Box

Thank you for your interest in contributing to Step Box! This document provides guidelines and steps for contributing.

## Code of Conduct

By participating in this project, you agree to maintain a respectful and inclusive environment for everyone.

## How to Contribute

### Reporting Bugs

1. Check if the bug has already been reported in [Issues](https://github.com/aiunlocked1412/step-box/issues)
2. If not, create a new issue with:
   - Clear title describing the bug
   - Steps to reproduce
   - Expected vs actual behavior
   - Your environment (OS, Claude Code version)

### Suggesting Features

1. Check existing issues for similar suggestions
2. Create a new issue with the `enhancement` label
3. Describe:
   - The feature you'd like
   - Why it would be useful
   - Possible implementation approach

### Pull Requests

1. Fork the repository
2. Create a feature branch:
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. Make your changes
4. Test your changes thoroughly
5. Commit with clear messages:
   ```bash
   git commit -m "feat: add new visualization style"
   ```
6. Push to your fork:
   ```bash
   git push origin feature/your-feature-name
   ```
7. Open a Pull Request

## Commit Message Convention

We follow [Conventional Commits](https://www.conventionalcommits.org/):

- `feat:` - New feature
- `fix:` - Bug fix
- `docs:` - Documentation changes
- `style:` - Code style changes (formatting, etc.)
- `refactor:` - Code refactoring
- `test:` - Adding or updating tests
- `chore:` - Maintenance tasks

## Development Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/aiunlocked1412/step-box.git
   cd step-box
   ```

2. Install the plugin locally for testing:
   ```bash
   claude plugin install ./
   ```

3. Test your changes:
   ```bash
   # Navigate to a test project
   cd /path/to/test-project

   # Run the plugin
   /step
   ```

## File Structure

```
step-box/
├── package.json          # Plugin manifest
├── README.md             # User documentation
├── CONTRIBUTING.md       # This file
├── CHANGELOG.md          # Version history
├── LICENSE               # MIT License
└── skills/
    ├── step.md           # Main /step command
    └── step-update.md    # Update command
```

## Skill File Guidelines

When modifying skill files:

1. Keep instructions clear and actionable
2. Use consistent formatting
3. Include examples where helpful
4. Test with various project types

## Questions?

Feel free to open an issue with the `question` label if you need help!

---

Thank you for contributing!
