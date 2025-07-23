# Markdown Export Workflows

Complete guide for creating and managing PM documents as local markdown files with Claude Code.

## Why Markdown?

**Simple and Portable**
- Works in any text editor
- Version control friendly
- Easy to share and collaborate
- Converts to any format (PDF, HTML, Word)

**Professional Output**
- Clean formatting with headers, tables, and lists
- Readable in plain text or rendered
- Compatible with documentation tools
- Searchable and indexable

## Quick Reference

### Export Types
- **Research Reports** → Competitive analysis, market intelligence
- **Planning Documents** → Strategy reviews, roadmaps, OKRs
- **Analysis Files** → RICE prioritization, SWOT analysis
- **Project Documentation** → PRDs, launch plans, stakeholder maps

### Common Workflows
- **Competitive Intelligence** → `/competitor-research` → `/markdown-export`
- **Strategy Planning** → `/strategy-review` → `/markdown-export`
- **Feature Planning** → `/feature-spec` → `/markdown-export`
- **Customer Research** → `/customer-feedback` → `/markdown-export`

## Export Workflows

### 1. Competitive Intelligence Reports
```
You: /competitor-research
You: Competitor: [company] vs [your company]
Claude: [Complete competitive analysis]

You: /markdown-export
You: Directory: C:\Users\joesa\Documents\Research
You: Type: competitive analysis
Claude: [Creates formatted markdown file]
```

**Output Example:**
- `Competitor_vs_YourCompany_Analysis.md`
- Executive summary, detailed analysis, recommendations
- Tables for feature/pricing comparisons
- Strategic action items with timelines

### 2. Strategy Documents
```
You: /strategy-review
You: [Paste strategy content]
Claude: [Analyzes using Good Strategy framework]

You: /markdown-export
You: Directory: C:\temp
You: Type: strategy review
Claude: [Creates structured strategy document]
```

**Output Structure:**
- Situation diagnosis
- Strategic approach
- Implementation plan
- Success metrics

### 3. Feature Planning
```
You: /feature-spec
You: Feature: [description]
Claude: [Creates complete PRD]

You: /markdown-export
You: Directory: C:\Users\joesa\Documents\Features
You: Title: Feature_Authentication_PRD
Claude: [Exports formatted specification]
```

**Output Includes:**
- User stories and acceptance criteria
- Technical requirements
- Success metrics
- Implementation timeline

### 4. Research Synthesis
```
You: /customer-feedback
You: [Paste interview notes]
Claude: [Synthesizes insights]

You: /markdown-export
You: Directory: C:\temp
You: Type: research summary
Claude: [Creates insights report]
```

**Output Format:**
- Key findings and themes
- Customer quotes and evidence
- Recommendations and next steps
- Methodology and sources

## File Organization Best Practices

### Directory Structure
```
C:\Users\[name]\Documents\PM-Work\
├── Competitive-Analysis\
│   ├── 2025-Q1-Competitors\
│   └── Threat-Assessments\
├── Strategy\
│   ├── Quarterly-Reviews\
│   └── Product-Strategy\
├── Features\
│   ├── PRDs\
│   └── Technical-Specs\
├── Research\
│   ├── Customer-Insights\
│   └── Market-Analysis\
└── Planning\
    ├── Roadmaps\
    └── OKRs\
```

### Naming Conventions
**Competitive Analysis:**
- `[Competitor]_vs_[Company]_[Date].md`
- `Market_Analysis_[Sector]_[Quarter].md`

**Strategy Documents:**
- `[Quarter]_Strategy_Review.md`
- `Product_Strategy_[Year].md`

**Feature Planning:**
- `PRD_[Feature]_[Version].md`
- `Spec_[Feature]_Technical.md`

**Research Reports:**
- `Customer_Research_[Topic]_[Date].md`
- `Market_Intelligence_[Sector].md`

## Markdown Features for PM Work

### Tables for Comparisons
```markdown
| Feature | Us | Competitor | Advantage |
|---------|-------|------------|-----------|
| Performance | 50ms | 100ms | 2x faster |
| Cost | $10/user | $20/user | 50% cheaper |
```

### Priority Lists
```markdown
## Immediate Actions (0-3 months)
1. **Performance optimization** - Critical path item
2. **Pricing analysis** - Competitive response needed
3. **Feature gap assessment** - Market positioning

## Medium-term Strategy (3-12 months)
- Market expansion opportunities
- Product differentiation initiatives
- Partnership evaluation
```

### Status Tracking
```markdown
## Action Items
- [ ] Competitive benchmark analysis (Due: Q1)
- [x] Customer interview synthesis (Complete)
- [ ] Pricing model review (In Progress)
```

## Integration with Other Tools

### Version Control
```bash
# Initialize git repo for PM documents
git init
git add *.md
git commit -m "Add Q1 competitive analysis"
```

### Convert to Other Formats
```bash
# Convert to PDF using pandoc
pandoc analysis.md -o analysis.pdf

# Convert to Word
pandoc analysis.md -o analysis.docx
```

### Share with Stakeholders
- **Email attachments** - MD files open in most editors
- **Copy-paste** - Markdown renders well in Slack, GitHub, Notion
- **Documentation sites** - Upload to GitBook, Confluence, etc.

## Common Use Cases

### Weekly Planning
```
You: /markdown-export
You: Directory: C:\temp
You: Type: weekly plan
You: Content: [team planning notes]
→ Creates structured weekly plan document
```

### Quarterly Reviews
```
You: /strategy-review
You: [Q3 performance data]
Claude: [Strategic analysis]

You: /markdown-export
You: Directory: C:\Users\joesa\Documents\Strategy
You: Title: Q3_2025_Review
→ Creates executive-ready strategy document
```

### Stakeholder Updates
```
You: /stakeholder-sync
You: [project status updates]
Claude: [Executive communication]

You: /markdown-export
You: Directory: C:\temp
You: Type: stakeholder update
→ Creates professional update document
```

## Tips for Better Markdown

### Use Clear Headers
```markdown
# Executive Summary
## Key Findings
### Market Position
```

### Include Metadata
```markdown
---
Date: January 2025
Author: PM Team
Classification: Internal
Review Date: March 2025
---
```

### Add Navigation
```markdown
## Table of Contents
1. [Executive Summary](#executive-summary)
2. [Analysis](#analysis)
3. [Recommendations](#recommendations)
```

---

*Use `/markdown-export` to create professional PM documents in markdown format.*