# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This is a special GitHub organization repository for [Nutthead Studios](https://github.com/nutthead) that contains:

- Organization profile README content (profile/README.md)
- Organization-wide documentation and assets
- Git hooks configuration using samoyed

## Development Commands

### Git Hooks Management

This repository uses [samoyed](https://github.com/nutthead/samoyed), a Rust-based Git hooks manager. Configuration is in `samoyed.toml`:

```bash
# Hooks are automatically managed by samoyed
# Pre-commit: Formats all Markdown files with Prettier
# Pre-push: Checks Markdown formatting with Prettier
```

### Formatting

```bash
# Format Markdown files (run automatically on pre-commit)
npx prettier --log-level debug --write "**/*.md"

# Check Markdown formatting (run automatically on pre-push)
npx prettier --log-level debug --check "**/*.md"
```

## Repository Structure

- `profile/README.md` - Organization profile page content (appears on GitHub organization page)
- `profile/assets/` - Hero images and other assets for the profile
- `samoyed.toml` - Git hooks configuration for the samoyed hooks manager
- `.samoyed/` - Internal samoyed working directory (ignored by git)

## Key Information

- This is a documentation-focused repository with minimal development commands
- Primary purpose is maintaining the Nutthead Studios organization profile
- All Markdown files are automatically formatted using Prettier via git hooks
- The repository showcases samoyed (the organization's main project) - a fast Rust Git hooks manager
