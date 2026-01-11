# Maestro System Architecture

> **Version 3.3** - Deep hierarchy and module mapping of the Maestro ecosystem.

## 🌐 Full System File Structure

```text
.claude/
├── agents/                           # 17 Specialized Agents
│   ├── orchestrator.md               # [CORE] Coordination & Orchestration
│   ├── backend-specialist.md         # [DEV] API, DB, Server logic
│   ├── frontend-specialist.md        # [DEV] Web UI/UX, React, Next.js
│   ├── mobile-developer.md           # [DEV] iOS/Android, React Native
│   ├── game-developer.md             # [DEV] Unity, Canvas, Mechanics
│   ├── database-architect.md         # [DATA] Complex schema, optimization
│   ├── devops-engineer.md            # [OPS] CI/CD, Deployment, Infrastructure
│   ├── security-auditor.md           # [SEC] Security compliance, audits
│   ├── penetration-tester.md         # [SEC] Ethical hacking, Red teaming
│   ├── performance-optimizer.md      # [OPT] Speed, Web Vitals, Profiling
│   ├── test-engineer.md              # [QA] Unit & Integration testing
│   ├── debugger.md                   # [QA] Systematic root cause analysis
│   ├── project-planner.md            # [MGMT] Roadmaps & Task breakdown
│   ├── documentation-writer.md       # [MGMT] Technical writing
│   ├── seo-specialist.md             # [MKTG] SEO, Analytics, Visibility
│   ├── explorer-agent.md             # [UTIL] Codebase discovery
│   └── README.md                     # Agent usage overview
│
├── skills/                           # 35 Skill Categories (Internal Files)
│   ├── api-patterns/                 # [API] REST, GraphQL, Auth
│   │   ├── SKILL.md                  # Index
│   │   ├── rest.md / graphql.md / trpc.md
│   │   └── auth.md / versioning.md / security-testing.md
│   ├── app-builder/                  # [APP] Scaffolding & Orchestration
│   │   ├── SKILL.md
│   │   ├── scaffolding.md / tech-stack.md / feature-building.md
│   │   └── templates/                # (Next.js, Saas, Mobile, etc.)
│   ├── architecture/                 # [ARCH] System Design
│   │   ├── SKILL.md
│   │   ├── pattern-selection.md / trade-off-analysis.md
│   │   └── context-discovery.md / examples.md
│   ├── bash-linux/                   # [CLI] Linux & macOS
│   │   └── SKILL.md
│   ├── behavioral-modes/             # [BEH] Agent Personas
│   │   └── SKILL.md
│   ├── brainstorming/                # [BRAIN] Socratic Questioning
│   │   └── SKILL.md
│   ├── clean-code/                   # [MANDATORY] Standards
│   │   └── SKILL.md
│   ├── code-review-checklist/        # [QA] Review standards
│   │   └── SKILL.md
│   ├── database-design/              # [DB] Schema & SQL
│   │   ├── SKILL.md
│   │   └── schema-design.md / indexing.md / migrations.md / orm.md
│   ├── deployment-procedures/        # [OPS] CI/CD
│   │   └── SKILL.md
│   ├── documentation-templates/      # [DOC] Standard formats
│   │   └── SKILL.md
│   ├── frontend-design/              # [UI/UX] Design Tokens & Spacing
│   │   ├── SKILL.md
│   │   ├── ux-psychology.md / typography-system.md / color-system.md
│   │   └── scripts/ux_audit.py
│   ├── game-development/             # [GAME] Engine & Mechanics
│   │   ├── SKILL.md
│   │   └── folders/ (2d-games, 3d-games, multiplayer, etc.)
│   ├── geo-fundamentals/             # [GEO] Generative Engine Optimization
│   │   └── SKILL.md
│   ├── lint-and-validate/            # [QA] Quality Automation
│   │   └── SKILL.md
│   ├── mcp-builder/                  # [MCP] Connector Creation
│   │   └── SKILL.md
│   ├── mobile-design/                # [UI/UX] App HIG & Material
│   │   ├── SKILL.md
│   │   ├── touch-psychology.md / platform-ios.md / platform-android.md
│   │   └── scripts/mobile_audit.py
│   ├── nextjs-best-practices/        # [WEB] App Router & SSR
│   │   └── SKILL.md
│   ├── nodejs-best-practices/        # [WEB] Server-side Node logic
│   │   └── SKILL.md
│   ├── parallel-agents/              # [CORE] Orchestration rules
│   │   └── SKILL.md
│   ├── performance-profiling/        # [OPT] Bottleneck detection
│   │   ├── SKILL.md
│   │   └── scripts/lighthouse_audit.py
│   ├── plan-writing/                 # [MGMT] Roadmaps
│   │   └── SKILL.md
│   ├── powershell-windows/           # [CLI] Windows PowerShell
│   │   └── SKILL.md
│   ├── python-patterns/              # [DEV] Pythonic code
│   │   └── SKILL.md
│   ├── react-patterns/               # [WEB] Composition & Hooks
│   │   └── SKILL.md
│   ├── red-team-tactics/             # [SEC] Offensive security
│   │   └── SKILL.md
│   ├── security-checklist/           # [SEC] OWASP hardening
│   │   └── SKILL.md
│   ├── seo-fundamentals/             # [MKTG] SEO Principles
│   │   └── SKILL.md
│   ├── server-management/            # [OPS] Nginx, SSH, Linux
│   │   └── SKILL.md
│   ├── systematic-debugging/         # [QA] RC Analysis
│   │   └── SKILL.md
│   ├── tailwind-patterns/            # [UI/UX] Utility styling
│   │   └── SKILL.md
│   ├── tdd-workflow/                 # [QA] Red-Green-Refactor
│   │   └── SKILL.md
│   ├── testing-patterns/             # [QA] Test strategy
│   │   └── SKILL.md
│   ├── vulnerability-scanner/        # [SEC] Security Auditing
│   │   ├── SKILL.md
│   │   └── scripts/security_scan.py
│   └── webapp-testing/               # [QA] E2E & Browser automation
│       ├── SKILL.md
│       └── scripts/playwright_runner.py
│
├── scripts/                          # 8 System Control Scripts
│   ├── session_hooks.py              # Startup/Shutdown logic
│   ├── explorer_helper.py            # Context builder
│   ├── dependency_scanner.py         # File dependency map
│   ├── auto_preview.py               # Live preview
│   ├── lint_check.py                 # Syntax audit
│   ├── session_manager.py            # Session persistence
│   ├── setup.py                      # Global installer
│   └── README.md                     # Script usage
│
├── CLAUDE.md                         # Global Constitution (v3.2)
```
