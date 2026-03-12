# Component Library

HTML component snippets for investigation report dossiers. Copy-paste these into your report template.

---

## Hero Section

```html
<div class="hero">
  <div class="hero-badge">Investigative Dossier</div>
  <h1>The <span>Subject</span> Investigation</h1>
  <p class="subtitle">A comprehensive investigation into...</p>
  <div class="hero-stats">
    <div class="hero-stat"><span class="num">$10M</span><span class="label">Amount</span></div>
    <div class="hero-stat"><span class="num" style="color:var(--red)">15</span><span class="label">Violations</span></div>
    <div class="hero-stat"><span class="num">42</span><span class="label">Documents</span></div>
  </div>
</div>
```

Use `style="color:var(--red)"` on `.num` spans to highlight alarming statistics.

---

## Sticky Navigation

```html
<nav class="toc">
  <div class="toc-inner">
    <a href="#origins">Origins</a>
    <a href="#evidence">Evidence</a>
    <a href="#analysis">Analysis</a>
    <a href="#conclusions">Conclusions</a>
  </div>
</nav>
```

---

## Section Header

```html
<section id="section-id">
<div class="container">
  <div class="section-num">Part 01</div>
  <h2>Section <span>Title</span></h2>
  <p>Introductory paragraph...</p>
</div>
</section>
```

The word wrapped in `<span>` gets the gold accent color.

---

## Cards

### Accent Card (gold)
```html
<div class="card card-accent">
  <div class="card-title">Key Finding</div>
  <p style="margin:0">Description with <strong>emphasis</strong>.</p>
</div>
```

### Red Card (alert/danger)
```html
<div class="card card-red">
  <div class="card-title" style="color:var(--red)">Critical Finding</div>
  <p style="margin:0">Serious allegation or confirmed violation.</p>
</div>
```

### Blue Card (informational)
```html
<div class="card card-blue">
  <div class="card-title" style="color:var(--blue)">Context</div>
  <p style="margin:0">Background information.</p>
</div>
```

### Green Card (verified/positive)
```html
<div class="card card-green">
  <div class="card-title" style="color:var(--green)">Verified</div>
  <p style="margin:0">Confirmed by multiple sources.</p>
</div>
```

---

## Grid Layouts

### Two-Column Grid
```html
<div class="grid-2">
  <div class="card card-red">
    <div class="card-title" style="color:var(--red)">Finding A</div>
    <p style="margin:0">Description</p>
  </div>
  <div class="card card-red">
    <div class="card-title" style="color:var(--red)">Finding B</div>
    <p style="margin:0">Description</p>
  </div>
</div>
```

### Three-Column Grid
```html
<div class="grid-3">
  <div class="card card-accent"><div class="card-title">Item 1</div><p style="margin:0">...</p></div>
  <div class="card card-accent"><div class="card-title">Item 2</div><p style="margin:0">...</p></div>
  <div class="card card-accent"><div class="card-title">Item 3</div><p style="margin:0">...</p></div>
</div>
```

Both grids collapse to single-column on mobile (768px breakpoint).

---

## Data Tables

```html
<div style="overflow-x:auto">
<table>
  <thead>
    <tr><th>Name</th><th>Role</th><th>Status</th></tr>
  </thead>
  <tbody>
    <tr><td>Subject Name</td><td>Position</td><td><span class="tag tag-active">Active</span></td></tr>
    <tr><td>Subject Name</td><td>Position</td><td><span class="tag tag-review">Under Review</span></td></tr>
  </tbody>
</table>
</div>
```

Always wrap tables in `<div style="overflow-x:auto">` for mobile scrolling.

---

## Tags

```html
<span class="tag tag-active">Active</span>
<span class="tag tag-cancelled">Cancelled</span>
<span class="tag tag-review">Under Review</span>
<span class="tag tag-operational">Operational</span>
<span class="tag tag-stalled">Stalled</span>
<span class="tag tag-disputed">Disputed</span>
```

---

## Timeline

```html
<div class="timeline">
  <div class="timeline-item">
    <div class="timeline-date">2024-01-15</div>
    <div class="timeline-text">Initial report filed with regulatory authority</div>
  </div>
  <div class="timeline-item">
    <div class="timeline-date">2024-03-22</div>
    <div class="timeline-text"><strong>Key event</strong> with significant implications</div>
  </div>
  <div class="timeline-item">
    <div class="timeline-date">2024-06-10</div>
    <div class="timeline-text">Follow-up investigation launched</div>
  </div>
</div>
```

---

## Flow Diagram

```html
<div class="flow-diagram">
  <span class="node">Source Entity</span>
  <span class="arrow">&rarr;</span>
  <span class="node">Shell Company A</span>
  <span class="arrow">&rarr;</span>
  <span class="node">Shell Company B</span>
  <span class="arrow">&rarr;</span>
  <span class="node">Final Recipient</span>
</div>
```

---

## Network Box

For ASCII-style relationship diagrams:

```html
<div class="network-box">
                    [Subject A]
                   /           \
          [Entity B]          [Entity C]
         /    |    \              |
   [Sub-1] [Sub-2] [Sub-3]   [Sub-4]
</div>
```

---

## Callouts

### Gold Callout (emphasis)
```html
<div class="callout">
  Key quote or critical observation that deserves special attention.
</div>
```

### Red Callout (warning)
```html
<div class="callout callout-red">
  Critical warning or alarming finding that requires immediate attention.
</div>
```

---

## Verdict Badges

```html
<span class="verdict verdict-red">Confirmed Violation</span>
<span class="verdict verdict-orange">Under Investigation</span>
```

---

## Collapsible Details

```html
<details>
  <summary>Supplementary Evidence: Document Analysis</summary>
  <div class="detail-body">
    <p>Detailed analysis of documents obtained through FOIA requests...</p>
    <table>
      <thead><tr><th>Document</th><th>Date</th><th>Relevance</th></tr></thead>
      <tbody>
        <tr><td>Internal Memo #142</td><td>2024-02-15</td><td>Shows prior knowledge</td></tr>
      </tbody>
    </table>
  </div>
</details>
```

---

## Footer

```html
<footer>
  <div class="container">
    <p>Investigation Report &mdash; Generated [Date] &mdash; Confidential</p>
  </div>
</footer>
```

---

## CSS Variables Reference

Override these in `:root` to customize the theme:

| Variable | Default | Purpose |
|----------|---------|---------|
| `--bg-primary` | `#0a0a0f` | Page background |
| `--bg-secondary` | `#12121a` | Navigation background |
| `--bg-card` | `#1a1a2e` | Card background |
| `--bg-highlight` | `#16213e` | Highlighted elements |
| `--text-primary` | `#e0e0e0` | Main text |
| `--text-secondary` | `#a0a0b0` | Secondary text |
| `--text-muted` | `#6a6a7a` | Muted labels |
| `--accent` | `#c9a84c` | Gold accent |
| `--accent-dim` | `#8a6d2b` | Dim gold |
| `--red` | `#e74c3c` | Alerts and danger |
| `--green` | `#27ae60` | Verified/success |
| `--blue` | `#3498db` | Informational |
| `--orange` | `#e67e22` | Warnings |
| `--purple` | `#9b59b6` | Special highlights |
| `--border` | `#2a2a3e` | Subtle borders |
| `--border-accent` | `#3a3a5e` | Accent borders |
