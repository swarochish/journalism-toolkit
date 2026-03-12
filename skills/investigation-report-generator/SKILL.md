---
name: investigation-report-generator
description: Generate comprehensive HTML investigation dossiers with dark theme, interactive navigation, timelines, network diagrams, and evidence cards
---

# Investigation Report Generator

Generate a self-contained HTML investigation dossier. These reports feature a dark theme with gold accents, sticky navigation, collapsible sections, and responsive layouts.

## Workflow

1. **Copy the template**: Start from `assets/report-template.html`
2. **Customize the hero section**: Replace `{{TITLE}}`, `{{SUBTITLE}}`, `{{BADGE}}`, and hero stats
3. **Populate sections**: Use components from `references/component-library.md` to build each section
4. **Update navigation**: Add section anchors to the sticky `<nav class="toc">` bar
5. **Update footer**: Replace `{{FOOTER_TEXT}}` with investigation metadata

## Available Components

See `references/component-library.md` for copy-paste HTML snippets:

- **Hero section** with badge, title, subtitle, and stat counters
- **Sticky table of contents** navigation bar
- **Section headers** with part numbers and accent-colored titles
- **Cards** (accent, red, blue, green variants) for key findings
- **Data tables** with hover effects and sortable columns
- **Timeline** with dated entries and vertical connector line
- **Flow diagrams** with node boxes and arrows
- **Network boxes** for ASCII relationship maps
- **Callouts** (gold accent or red warning)
- **Verdict badges** (red, orange) for assessments
- **Tags** (active, cancelled, review, operational, stalled, disputed)
- **Collapsible details** sections for supplementary evidence
- **Grid layouts** (2-column and 3-column, responsive)

## CSS Variables

The template uses CSS custom properties for consistent theming:

```css
--bg-primary: #0a0a0f      /* Page background */
--bg-secondary: #12121a    /* Nav background */
--bg-card: #1a1a2e         /* Card background */
--bg-highlight: #16213e    /* Highlighted elements */
--text-primary: #e0e0e0    /* Main text */
--text-secondary: #a0a0b0  /* Secondary text */
--text-muted: #6a6a7a      /* Muted labels */
--accent: #c9a84c          /* Gold accent */
--accent-dim: #8a6d2b      /* Dim gold */
--red: #e74c3c             /* Alert/danger */
--green: #27ae60           /* Success/verified */
--blue: #3498db            /* Info */
--orange: #e67e22          /* Warning */
--purple: #9b59b6          /* Special */
--border: #2a2a3e          /* Subtle borders */
--border-accent: #3a3a5e   /* Accent borders */
```

## Guidelines

- Keep reports self-contained (single HTML file, no external dependencies)
- Use semantic section IDs for navigation anchors
- Include a sticky table of contents for long reports
- Use cards for key findings, tables for structured data, timelines for chronology
- Apply appropriate tag colors for status indicators
- Use collapsible `<details>` for supplementary evidence to keep the report scannable
- All text content should be factual and evidence-based
