# Cursor Spec Workflow Rule

*[中文文档 / Chinese Documentation](README-CN.md)*

A comprehensive workflow rule for Cursor IDE that transforms rough feature ideas into detailed specifications, designs, and implementation plans using a systematic spec-driven development approach.

## What is Spec-Driven Development?

Spec-driven development is a methodology that breaks down complex feature development into three systematic phases:

1. **Requirements Gathering** - Transform ideas into structured user stories and acceptance criteria
2. **Design Documentation** - Create comprehensive technical designs with architecture and components
3. **Implementation Planning** - Generate actionable task lists for code implementation

## Features

- **Systematic Workflow**: Guided three-phase process from idea to implementation
- **EARS Format Requirements**: Uses Easy Approach to Requirements Syntax for clear acceptance criteria
- **Research Integration**: Conducts necessary research during design phase
- **Task-Driven Implementation**: Generates specific, actionable coding tasks
- **Iterative Feedback**: Requires explicit user approval before progressing between phases
- **Todo Integration**: Tracks progress using Cursor's todo system

## Installation

1. Clone this repository to your project directory:
   ```bash
   git clone https://github.com/yourusername/cursor-spec-workflow-rule.git
   cd cursor-spec-workflow-rule
   ```

2. Copy the rule file to your project's Cursor rules directory:
   ```bash
   mkdir -p .cursor/rules
   cp .cursor/rules/spec-workflow.mdc .cursor/rules/
   ```

3. The rule will be automatically loaded by Cursor when you restart the IDE.

## Usage

### Starting a New Spec

1. **Initiate the workflow** by describing your feature idea to Cursor:
   ```
   I want to create a spec for [your feature idea]
   ```

2. **Requirements Phase**: The AI will:
   - Generate an initial requirements document at `.cursor/specs/{feature-name}/requirements.md`
   - Create user stories and EARS-format acceptance criteria
   - Ask for your approval before proceeding

3. **Design Phase**: After requirements approval:
   - Conducts necessary research
   - Creates a comprehensive design document at `.cursor/specs/{feature-name}/design.md`
   - Includes architecture, components, data models, and testing strategy

4. **Implementation Phase**: After design approval:
   - Generates an actionable task list at `.cursor/specs/{feature-name}/tasks.md`
   - Creates numbered, checkbox-format coding tasks
   - Each task references specific requirements

### Executing Tasks

Once your spec is complete, you can execute individual tasks:

1. Open the `tasks.md` file for your feature
2. Click "Start task" next to any task item
3. The AI will implement that specific task based on your requirements and design
4. Review the implementation before proceeding to the next task

### File Structure

The workflow creates the following structure:
```
.cursor/
  specs/
    {feature-name}/
      requirements.md    # User stories and acceptance criteria
      design.md         # Technical design and architecture
      tasks.md          # Implementation task checklist
```

## Workflow Phases

### 1. Requirements Gathering
- Transforms rough ideas into structured requirements
- Uses user story format: "As a [role], I want [feature], so that [benefit]"
- Creates EARS-format acceptance criteria
- Requires explicit user approval before proceeding

### 2. Design Documentation
- Conducts research on best practices and existing patterns
- Creates comprehensive technical design
- Includes architecture, components, interfaces, data models
- Addresses error handling and testing strategies

### 3. Implementation Planning
- Converts design into actionable coding tasks
- Prioritizes test-driven development
- Creates incremental, manageable steps
- References specific requirements for each task

## Best Practices

- **One Task at a Time**: Focus on completing individual tasks rather than rushing through multiple tasks
- **Iterative Feedback**: Provide feedback during each phase to ensure accuracy
- **Review Documents**: Carefully review each generated document before approval
- **Task Execution**: Execute tasks in order for best results

## Requirements

- Cursor IDE with rule support
- Project workspace with write permissions

## Contributing

Feel free to submit issues and enhancement requests. Contributions are welcome!

## License

This project is open source and available under the [MIT License](LICENSE).
