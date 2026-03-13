[![Version](https://img.shields.io/badge/version-1.1.0-blue.svg)](https://github.com/swarochish/journalism-toolkit)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Claude Code](https://img.shields.io/badge/Claude%20Code-v1.0.33+-purple.svg)](https://claude.com/claude-code)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/swarochish/journalism-toolkit/pulls)

# Journalism Toolkit for Claude Code

The most comprehensive journalism AI system available as a Claude Code plugin. 30 specialized agents, 2 commands, and 1 analytical skill covering investigative reporting, fact-checking, disinformation analysis, AI content detection, foreign news de-biasing, bot & troll detection, multimedia production, and content distribution.

> One command. Five journalism modes. From tip to publication.

---

## Table of Contents

- [Why This Plugin?](#why-this-plugin)
- [Domains Covered](#domains-covered)
- [Installation](#installation)
- [Quick Start Commands](#quick-start-commands)
- [How It Works](#how-it-works)
- [What's Inside](#whats-inside)
- [Architecture](#architecture)
- [Repository Structure](#repository-structure)
- [Use Cases](#use-cases)
- [Contributing](#contributing)
- [FAQ](#faq)
- [Disclaimer](#disclaimer)
- [License & Author](#license--author)

---

## Why This Plugin?

Modern journalism demands speed without sacrificing accuracy — verifying viral claims, detecting deepfakes, tracing disinformation networks, and producing multimedia content across platforms. Manual workflows can't keep up.

**Four Key Components:**
- **30 specialist agents** across investigative, forensic, multimedia, and distribution domains
- **19 verification agents** organized in 5 tiers for systematic disinformation analysis
- **2 slash commands** for full journalism workflows and dedicated disinformation investigations
- **Master orchestrator** routing queries automatically to the right specialist

**Target Users:** Investigative journalists, fact-checkers, newsroom editors, media analysts, and disinformation researchers.

---

## Domains Covered

| Domain | Coverage |
|--------|----------|
| Investigative Reporting | FOIA requests, document analysis, source development, legal review |
| Fact-Checking | Claim verification, source cross-referencing, evidence grading |
| Disinformation Analysis | Bot detection, narrative tracking, deepfake forensics, financial trails |
| AI Content Forensics | AI-generated text detection, click-farm content, stylometric fingerprinting |
| Foreign Media Analysis | Cross-language translation, PR-sanitization detection, state media patterns |
| Grassroots Intelligence | Human sincerity scoring, troll-army detection, grassroots willowing |
| Verification & Forensics | 19-agent pipeline: timeline analysis, platform tracking, bias assessment |
| Multimedia Production | Automated video (MoviePy, Whisper), data visualization (Plotly, Folium) |
| Content Distribution | Multi-platform formatting (Twitter, TikTok, YouTube, Instagram), SEO |
| Ethics & Editorial | Ethical guidance, legal risk, narrative structure, publication readiness |

---

## Installation

**Requirements:** Claude Code v1.0.33 or later

```bash
# Clone the repository
git clone https://github.com/swarochish/journalism-toolkit.git

# Load the plugin
claude --plugin-dir ./journalism-toolkit
```

**Alternative:** Add to `.claude/settings.json`:
```json
{
  "plugins": ["path/to/journalism-toolkit"]
}
```

---

## Quick Start Commands

**Master Command:**
```
/journalism-toolkit:ultimate-multimedia-journalist
```

**Story Development:**
```
/journalism-toolkit:ultimate-multimedia-journalist
```
Plan and develop stories with investigative reporting, fact-checking, editing, and multimedia.

**Verification & Fact-Checking:**
```
/journalism-toolkit:ultimate-multimedia-journalist verify [topic or URL]
```
Forensic analysis of viral content with interactive dashboards and risk assessment.

**Investigative Reporting:**
```
/journalism-toolkit:ultimate-multimedia-journalist investigate [topic]
```
Multi-week investigations with document analysis, source development, and legal review.

**Multimedia Production:**
```
/journalism-toolkit:ultimate-multimedia-journalist create [content type]
```
Video production, data visualization, and cross-platform content with Python automation.

**Real-Time Monitoring:**
```
/journalism-toolkit:ultimate-multimedia-journalist monitor [topic]
```
Ongoing narrative monitoring with automated alerts.

**Disinformation Analysis:**
```
/journalism-toolkit:disinformation-brain
```
Dedicated interface coordinating 19 forensic sub-agents for comprehensive disinformation detection.

**Investigation Reports:**

Use the `journalism-toolkit:investigation-report-generator` skill to produce self-contained HTML dossiers with a dark editorial theme, interactive navigation, timelines, and evidence cards.

---

## How It Works

```
User Query
    |
journalism-master-orchestrator
    |-> Classifies query by journalism mode
    |-> Routes to specialist agent (1 of 30)
    |   |-> Agent applies domain-specific analysis
    |   |-> Collaborates with other agents as needed
    |   |-> Returns structured output
    |
Structured Response with:
  - Verified facts & source grades
  - Evidence assessment
  - Multimedia assets
  - Distribution-ready content
  - Actionable next steps
```

**Multi-Agent Architecture:** Each journalism domain has dedicated specialist agents. The master orchestrator handles routing; agents collaborate on cross-domain tasks (e.g., an investigation requiring fact-checking, forensic analysis, and multimedia production).

**Tiered Verification Pipeline:** Disinformation investigations use a 5-tier forensic pipeline — from initial narrative analysis through deep financial/technical investigation to real-time monitoring.

---

## What's Inside

### Summary

| Component | Count | Description |
|-----------|-------|-------------|
| Agents | 30 | Specialist agents covering all journalism domains |
| Commands | 2 | Slash commands for journalism workflows |
| Skills | 1 | Reusable investigation report generation |
| **Total** | **33** | |

### Key Agents

| Agent | Domain |
|-------|--------|
| `journalism-master-orchestrator` | Routes queries to appropriate specialist |
| `investigative-reporter` | Lead investigations, FOIA requests, document analysis |
| `fact-checker` | Verify claims, check sources, cross-reference |
| `disinformation-investigation-orchestrator` | Coordinates 19 forensic agents for disinfo analysis |
| `deepfake-forensics-specialist` | Detect manipulated videos, deepfakes, edited media |
| `ai-content-detector` | Detect AI-generated text, click-farm content, synthetic articles |
| `bot-network-detector` | Identify coordinated inauthentic behavior |
| `grassroots-sincerity-analyst` | Evaluate real human accounts for sincerity, troll-army detection |
| `foreign-news-analyst` | Translate foreign news, detect PR-sanitization across languages |
| `financial-trail-investigator` | Trace funding sources, ad revenue, dark money |
| `narrative-timeline-analyst` | Track story emergence, peak periods, geographic spread |
| `video-journalist` | Automated video production (MoviePy, Whisper) |
| `data-visualization-specialist` | Interactive charts, graphs, maps (Plotly, Folium) |
| `visualization-dashboard-generator` | Create interactive HTML investigation reports |

### Key Skills

| Skill | Functionality |
|-------|--------------|
| `investigation-report-generator` | Generate self-contained HTML dossiers with dark editorial theme, interactive navigation, timelines, and evidence cards |

---

## Architecture

```
journalism-master-orchestrator
|-- Core Agents
|   |-- investigative-reporter
|   |-- fact-checker
|   |-- interview-specialist
|   |-- ethics-advisor
|   |-- story-editor
|-- Verification Agents (Tier 1-5)
|   |-- Tier 1: narrative-timeline-analyst, source-ecosystem-mapper, attribution-tracking-specialist
|   |-- Tier 2: deepfake-forensics-specialist, ai-content-detector, bot-network-detector, grassroots-sincerity-analyst, psychological-manipulation-detector, narrative-cluster-analyst, cross-platform-tracker
|   |-- Tier 3: bias-assessment-analyst, foreign-news-analyst, financial-trail-investigator, author-history-profiler, agency-bias-profiler, technical-infrastructure-analyst
|   |-- Tier 4: impact-measurement-analyst, visualization-dashboard-generator
|   |-- Tier 5: real-time-monitoring-coordinator
|-- Multimedia Agents
|   |-- video-journalist
|   |-- data-visualization-specialist
|-- Distribution Agents
    |-- multi-platform-distributor
    |-- seo-optimization-specialist

disinformation-investigation-orchestrator
|-- Coordinates same verification agents for dedicated disinformation workflows
```

---

## Repository Structure

```
journalism-toolkit/
|-- .claude-plugin/plugin.json    Plugin manifest
|-- LICENSE                       MIT License
|-- README.md                     This file
|-- agents/
|   |-- journalism/               29 specialist agents
|   |-- disinformation/           1 orchestrator agent
|-- commands/                     2 slash commands
|-- skills/
    |-- investigation-report-generator/
        |-- SKILL.md
        |-- assets/               HTML report template
        |-- references/           Component library
```

---

## Use Cases

### Investigative Journalists
- Plan multi-month investigations with document analysis, source development, and legal review
- Trace financial trails, dark money, and ownership networks
- Generate evidence packages with interactive dashboards

### Fact-Checkers
- Verify viral claims using 5-tier forensic pipeline
- Detect deepfakes, AI-generated text, and manipulated media
- Assess bot amplification and coordinated inauthentic behavior

### Newsroom Editors
- Evaluate source credibility and institutional bias
- Identify AI-generated or click-farm content before publication
- Cross-check foreign-language sources with PR-sanitization detection

### Disinformation Researchers
- Map influence networks and narrative evolution across platforms
- Separate genuine grassroots voices from troll armies and paid shills
- Analyze state media propaganda patterns (RT, CGTN, IRNA, KCNA)

### Media Analysts
- Quantify reach, engagement, and real-world impact of campaigns
- Track narrative clusters and echo chamber dynamics
- Monitor evolving campaigns with automated alerts

---

## Contributing

Contributions welcome! Here's how to get involved:

### Adding a New Agent

Use the short-form pattern (YAML frontmatter + structured sections):

```markdown
---
name: your-agent-name
description: One-line description
---

# Your Agent Name

**Purpose**: What it does
**Outputs**: What it produces
**When to Use**: When to deploy it (Tier level)
**Key Tools**: Tools and APIs used

## Core Functions

- Function 1
- Function 2
```

### PR Workflow
1. Fork the repository
2. Create a feature branch (`git checkout -b add-agent-name`)
3. Add or update agent files following existing naming convention (`domain-function-role.md`)
4. Update orchestrators and commands to reference new agents
5. Update README agent counts and architecture tree
6. Submit a PR with a clear description of what the agent does and which issue it addresses

### Reporting Issues
- Include the journalism domain and specific use case
- Describe what capability is missing or what isn't working
- Reference relevant existing agents if applicable

---

## FAQ

**Q: Do I need API keys to use this plugin?**
A: The plugin works as a Claude Code agent system. Some agents reference external APIs (GPTZero, DeepL, Sensity AI, etc.) for tool suggestions, but the agents themselves provide analysis frameworks and workflows without requiring API keys.

**Q: How do I choose between `/ultimate-multimedia-journalist` and `/disinformation-brain`?**
A: Use `/ultimate-multimedia-journalist` for general journalism workflows (story development, verification, investigation, multimedia production, monitoring). Use `/disinformation-brain` for dedicated disinformation investigations where you want the full forensic pipeline.

**Q: Can I use individual agents without the orchestrator?**
A: Yes. Each agent is a standalone markdown file that can be referenced directly. The orchestrators coordinate multiple agents for complex workflows, but individual agents work independently for focused tasks.

**Q: How does the bot-to-grassroots pipeline work?**
A: The `bot-network-detector` first classifies accounts as bot or human. Human accounts that show suspicious patterns are then passed to `grassroots-sincerity-analyst` for sincerity scoring (0-100), troll-army detection, and information value assessment.

---

## Disclaimer

This plugin provides journalism analysis tools and workflows for research and educational purposes. It does **not** replace professional editorial judgment. Always independently verify facts, consult legal counsel for sensitive investigations, and follow your organization's editorial standards. The authors accept no liability for decisions made based on this plugin's output.

---

## License & Author

**License:** MIT — Swarochish Chekuri

**Author:** Swarochish Chekuri

**Repository:** https://github.com/swarochish/journalism-toolkit
