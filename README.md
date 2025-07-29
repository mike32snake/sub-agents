# Claude Code Basic Agents Collection

A comprehensive collection of specialized AI agents designed for use with Claude Code. These agents cover the complete software development lifecycle, from ideation to maintenance.

## Overview

This repository contains 11 specialized agents that can be easily integrated into your Claude Code workflows. Each agent is designed with specific objectives, tools, and methodologies to help streamline different aspects of software development and project management.

## Available Agents

### 1. **Ideation & Research Lead** (`ideation-research-lead.md`)
- **Purpose**: Conduct market research, competitive analysis, and ideation
- **Tools**: Write, Read, WebSearch
- **Key Tasks**: Market analysis, competitor research, opportunity identification

### 2. **Product Plan & Strategy** (`product-plan-strategy.md`)
- **Purpose**: Create comprehensive product requirement documents and strategic plans
- **Tools**: Write, Read, WebSearch
- **Key Tasks**: PRD creation, roadmap planning, feature prioritization

### 3. **UX/UI Designer** (`ux-ui-designer.md`)
- **Purpose**: Design user interfaces and create usability test plans
- **Tools**: Write, Read, WebSearch
- **Key Tasks**: Wireframing, mockups, component libraries, accessibility compliance

### 4. **Technical Feasibility Engineer** (`technical-feasibility-engineer.md`)
- **Purpose**: Assess technical viability and architectural requirements
- **Tools**: Write, Read, WebSearch
- **Key Tasks**: Technical analysis, risk assessment, architecture recommendations

### 5. **Code Implementation** (`code-implementation.md`)
- **Purpose**: Develop production-ready code following best practices
- **Tools**: Write, Read, Edit, Bash, WebSearch
- **Key Tasks**: Feature implementation, code optimization, documentation

### 6. **QA Test** (`qa-test.md`)
- **Purpose**: Ensure software quality through comprehensive testing
- **Tools**: Write, Read, Bash, WebSearch
- **Key Tasks**: Test planning, test case creation, bug reporting

### 7. **Security & Compliance** (`security-compliance.md`)
- **Purpose**: Ensure security best practices and regulatory compliance
- **Tools**: Write, Read, WebSearch
- **Key Tasks**: Security audits, vulnerability assessment, compliance documentation

### 8. **Deployment & DevOps** (`deployment-devops.md`)
- **Purpose**: Manage deployment pipelines and infrastructure
- **Tools**: Write, Read, Bash, WebSearch
- **Key Tasks**: CI/CD setup, infrastructure as code, monitoring

### 9. **Marketing & Launch** (`marketing-launch.md`)
- **Purpose**: Develop go-to-market strategies and launch campaigns
- **Tools**: Write, Read, WebSearch
- **Key Tasks**: Marketing plans, content creation, launch coordination

### 10. **Customer Support & Success** (`customer-support-success.md`)
- **Purpose**: Ensure customer satisfaction and product adoption
- **Tools**: Write, Read, WebSearch
- **Key Tasks**: Support documentation, success metrics, feedback analysis

### 11. **Maintenance & Analytics** (`maintenance-analytics.md`)
- **Purpose**: Monitor performance and guide continuous improvement
- **Tools**: Write, Read, Bash, WebSearch
- **Key Tasks**: Performance monitoring, analytics, optimization recommendations

## Installation & Usage

### Prerequisites
- Claude Code CLI installed on your system
- Access to Claude API

### Quick Start

1. **Clone this repository:**
   ```bash
   git clone https://github.com/mike32snake/basic-agents.git
   cd basic-agents
   ```

2. **Copy agents to your Claude Code agents directory:**
   ```bash
   # For macOS/Linux
   cp *.md ~/.claude/agents/

   # For Windows
   copy *.md %USERPROFILE%\.claude\agents\
   ```

3. **Use an agent in Claude Code:**
   ```bash
   claude --agent ux-ui-designer "Design a login page"
   ```

### Alternative: Direct Usage

You can also use these agents directly by referencing the markdown file:

```bash
claude --agent-file ./ux-ui-designer.md "Create wireframes for a dashboard"
```

## Agent Structure

Each agent follows a consistent structure:

```markdown
---
name: agent-name
description: Brief description of the agent's purpose
tools: List of available tools (Write, Read, Edit, Bash, WebSearch)
---

# Agent Role and Expertise

## Objectives
- Primary goals and responsibilities

## Steps
1. Detailed workflow steps
2. Specific methodologies to follow

## Deliverables
- Expected outputs and artifacts
```

## Contributing

We welcome contributions! To add a new agent or improve existing ones:

1. Fork this repository
2. Create a new branch (`git checkout -b feature/new-agent`)
3. Add or modify agent files
4. Test your agent thoroughly
5. Submit a pull request with a clear description

### Guidelines for New Agents
- Follow the existing agent structure
- Clearly define objectives and deliverables
- Specify required tools accurately
- Include practical examples where helpful
- Ensure the agent is focused on a specific domain

## Best Practices

1. **Choose the Right Agent**: Select agents based on your current project phase
2. **Chain Agents**: Use multiple agents in sequence for complex workflows
3. **Customize Prompts**: Provide specific context when invoking agents
4. **Review Outputs**: Always review and refine agent-generated content

## Examples

### Example 1: Full Development Cycle
```bash
# 1. Start with ideation
claude --agent ideation-research-lead "Research market for a task management app"

# 2. Create product requirements
claude --agent product-plan-strategy "Create PRD based on research findings"

# 3. Design the interface
claude --agent ux-ui-designer "Design the main dashboard interface"

# 4. Implement features
claude --agent code-implementation "Implement the task creation feature"

# 5. Test the implementation
claude --agent qa-test "Create test cases for task management features"
```

### Example 2: Quick Security Review
```bash
claude --agent security-compliance "Review this codebase for security vulnerabilities"
```

## License

This project is open source and available under the MIT License.

## Support

- **Issues**: Report bugs or request features via [GitHub Issues](https://github.com/mike32snake/basic-agents/issues)
- **Discussions**: Join our community discussions on [GitHub Discussions](https://github.com/mike32snake/basic-agents/discussions)

## Acknowledgments

These agents are designed to work seamlessly with Claude Code by Anthropic. Special thanks to the Claude team for creating such a powerful development assistant.

---

**Note**: These agents are templates and starting points. Feel free to modify them to suit your specific needs and workflows.