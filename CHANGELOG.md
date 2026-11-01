# Changelog

All notable changes to the **App Idea Validation Protocol** will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

---

## [1.0.0] - 2026-11-02

### Added
- Complete 12-stage validation protocol preservation from original Arabic master specification (`references/KHALIL_COLDSTART_PROTOCOL.md`).
- Fully standalone, compliant Claude Skill specification (`SKILL.md`) with valid YAML frontmatter, execution triggers, and Arabic-first interaction standards.
- English documentation suite:
  - Comprehensive `README.md` with visual Mermaid workflow diagram, philosophy, lifecycle flow, and prompt guides.
  - Research and validation philosophy (`docs/methodology.md`).
  - Decision gate taxonomy and continue/pivot/kill evaluation criteria (`docs/decision-gates.md`).
  - Strict evidence classification and data-freshness standards (`docs/evidence-standards.md`).
  - Platform developer policies and source verification procedures (`docs/source-verification.md`).
- Comprehensive Arabic documentation (`README.ar.md`) mirroring all technical depth, operational stages, and worked examples.
- Repository governance templates:
  - Issue templates for bug reports and improvement requests (`.github/ISSUE_TEMPLATE/`).
  - Pull request template (`.github/PULL_REQUEST_TEMPLATE.md`).
  - Lightweight GitHub Actions validation workflow (`.github/workflows/validate.yml`).
  - `.gitignore`, `.gitattributes`, `CONTRIBUTING.md`, and `SECURITY.md`.
