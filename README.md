# AI Coding Rules Collection

*[中文文档 / Chinese Documentation](README-CN.md)*

A comprehensive collection of AI coding rules and workflows for Cursor IDE, designed to enhance development productivity through specialized AI agents.

## 🚀 Overview

This repository contains specialized AI coding rules that transform how you interact with AI in development environments. Each rule focuses on specific development tasks for more effective AI assistance.

## ⚡ Quick Start

1. **Choose your installation method** (see Installation section below)
2. **Pick a rule** from the categories that match your needs
3. **Use in Cursor** with `@rule-name` to activate specific behaviors
4. **Explore examples** in the Usage section for each category

### 🎯 Popular Combinations
- **New Project**: `@spec-workflow` → `@6A-workflow` → `@code-expert`
- **Code Review**: `@linus-coding-style` → `@code-refactorer`
- **Documentation**: `@prd-writer` → `@content-writer`
- **Learning**: `@chatgpt-study-mode` → `@book-recommendation-expert`

## 📂 Rule Categories

### 🔄 Development Workflows

#### Spec Workflow → [spec-workflow.md](spec-workflow.md)
Systematic spec-driven development workflow that transforms feature ideas into requirements, design, and implementation plans through a 3-phase iterative process.

#### RIPER-5 Workflow → [English](riper-5-workflow-EN.md) | [中文](riper-5-workflow-CN.md)
5-mode AI development collaboration framework (RESEARCH → INNOVATE → PLAN → EXECUTE → REFLECT) designed to prevent unauthorized code changes while maintaining structured development processes.

#### 6A Workflow → [中文](6A-workflow-CN.md)
Comprehensive 6-stage development process (Align → Architect → Atomize → Approve → Automate → Assess) for complex project management and systematic implementation.

### 🔧 Code Enhancement & Quality

#### Code Expert → [code-expert.md](code-expert.md)
Advanced development guidelines emphasizing incremental progress, test-driven development, and pragmatic code quality standards for professional software development.

#### Code Refactorer → [code-refactorer.md](code-refactorer.md)
Improves existing code structure, readability, and maintainability without changing functionality through systematic analysis and risk-managed improvements.

#### Linus Coding Style → [中文](linus-coding-style-CN.md)
Embodying Linus Torvalds' philosophy for code quality, focusing on "good taste," simplicity, and eliminating special cases through better data structures.

### 📝 Documentation & Content

#### PRD Writer → [prd-writer.md](prd-writer.md)
Creates comprehensive Product Requirements Documents (PRDs) with structured sections, user stories, and acceptance criteria following industry best practices.

#### Content Writer → [content-writer.md](content-writer.md)
Content marketing and copywriting agent with dual modes (outline/write) optimized for creating engaging, informative content that explains complex topics clearly.

#### Message Card Designer → [中文](message-card-CN.md)
Specialized UI designer for creating glassmorphism-style message cards with advanced visual design principles and responsive layouts.

### 🎓 Learning & Education

#### ChatGPT Study Mode → [English](chatgpt-study-mode-EN.md) | [中文](chatgpt-study-mode-CN.md)
Educational AI assistant designed to guide learning through questions, hints, and collaborative discovery rather than providing direct answers.

#### American Buddy Language Coach → [American-Buddy-Language-Coach.md](American-Buddy-Language-Coach.md)
Friendly American English language coach specializing in casual conversation, slang, idioms, and cultural references for immersive language learning.

#### Book Recommendation Expert → [Book-Recommendation-Expert.md](Book-Recommendation-Expert.md)
Personalized book recommendation system that provides detailed book analysis, benefits, and tailored suggestions across various genres and interests.

### 🚀 AI Enhancement

#### GPT GeniusBoost → [GPT-GeniusBoost.md](GPT-GeniusBoost.md)
Advanced AI assistant designed for highly intelligent users seeking comprehensive, in-depth analysis and detailed explorations of complex topics across all domains.

### 🎯 Specialized Tools

#### Project Naming Master → [Project-Naming-Master.md](Project-Naming-Master.md)
Expert in creating memorable, meaningful project names using multiple languages, mythology, and creative word formation techniques.

## 🛠️ Installation

### Method 1: Individual Rules
```bash
# Create rules directory
mkdir -p .cursor/rules

# Copy specific rule files
cp spec-workflow.md .cursor/rules/
cp code-expert.md .cursor/rules/
# ... copy other rules as needed
```

### Method 2: Full Collection
```bash
# Clone the repository
git clone https://github.com/yourusername/cursor-spec-workflow-rule.git

# Create rules directory
mkdir -p .cursor/rules

# Create symbolic links to all rules
ln -s /path/to/cursor-spec-workflow-rule/*.md .cursor/rules/
```

### Method 3: Git Submodule (Recommended)
```bash
# Add as submodule
git submodule add https://github.com/yourusername/cursor-spec-workflow-rule.git .cursor/ai-rules

# Create symbolic links
ln -s .cursor/ai-rules/*.md .cursor/rules/
```

### Method 4: Direct Download
```bash
# Download specific rules directly
curl -o .cursor/rules/spec-workflow.md https://raw.githubusercontent.com/yourusername/cursor-spec-workflow-rule/main/spec-workflow.md
```

## 🎯 Usage

Reference specific rules using the `@` symbol in Cursor:

### Development Workflows
```
@spec-workflow I want to create a spec for user authentication
@riper-5-workflow Help me plan a new feature systematically
@6A-workflow I need to implement a complex system with proper architecture
```

### Code Quality & Enhancement
```
@code-expert Review this code and suggest improvements
@code-refactorer Help me clean up this messy function
@linus-coding-style Analyze this code for "good taste" and simplicity
```

### Documentation & Content
```
@prd-writer Create a PRD for our new dashboard feature
@content-writer Help me write technical documentation
@message-card-designer Design a modern UI component
```

### Learning & Education
```
@chatgpt-study-mode Help me understand this concept through guided learning
@american-buddy-language-coach Practice casual English conversation
@book-recommendation-expert Recommend books for learning software architecture
```

### AI Enhancement & Tools
```
@gpt-geniusboost Provide comprehensive analysis of this complex topic
@project-naming-master Help me find a great name for my new project
```

## 📋 Rule Comparison

| Rule | Category | Best For | Duration | Language |
|------|----------|----------|----------|----------|
| **Spec Workflow** | Development | Feature planning | Multi-session | EN |
| **RIPER-5** | Development | Controlled development | Per-task | EN/CN |
| **6A Workflow** | Development | Complex project management | Multi-session | CN |
| **Code Expert** | Code Quality | Professional development | Per-task | EN |
| **Code Refactorer** | Code Quality | Code improvement | Single session | EN |
| **Linus Coding Style** | Code Quality | Code quality analysis | Single session | CN |
| **PRD Writer** | Documentation | Product documentation | Single session | EN |
| **Content Writer** | Documentation | Technical writing | 1-2 sessions | EN |
| **Message Card Designer** | Documentation | UI design | Single session | CN |
| **ChatGPT Study Mode** | Learning | Educational guidance | Per-session | EN/CN |
| **American Buddy** | Learning | Language learning | Ongoing | EN |
| **Book Recommendation** | Learning | Reading suggestions | Single session | EN |
| **GPT GeniusBoost** | AI Enhancement | Deep analysis | Per-query | EN |
| **Project Naming Master** | Tools | Project naming | Single session | EN |

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Follow the established rule format with YAML frontmatter
4. Submit a pull request

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
