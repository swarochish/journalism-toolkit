[![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)](https://github.com/swarochish/journalism-toolkit)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Claude Code](https://img.shields.io/badge/Claude%20Code-v1.0.33+-purple.svg)](https://claude.com/claude-code)

# Journalism Toolkit for Claude Code

The most comprehensive journalism AI system available as a Claude Code plugin. 27 specialized agents, 2 commands, and 1 analytical skill covering investigative reporting, fact-checking, disinformation analysis, multimedia production, and content distribution.

> One command. Five journalism modes. From tip to publication.

---

## Why This Plugin?

Modern journalism demands speed without sacrificing accuracy — verifying viral claims, detecting deepfakes, tracing disinformation networks, and producing multimedia content across platforms. Manual workflows can't keep up.

**Four Key Components:**
- **27 specialist agents** across investigative, forensic, multimedia, and distribution domains
- **16 verification agents** organized in 5 tiers for systematic disinformation analysis
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
| Verification & Forensics | 16-agent pipeline: timeline analysis, platform tracking, bias assessment |
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
Dedicated interface coordinating 16 forensic sub-agents for comprehensive disinformation detection.

**Investigation Reports:**

Use the `journalism-toolkit:investigation-report-generator` skill to produce self-contained HTML dossiers with a dark editorial theme, interactive navigation, timelines, and evidence cards.

---

## How It Works

```
User Query
    |
journalism-master-orchestrator
    |-> Classifies query by journalism mode
    |-> Routes to specialist agent (1 of 27)
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
| Agents | 27 | Specialist agents covering all journalism domains |
| Commands | 2 | Slash commands for journalism workflows |
| Skills | 1 | Reusable investigation report generation |
| **Total** | **30** | |

### Key Agents

| Agent | Domain |
|-------|--------|
| `journalism-master-orchestrator` | Routes queries to appropriate specialist |
| `investigative-reporter` | Lead investigations, FOIA requests, document analysis |
| `fact-checker` | Verify claims, check sources, cross-reference |
| `disinformation-investigation-orchestrator` | Coordinates 16 forensic agents for disinfo analysis |
| `deepfake-forensics-specialist` | Detect manipulated videos, deepfakes, edited media |
| `bot-network-detector` | Identify coordinated inauthentic behavior |
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
|   |-- Tier 2: deepfake-forensics-specialist, bot-network-detector, psychological-manipulation-detector, narrative-cluster-analyst, cross-platform-tracker
|   |-- Tier 3: bias-assessment-analyst, financial-trail-investigator, author-history-profiler, agency-bias-profiler, technical-infrastructure-analyst
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
|   |-- journalism/               26 specialist agents
|   |-- disinformation/           1 orchestrator agent
|-- commands/                     2 slash commands
|-- skills/
    |-- investigation-report-generator/
        |-- SKILL.md
        |-- assets/               HTML report template
        |-- references/           Component library
```

---

## Contributing

Contributions welcome:
- Add agents following the existing naming convention (e.g., `domain-function-role.md`)
- Improve existing agents ensuring correct cross-references
- Report issues with journalism domain and use case details

---

## Disclaimer

This plugin provides journalism analysis tools and workflows for research and educational purposes. It does **not** replace professional editorial judgment. Always independently verify facts, consult legal counsel for sensitive investigations, and follow your organization's editorial standards. The authors accept no liability for decisions made based on this plugin's output.

---

## License & Author

**License:** MIT — Swarochish Chekuri

**Author:** Swarochish Chekuri

**Repository:** https://github.com/swarochish/journalism-toolkit
