# AI 编程规则集合

*[English Documentation / 英文文档](README.md)*

专为 Cursor IDE 设计的 AI 编程规则和工作流综合集合，通过专业化的 AI 代理和系统化工作流提升开发效率。

## 🚀 项目概述

本仓库包含一套精心策划的 AI 编程规则，旨在改变你在开发环境中与 AI 的交互方式。每个规则都专注于特定的开发任务，从需求收集到代码重构，实现更专注和高效的 AI 辅助。

## 📂 规则分类

### 🔄 开发工作流

#### 规格工作流 (Spec Workflow)
**文件**: `spec-workflow.md`

一个系统化的规格驱动开发工作流，将粗糙的功能想法转化为详细的规格说明、设计方案和实施计划。

**核心功能**:
- **三阶段流程**: 需求 → 设计 → 实施任务
- **EARS 格式**: 使用简易需求语法创建清晰的验收标准
- **研究集成**: 在设计阶段进行必要的研究调查
- **迭代反馈**: 在各阶段之间需要用户明确批准
- **任务管理**: 与 Cursor 的 todo 系统集成

**使用方法**: `I want to create a spec for [你的功能想法]`

#### RIPER-5 工作流
**文件**: `riper-5-workflow-EN.md`, `riper-5-workflow-CN.md`

一个 5 模式的 AI 开发协作框架，旨在防止未授权的代码更改，同时保持结构化的开发流程。

**5 大模式**:
1. **RESEARCH**: 信息收集和深入理解
2. **INNOVATE**: 创造性解决方案生成
3. **PLAN**: 战略实施规划
4. **EXECUTE**: 受控代码实现
5. **REFLECT**: 质量评估和优化

**核心功能**:
- **模式声明**: 每个响应都必须声明当前操作模式
- **系统思维**: 整合系统性、辩证性、创新性和批判性思维
- **变更控制**: 防止对现有代码的未授权修改
- **分支管理**: 包含 git 工作流集成

### 📝 文档与内容

#### PRD 写作器
**文件**: `prd-writer.md`

专门用于创建遵循行业最佳实践的综合产品需求文档 (PRD) 的代理。

**核心功能**:
- **结构化输出**: 组织化的章节，包括目标、用户画像、需求、UX 流程
- **用户故事**: 带有唯一 ID 和验收标准的综合用户故事
- **技术考量**: 包含可扩展性、性能和集成要点
- **专业格式**: 行业标准的 PRD 格式

**使用方法**: `Create a PRD for [你的项目/功能]`

#### 内容写作器
**文件**: `content-writer.md`

专为创建引人入胜、信息丰富且能清晰解释复杂主题的内容而优化的内容营销和文案写作代理。

**核心功能**:
- **双模式**: 大纲创建和内容写作
- **可读性专注**: 针对初中阅读水平，句式结构多样化
- **研究集成**: 使用网络搜索和 MCP 服务器进行事实验证
- **反 AI 检测**: 具有受控瑕疵的自然写作模式
- **严格准则**: 避免常用的 AI 短语，保持真实性

**使用方法**: 
- 大纲: `Create an outline for an article about [主题]`
- 写作: `Write the full article based on the outline`

### 🔧 代码改进

#### 代码重构器
**文件**: `code-refactorer.md`

专门用于改善现有代码结构、可读性和可维护性而不改变功能的代理。

**核心功能**:
- **系统化分析**: 识别重复、命名问题、复杂性问题
- **保持功能**: 在改善结构的同时维持确切的功能
- **最佳实践**: 遵循既定模式和约定
- **风险管理**: 优先考虑高价值、低风险的改进
- **清晰解释**: 为每个重构建议解释是什么、为什么和如何

**使用方法**: `Help me refactor this code` 或 `Clean up the [具体组件]`

## 🛠️ 安装方法

### 方法一：单个规则
将特定的规则文件复制到项目的 Cursor 规则目录：

```bash
# 创建规则目录
mkdir -p .cursor/rules

# 复制所需规则（示例）
cp spec-workflow.md .cursor/rules/
cp code-refactorer.md .cursor/rules/
```

### 方法二：完整集合
克隆整个仓库并链接到你的项目：

```bash
# 克隆仓库
git clone https://github.com/yourusername/cursor-spec-workflow-rule.git

# 创建符号链接（推荐）
mkdir -p .cursor/rules
ln -s /path/to/cursor-spec-workflow-rule/*.md .cursor/rules/
```

### 方法三：子模块（适用于 Git 项目）
作为 git 子模块添加：

```bash
git submodule add https://github.com/yourusername/cursor-spec-workflow-rule.git .cursor/ai-rules
ln -s .cursor/ai-rules/*.md .cursor/rules/
```

## 🎯 使用指南

### 规则激活
在 Cursor 中，使用 `@` 符号引用特定规则：
```
@spec-workflow I want to create a spec for user authentication
@code-refactorer Help me clean up this messy function
@prd-writer Create a PRD for our new dashboard feature
```

### 最佳实践
- **一次一个规则**: 每次交互专注于一个专业化任务
- **清晰上下文**: 提供关于项目和需求的具体上下文
- **遵循工作流**: 尊重每个规则定义的结构化流程
- **审查输出**: 在继续之前始终审查生成的文档和代码

## 📋 规则对比

| 规则 | 最适用于 | 输入 | 输出 | 持续时间 |
|------|----------|-------|---------|----------|
| **规格工作流** | 功能规划 | 功能想法 | 需求、设计、任务 | 多会话 |
| **RIPER-5** | 受控开发 | 任何开发任务 | 特定模式响应 | 按任务 |
| **PRD 写作器** | 产品文档 | 项目描述 | 完整 PRD 文档 | 单会话 |
| **内容写作器** | 技术写作 | 主题/大纲 | 文章、博客文章 | 1-2会话 |
| **代码重构器** | 代码改进 | 现有代码 | 重构代码+解释 | 单会话 |

## 🤝 贡献

我们欢迎贡献！添加新规则或改进existing规则：

1. Fork 仓库
2. 创建功能分支
3. 遵循既定的规则格式，包含 YAML frontmatter
4. 添加全面的文档
5. 提交 pull request

### 规则格式
每个规则应包含：
```yaml
---
name: rule-name
description: 清晰的描述和示例
tools: 所需工具列表
color: UI 颜色标识符
---
```

## 📄 许可证

该项目是开源的，遵循 [MIT 许可证](LICENSE)。

## 🔗 相关资源

- [Cursor IDE 文档](https://cursor.sh/docs)
- [AI 代理最佳实践](https://docs.anthropic.com/claude/docs)
- [规格驱动开发](https://en.wikipedia.org/wiki/Specification-driven_development) 