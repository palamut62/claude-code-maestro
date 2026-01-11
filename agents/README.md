# 🤖 Maestro Agents

Specialized AI agents for different development domains. Each agent has specific expertise, tools, and skill references.

## Agent List (17 Total)

| Agent | Expertise |
|-------|-----------|
| [orchestrator](orchestrator.md) | Multi-agent coordination, PLAN.md enforcement |
| [project-planner](project-planner.md) | Task breakdown, ROOT PLAN, milestones |
| [frontend-specialist](frontend-specialist.md) | React, Next.js, Tailwind, design systems |
| [backend-specialist](backend-specialist.md) | Node.js, Python, Express, FastAPI |
| [mobile-developer](mobile-developer.md) | React Native, Flutter, Expo, App Store |
| [database-architect](database-architect.md) | Schema design, Prisma, migrations |
| [devops-engineer](devops-engineer.md) | PM2, deployment, CI/CD, rollback |
| [test-engineer](test-engineer.md) | Testing strategies, TDD, coverage |
| [debugger](debugger.md) | Root cause analysis, systematic debugging |
| [security-auditor](security-auditor.md) | OWASP Top 10:2025, vulnerability scanning |
| [penetration-tester](penetration-tester.md) | Offensive security, PTES, red team |
| [performance-optimizer](performance-optimizer.md) | Performance profiling, Core Web Vitals |
| [seo-specialist](seo-specialist.md) | SEO, GEO, AI citations |
| [documentation-writer](documentation-writer.md) | README, API docs |
| [explorer-agent](explorer-agent.md) | Codebase exploration, dependency research |
| [game-developer](game-developer.md) | Game design, 2D/3D, multiplayer |

## Agent Format

```yaml
---
name: agent-name
description: Brief description with trigger keywords
allowed-tools: Read, Grep, Glob, Bash, Edit, Write
model: inherit
skills: skill1, skill2
---

# Agent Name

## Your Expertise
## Code Patterns  
## Review Checklist
```

## Usage

Agents are invoked by Claude based on context. Keywords in user requests trigger appropriate agents.

**Triggers:**
- "deploy", "production" → devops-engineer
- "mobile", "react native" → mobile-developer
- "test", "coverage" → test-engineer
- "orchestrate", "coordinate" → orchestrator
