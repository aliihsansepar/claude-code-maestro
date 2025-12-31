# Changelog

All notable changes to Maestro will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [0.0.3] - 2025-12-31

### Added
- **OS Detection & Context Injection**
  - Added automatic OS detection (Windows, macOS, Linux) in `session_hooks.py`
  - Added OS-specific terminal commands (PowerShell, bash, zsh)
  - Added dynamic `.claude/rules.md` generation in each project
  - Added `load_clean_code_skill()` to inject clean code standards into project context
  - Added `get_os_info()` and `get_os_commands()` functions

### Changed
- Session hooks now create `project/.claude/rules.md` with:
  - Project information (name, framework, type, path)
  - OS information and shell type
  - OS-specific terminal commands
  - Project-specific commands (npm, python, etc.)
  - Clean code standards from `skills/clean-code/SKILL.md`
- Fixed frontmatter parsing in `load_clean_code_skill()` - now correctly extracts content after YAML

### Removed
- **Terminal Error Learning System** (broken hooks compatibility)
  - Removed `scripts/pre_bash.py` - Error warning system
  - Removed `scripts/check_prevention.py` - Dangerous command blocking
  - Removed `scripts/track_error.py` - Error recording system
  - Removed `skills/terminal-error-patterns/` - Error patterns skill
  - Removed error tracking hooks from `settings.json`
  - Removed error database references from documentation

### Updated Documentation
- Updated README.md - Removed error learning feature
- Updated CLAUDE.md - Removed error tracking references
- Updated scripts/README.md - Simplified hook system documentation
- Updated data/README.md - Removed error database schema
- Updated docs/RESOURCES.md - Removed error learning resources
- Updated agents/debugger.md - Removed terminal-error-patterns skill reference
- Reduced script count from 9 to 5
- Reduced skill count from 40 to 37

---

## [0.0.2] - 2025-12-31

### Added
- **Security Testing**
  - New agent: `penetration-tester.md` for security assessments
  - New skill: `api-security-testing/` - API security patterns
  - New skill: `red-team-tactics/` - Adversary simulation tactics
  - New skill: `vulnerability-scanner/` - Vulnerability scanning procedures
- **Debug Logging**
  - Added `debug_log()` to `check_prevention.py`
  - Added `debug_log()` to `pre_bash.py`
  - Added `debug_log()` to `track_error.py`
  - Added `debug_log()` to `parallel_orchestrator.py`
- **Documentation**
  - Created `docs/RESOURCES.md` - Project resources (Turkish)
  - Created `docs/claude-code-reference.md` - Claude Code documentation

### Changed
- Updated README.md statistics (15 agents, 40+ skills, 8 scripts)
- Updated agents/README.md with new penetration-tester agent
- Updated skills/README.md with new security skills

### Removed
- **`scripts/progress_reporter.py`** - Removed unused script
- Removed `progress_reporter` references from all files
  - `scripts/parallel_orchestrator.py`
  - `README.md`, `CLAUDE.md`
  - `commands/status.md`, `commands/create.md`
  - `scripts/README.md`

### Fixed
- Fixed inaccurate multi-agent orchestration description in README
- Clarified agents work independently, not via JSON message passing

---

## [0.0.1] - 2025-12-30

### Initial Release
- 14 specialized agents
- 37 skills (patterns, templates)
- 9 Python hook scripts
- 8 slash commands
- Error learning system
- Parallel orchestration support
- Session management
- Auto preview server

---

[Unreleased]: https://github.com/xenitV1/claude-code-maestro/compare/v0.0.3...HEAD
[0.0.3]: https://github.com/xenitV1/claude-code-maestro/compare/v0.0.2...v0.0.3
[0.0.2]: https://github.com/xenitV1/claude-code-maestro/compare/v0.0.1...v0.0.2
[0.0.1]: https://github.com/xenitV1/claude-code-maestro/releases/tag/v0.0.1
