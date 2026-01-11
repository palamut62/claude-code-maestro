# 🐍 Maestro Scripts

Python automation scripts for hooks and utilities.

## Hook Scripts (6 Total)

These run automatically via `settings.json` hooks:

| Script | Hook | Purpose |
|--------|------|---------|
| [session_hooks.py](session_hooks.py) | SessionStart/End | Project detection, session tracking, dependency analysis |
| [explorer_helper.py](explorer_helper.py) | SessionStart | Deep project discovery |
| [dependency_scanner.py](dependency_scanner.py) | SessionStart | Dependency analysis |

## Utility Scripts

| Script | Purpose |
|--------|---------|
| [session_manager.py](session_manager.py) | Project state management |
| [auto_preview.py](auto_preview.py) | Preview server control |
| [setup.py](setup.py) | Cross-platform installation script |

## Per-Skill Scripts (Zero-Context Execution)

Skills now include their own scripts in `skills/<skill-name>/scripts/` subdirectories. See each skill's SKILL.md for available scripts.

**How Zero-Context Works:**
1. Claude does NOT read the script into context
2. Claude EXECUTES the script directly (`python scripts/xyz.py`)
3. Only script OUTPUT enters context
4. Result: Consistent, tested, fast execution

## Usage

### Hook Scripts (automatic)
```bash
# Configured in settings.json, runs automatically
python session_hooks.py start
```

### Utility Scripts (manual)
```bash
# Session manager
python session_manager.py init --path /project --type nextjs
python session_manager.py status

# Auto preview
python auto_preview.py start
python auto_preview.py stop
```

## Dependencies

```bash
pip install rich pydantic
```

## Data Files

Scripts read/write to `~/.claude/data/`:
- `session-stats.json` - Session metadata per project
- `current-project.json` - Global project reference
- `discovery-report.json` - Project structure analysis

---

**Last Updated:** 2026-01-09
**Version:** 3.0
