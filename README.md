# AI Coding Rules Collection

*[中文文档 / Chinese Documentation](README-CN.md)*

A comprehensive collection of AI coding rules and workflows for Cursor IDE, designed to enhance development productivity through specialized AI agents and systematic workflows.

## 🚀 Overview

This repository contains a curated set of AI coding rules that transform how you interact with AI in development environments. Each rule specializes in specific development tasks, from requirements gathering to code refactoring, enabling more focused and effective AI assistance.

## 📂 Rule Categories

### 🔄 Development Workflows

#### Spec Workflow
**File**: `spec-workflow.md`

A systematic spec-driven development workflow that transforms rough feature ideas into detailed specifications, designs, and implementation plans.

**Key Features**:
- **3-Phase Process**: Requirements → Design → Implementation Tasks
- **EARS Format**: Uses Easy Approach to Requirements Syntax for clear acceptance criteria
- **Research Integration**: Conducts necessary research during design phase
- **Iterative Feedback**: Requires explicit user approval between phases
- **Task Management**: Integrates with Cursor's todo system

**Usage**: `I want to create a spec for [your feature idea]`

#### RIPER-5 Workflow
**Files**: `riper-5-workflow-EN.md`, `riper-5-workflow-CN.md`

A 5-mode AI development collaboration framework designed to prevent unauthorized code changes while maintaining structured development processes.

**The 5 Modes**:
1. **RESEARCH**: Information gathering and deep understanding
2. **INNOVATE**: Creative solution generation
3. **PLAN**: Strategic implementation planning
4. **EXECUTE**: Controlled code implementation
5. **REFLECT**: Quality assessment and optimization

**Key Features**:
- **Mode Declaration**: Every response must declare current operating mode
- **Systematic Thinking**: Integrates systems, dialectical, innovative, and critical thinking
- **Change Control**: Prevents unauthorized modifications to existing code
- **Branch Management**: Includes git workflow integration

### 📝 Documentation & Content

#### PRD Writer
**File**: `prd-writer.md`

A specialized agent for creating comprehensive Product Requirements Documents (PRDs) following industry best practices.

**Key Features**:
- **Structured Output**: Organized sections including goals, personas, requirements, UX flows
- **User Stories**: Comprehensive user stories with unique IDs and acceptance criteria
- **Technical Considerations**: Includes scalability, performance, and integration points
- **Professional Format**: Industry-standard PRD formatting

**Usage**: `Create a PRD for [your project/feature]`

#### Content Writer
**File**: `content-writer.md`

A content marketing and copywriting agent optimized for creating engaging, informative content that explains complex topics clearly.

**Key Features**:
- **Two Modes**: Outline creation and content writing
- **Readability Focus**: Targets 8th-grade reading level with varied sentence structure
- **Research Integration**: Uses web search and MCP servers for fact verification
- **Anti-AI Detection**: Natural writing patterns with controlled imperfections
- **Strict Guidelines**: Avoids overused AI phrases and maintains authenticity

**Usage**: 
- Outline: `Create an outline for an article about [topic]`
- Writing: `Write the full article based on the outline`

### 🔧 Code Enhancement

#### Code Refactorer
**File**: `code-refactorer.md`

A specialized agent for improving existing code structure, readability, and maintainability without changing functionality.

**Key Features**:
- **Systematic Analysis**: Identifies duplication, naming issues, complexity problems
- **Preservation Focus**: Maintains exact functionality while improving structure
- **Best Practices**: Follows established patterns and conventions
- **Risk Management**: Prioritizes high-value, low-risk improvements
- **Clear Explanations**: Explains what, why, and how for each refactoring suggestion

**Usage**: `Help me refactor this code` or `Clean up the [specific component]`

## 🛠️ Installation

### Method 1: Individual Rules
Copy specific rule files to your project's Cursor rules directory:

```bash
# Create rules directory
mkdir -p .cursor/rules

# Copy desired rules (example)
cp spec-workflow.md .cursor/rules/
cp code-refactorer.md .cursor/rules/
```

### Method 2: Full Collection
Clone the entire repository and link to your project:

```bash
# Clone repository
git clone https://github.com/yourusername/cursor-spec-workflow-rule.git

# Create symbolic links (recommended)
mkdir -p .cursor/rules
ln -s /path/to/cursor-spec-workflow-rule/*.md .cursor/rules/
```

### Method 3: Submodule (For Git Projects)
Add as a git submodule:

```bash
git submodule add https://github.com/yourusername/cursor-spec-workflow-rule.git .cursor/ai-rules
ln -s .cursor/ai-rules/*.md .cursor/rules/
```

## 🎯 Usage Guidelines

### Rule Activation
In Cursor, reference specific rules using the `@` symbol:
```
@spec-workflow I want to create a spec for user authentication
@code-refactorer Help me clean up this messy function
@prd-writer Create a PRD for our new dashboard feature
```

### Best Practices
- **One Rule at a Time**: Focus on one specialized task per interaction
- **Clear Context**: Provide specific context about your project and requirements
- **Follow Workflows**: Respect the structured processes each rule defines
- **Review Outputs**: Always review generated documents and code before proceeding

## 📋 Rule Comparison

| Rule | Best For | Input | Output | Duration |
|------|----------|-------|---------|----------|
| **Spec Workflow** | Feature planning | Feature idea | Requirements, Design, Tasks | Multi-session |
| **RIPER-5** | Controlled development | Any dev task | Mode-specific responses | Per-task |
| **PRD Writer** | Product documentation | Project description | Complete PRD document | Single session |
| **Content Writer** | Technical writing | Topic/outline | Articles, blog posts | 1-2 sessions |
| **Code Refactorer** | Code improvement | Existing code | Refactored code + explanations | Single session |

## 🤝 Contributing

We welcome contributions! To add new rules or improve existing ones:

1. Fork the repository
2. Create a feature branch
3. Follow the established rule format with YAML frontmatter
4. Add comprehensive documentation
5. Submit a pull request

### Rule Format
Each rule should include:
```yaml
---
name: rule-name
description: Clear description with examples
tools: List of required tools
color: UI color identifier
---
```

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🔗 Related Resources

- [Cursor IDE Documentation](https://cursor.sh/docs)
- [AI Agent Best Practices](https://docs.anthropic.com/claude/docs)
- [Spec-Driven Development](https://en.wikipedia.org/wiki/Specification-driven_development)
