# Project Context Plugin

A Claude Code plugin that scans and analyzes `CLAUDE.md` files to provide developers with a structured overview of project documentation, architecture, and dependencies.

## What It Does

This plugin helps developers quickly understand a codebase by:

- **Finding Documentation**: Locates all `CLAUDE.md` files in your project (root and subdirectories)
- **Analyzing Structure**: Extracts sections, headings, and organization of documentation
- **Extracting Key Info**: Identifies project scope, architecture patterns, conventions, and critical context
- **Mapping Dependencies**: Lists frameworks, libraries, tools, and build systems
- **Presenting Analysis**: Delivers a structured, scannable project brief

## Usage

Run the scan command in your project:

```bash
/project-context:scan-context
```

Claude will analyze your documentation and respond with a structured brief containing:
- Project overview and technology stack
- Document structure
- Key architectural information
- Dependencies and tools
- Quick start references

## When to Use

- Onboarding new developers to a project
- Getting a quick refresher on project architecture
- Understanding dependencies and tooling
- Identifying documentation gaps

## Requirements

- At least one `CLAUDE.md` file in your project
- If no `CLAUDE.md` exists, the plugin will suggest creating one

## Token Efficiency

Only loads one command into context when installed, making it lightweight and fast.
