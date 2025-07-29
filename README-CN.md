# AI 编程规则集合

*[English Documentation / 英文文档](README.md)*

专为 Cursor IDE 设计的 AI 编程规则和工作流综合集合，通过专业化的 AI 代理提升开发效率。

## 🚀 项目概述

本仓库包含专业化的 AI 编程规则，旨在改变你在开发环境中与 AI 的交互方式。每个规则专注于特定开发任务，实现更高效的 AI 辅助。

## 📂 规则分类

### 🔄 开发工作流

#### 规格工作流 → [spec-workflow.md](spec-workflow.md)
系统化的规格驱动开发工作流，通过三阶段迭代流程将功能想法转化为需求、设计和实施计划。

#### RIPER-5 工作流 → [英文版](riper-5-workflow-EN.md) | [中文版](riper-5-workflow-CN.md)
5模式AI开发协作框架（研究→创新→规划→执行→反思），旨在防止未授权代码更改的同时保持结构化开发流程。

### 📝 文档与内容

#### PRD 写作器 → [prd-writer.md](prd-writer.md)
创建包含结构化章节、用户故事和验收标准的综合产品需求文档（PRD），遵循行业最佳实践。

#### 内容写作器 → [content-writer.md](content-writer.md)
具有双模式（大纲/写作）的内容营销和文案写作代理，专为创建清晰解释复杂主题的引人入胜内容而优化。

### 🔧 代码改进

#### 代码重构器 → [code-refactorer.md](code-refactorer.md)
通过系统化分析和风险管理改进，在不改变功能的前提下提升现有代码结构、可读性和可维护性。

## 🛠️ 安装方法

### 方法一：单个规则
```bash
mkdir -p .cursor/rules
cp [规则文件].md .cursor/rules/
```

### 方法二：完整集合
```bash
git clone https://github.com/yourusername/cursor-spec-workflow-rule.git
mkdir -p .cursor/rules
ln -s /path/to/cursor-spec-workflow-rule/*.md .cursor/rules/
```

### 方法三：Git 子模块
```bash
git submodule add https://github.com/yourusername/cursor-spec-workflow-rule.git .cursor/ai-rules
ln -s .cursor/ai-rules/*.md .cursor/rules/
```

## 🎯 使用方法

在 Cursor 中使用 `@` 符号引用特定规则：
```
@spec-workflow I want to create a spec for user authentication
@code-refactorer Help me clean up this messy function
@prd-writer Create a PRD for our new dashboard feature
```

## 📋 规则对比

| 规则 | 最适用于 | 持续时间 |
|------|----------|----------|
| **规格工作流** | 功能规划 | 多会话 |
| **RIPER-5** | 受控开发 | 按任务 |
| **PRD 写作器** | 产品文档 | 单会话 |
| **内容写作器** | 技术写作 | 1-2会话 |
| **代码重构器** | 代码改进 | 单会话 |

## 🤝 贡献

1. Fork 仓库
2. 创建功能分支
3. 遵循既定的规则格式，包含 YAML frontmatter
4. 提交 pull request

## 📄 许可证

该项目是开源的，遵循 [MIT 许可证](LICENSE)。 