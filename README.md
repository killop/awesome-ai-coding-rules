# AI Coding Rules Collection

*[中文文档 / Chinese Documentation](README-CN.md)*

A comprehensive collection of AI coding rules and workflows for Cursor IDE, designed to enhance development productivity through specialized AI agents.

## 🚀 Overview

This repository contains specialized AI coding rules that transform how you interact with AI in development environments. Each rule focuses on specific development tasks for more effective AI assistance.

## 📂 Rule Categories

### 🔄 Development Workflows

#### Spec Workflow → [spec-workflow.md](spec-workflow.md)
Systematic spec-driven development workflow that transforms feature ideas into requirements, design, and implementation plans through a 3-phase iterative process.

#### RIPER-5 Workflow → [English](riper-5-workflow-EN.md) | [中文](riper-5-workflow-CN.md)
5-mode AI development collaboration framework (RESEARCH → INNOVATE → PLAN → EXECUTE → REFLECT) designed to prevent unauthorized code changes while maintaining structured development processes.

### 📝 Documentation & Content

#### PRD Writer → [prd-writer.md](prd-writer.md)
Creates comprehensive Product Requirements Documents (PRDs) with structured sections, user stories, and acceptance criteria following industry best practices.

#### Content Writer → [content-writer.md](content-writer.md)
Content marketing and copywriting agent with dual modes (outline/write) optimized for creating engaging, informative content that explains complex topics clearly.

### 🔧 Code Enhancement

#### Code Refactorer → [code-refactorer.md](code-refactorer.md)
Improves existing code structure, readability, and maintainability without changing functionality through systematic analysis and risk-managed improvements.

## 🛠️ Installation

### Method 1: Individual Rules
```bash
mkdir -p .cursor/rules
cp [rule-file].md .cursor/rules/
```

### Method 2: Full Collection
```bash
git clone https://github.com/yourusername/cursor-spec-workflow-rule.git
mkdir -p .cursor/rules
ln -s /path/to/cursor-spec-workflow-rule/*.md .cursor/rules/
```

### Method 3: Git Submodule
```bash
git submodule add https://github.com/yourusername/cursor-spec-workflow-rule.git .cursor/ai-rules
ln -s .cursor/ai-rules/*.md .cursor/rules/
```

## 🎯 Usage

Reference specific rules using the `@` symbol in Cursor:
```
@spec-workflow I want to create a spec for user authentication
@code-refactorer Help me clean up this messy function
@prd-writer Create a PRD for our new dashboard feature
```

## 📋 Rule Comparison

| Rule | Best For | Duration |
|------|----------|----------|
| **Spec Workflow** | Feature planning | Multi-session |
| **RIPER-5** | Controlled development | Per-task |
| **PRD Writer** | Product documentation | Single session |
| **Content Writer** | Technical writing | 1-2 sessions |
| **Code Refactorer** | Code improvement | Single session |

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Follow the established rule format with YAML frontmatter
4. Submit a pull request

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
