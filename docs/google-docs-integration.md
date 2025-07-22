# Google Docs Integration Guide

*How to use this library with your existing Google Docs workflow*

## Copy-Paste Method (Recommended)

**Step 1: Export from Google Docs**
```
File → Download → Plain text (.txt)
```
Or select all text and copy directly.

**Step 2: Use with Claude Code**
```
# Paste content then apply framework
/strategy-review
[paste your Google Doc content here]

# Or reference frameworks directly  
"Apply the economical-writing prompt to this document:
[paste content]"
```

## Direct Analysis Pattern

**Common workflow:**
1. Copy Google Doc content
2. Ask Claude to apply specific prompt: "Use the stakeholder-communication framework to improve this email draft"
3. Get revised version with explanations
4. Copy improvements back to Google Doc

## File-Based Workflow

**For regular documents:**
```bash
# Download as .txt, then
/prd-review downloaded-doc.txt

# Or create local copy
echo "Google Doc content" > strategy-draft.md
/strategy-review strategy-draft.md
```

## Integration Examples

**Strategy Review:**
```
"I have a strategy doc from Google Docs. Apply the good-strategy-framework to identify issues:

[paste full Google Doc content]"
```

**PRD Improvement:**
```
/prd-review
[paste Google Doc PRD content]
```

**Email Draft Polish:**
```
"Use economical-writing principles to improve this stakeholder email:

[paste Google Doc email draft]"
```

## Best Practices

- Copy just the relevant section for focused feedback
- Include document context ("this is a Q4 strategy doc for the mobile team")
- Apply one framework at a time for clearer feedback
- Keep original in Google Docs, iterate with Claude Code input

This bridges your existing Google Docs workflow with systematic PM frameworks.