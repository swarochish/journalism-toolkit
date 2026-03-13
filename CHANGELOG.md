# Changelog

## 1.1.0 (2026-03-13)

### New Agents
- **ai-content-detector** - Detect AI-generated text, click-farm content, and synthetic articles using multi-tool consensus (GPTZero, Originality.ai, Copyleaks), perplexity/burstiness analysis, and stylometric fingerprinting
- **foreign-news-analyst** - Translate foreign-language news with editorial quality, detect PR-sanitization in cross-language reporting, identify state media propaganda patterns (RT, CGTN, IRNA, KCNA)
- **grassroots-sincerity-analyst** - Evaluate real human accounts for sincerity (0-100 scoring), detect troll-army patterns and paid shills, separate high-value grassroots voices from coordinated amplifiers

### Improvements
- Updated README for better GitHub discoverability: added table of contents, use cases, FAQ, expanded contributing section, PRs Welcome badge
- Updated GitHub repo description and topics for search visibility
- Updated journalism-master-orchestrator to coordinate 28+ agents with new Tier 2/3 entries
- Updated disinformation-investigation-orchestrator to coordinate 19 sub-agents with new agent conditions and pseudocode
- Updated both commands (ultimate-multimedia-journalist, disinformation-brain) with new agent references and verification triggers

## 1.0.0 (2025-03-11)

- Initial release as Claude Code plugin
- 27 journalism agents (6 core, 16 verification, 4 multimedia/distribution, 1 disinformation)
- 2 commands: ultimate-multimedia-journalist, disinformation-brain
- 1 skill: investigation-report-generator (HTML dossier generation)
