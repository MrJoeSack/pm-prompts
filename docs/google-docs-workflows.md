# Google Docs Integration Workflows

Complete guide for importing from and exporting to Google Docs and Sheets with Claude Code.

## Quick Reference

### Import Workflows
- **Strategy Review**: Import Google Docs for analysis using Good Strategy framework
- **Data Analysis**: Import Google Sheets for RICE prioritization and metrics review
- **Customer Research**: Import interview notes and feedback for synthesis
- **Competitive Intelligence**: Import market research docs for analysis

### Export Workflows
- **Research Reports** → Google Docs (formatted for sharing)
- **Prioritization Results** → Google Sheets (with calculations)
- **Strategy Documents** → Google Docs (executive-ready)
- **Planning Matrices** → Google Sheets (interactive data)

## Import Workflows

### 1. Strategy Document Analysis
```
You: /google-docs-integration
You: Import: [Google Docs URL with strategy document]
You: Apply Rumelt's Good Strategy framework analysis
Claude: [Analyzes strategy using diagnosis/policy/action kernel]
```

**What I'll analyze:**
- Strategy clarity and coherence
- Problem diagnosis quality
- Policy alignment with diagnosis
- Action plan specificity
- Missing elements and recommendations

### 2. Customer Research Synthesis
```
You: /google-docs-integration
You: Import: [Google Docs URL with interview notes]
You: Synthesize using Jobs-to-be-Done framework
Claude: [Extracts insights, themes, and job statements]
```

**What I'll extract:**
- Customer job statements
- Pain points and motivations
- Outcome expectations
- Behavioral patterns
- Feature implications

### 3. Competitive Intelligence Import
```
You: /google-docs-integration
You: Import: [Google Docs URL with market research]
You: Create competitive positioning analysis
Claude: [Structures data for strategic insights]
```

**What I'll process:**
- Competitor feature comparisons
- Market positioning gaps
- Pricing analysis
- Strategic recommendations

## Export Workflows

### 1. Competitive Research Reports (Google Docs)

**Input Example:**
```
You: /google-docs-integration
You: Export competitive research report to Google Docs format
You: [Paste analysis like the Turbopuffer vs Elasticsearch report]
Claude: [Formats for Google Docs with proper structure]
```

**Output Structure:**
```markdown
# Competitive Intelligence Report: [Competitor] vs [Your Company]

## Executive Summary
- Key findings (3-4 bullet points)
- Strategic implications
- Recommended actions

## Detailed Analysis
### Product Comparison
[Feature comparison table]

### Market Positioning
[Positioning analysis]

### Pricing Analysis
[Cost comparison and implications]

## Strategic Recommendations
### Immediate Actions (0-3 months)
### Medium-term Strategy (3-12 months)
### Long-term Considerations (12+ months)

## Appendix
### Data Sources
### Methodology
### Next Review Date
```

### 2. Prioritization Matrices (Google Sheets)

**Input Example:**
```
You: /google-docs-integration
You: Export feature prioritization to Google Sheets
You: Features: [list of features with RICE scores]
Claude: [Creates spreadsheet format with formulas]
```

**Output Structure:**
```
Column A: Feature Name
Column B: Reach (estimated users)
Column C: Impact (1-3 scale)
Column D: Confidence (% certainty)
Column E: Effort (person-months)
Column F: RICE Score (formula: B*C*D/E)
Column G: Priority Rank (auto-sorted)
Column H: Status
Column I: Owner
Column J: Notes
```

### 3. Strategy Review Documents (Google Docs)

**Output Structure:**
```markdown
# Strategy Review: [Topic]
Date: [Current Date]

## Current Situation
### Market Context
### Competitive Landscape
### Internal Capabilities

## Strategic Analysis
### Diagnosis (What's really happening?)
### Policy (Our approach)
### Actions (Specific next steps)

## Recommendations
### Continue (What's working)
### Stop (What to eliminate)
### Start (New initiatives)

## Success Metrics
### Leading Indicators
### Lagging Indicators
### Review Schedule
```

### 4. OKR Planning Sheets (Google Sheets)

**Output Structure:**
```
Tab 1: Quarterly OKRs
- Objective | Key Result 1 | Key Result 2 | Key Result 3 | Owner | Status

Tab 2: Progress Tracking
- Week | KR Progress | Confidence | Blockers | Actions

Tab 3: Calculations
- Completion % formulas
- Confidence trending
- Risk indicators
```

## Integration Best Practices

### For Imports
1. **Share Settings**: Set Google Docs/Sheets to "Anyone with link can view"
2. **URL Format**: Use full shareable URLs
3. **Content Structure**: Well-organized docs work better for analysis
4. **Context Provision**: Tell me what specific analysis you need

### For Exports
1. **Audience Clarity**: Specify if for team, executives, or stakeholders
2. **Format Preference**: Docs for reports, Sheets for data/calculations
3. **Update Frequency**: Mention if this needs regular updates
4. **Action Items**: Include next steps and owners

## Document Templates

### Competitive Analysis Template (Google Docs)
- Executive Summary (1 page)
- Detailed Analysis (2-3 pages)
- Strategic Implications (1 page)
- Recommended Actions (1 page)

### Feature Prioritization Template (Google Sheets)
- RICE scoring matrix
- Priority rankings
- Resource allocation
- Timeline planning

### Strategy Review Template (Google Docs)
- Situation analysis
- Strategic options
- Recommendations
- Implementation plan

### OKR Planning Template (Google Sheets)
- Objective setting
- Key result tracking
- Progress monitoring
- Performance analysis

## Common Use Cases

### Weekly Planning
```
You: /google-docs-integration
You: Import team's weekly planning doc
You: Export prioritized task list to Google Sheets
```

### Quarterly Reviews
```
You: /google-docs-integration
You: Import Q3 performance data
You: Export strategy recommendations to Google Docs for leadership
```

### Customer Research
```
You: /google-docs-integration
You: Import customer interview notes
You: Export insights summary to Google Docs with recommendations
```

### Competitive Monitoring
```
You: /google-docs-integration
You: Export monthly competitive update to Google Docs
You: Include market changes and strategic implications
```

## Security and Sharing

### Document Access
- Use "Anyone with link" for imports
- Consider "Restricted" sharing for sensitive exports
- Include document expiration dates for confidential analysis

### Data Handling
- Claude Code processes locally
- No data retention beyond session
- Export formats are provided as text for you to paste

### Best Practices
- Review sharing permissions before import
- Add document version dates
- Include data sources and methodology
- Set regular review schedules for exported documents

---

*Use `/google-docs-integration` to start working with Google Docs and Sheets in your PM workflow.*