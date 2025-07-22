# Claude Code Usage Examples

*Step-by-step workflows for PMs*

## How Slash Commands Work

**Method 1: With Files**
```bash
# If you have a file
/strategy-review strategy-q4.md
```

**Method 2: With Text Input**
```bash
# Type the command, press enter, then paste/type your content
/strategy-review
[Then paste your Google Doc content or type your text]
```

**Method 3: Direct Request**
```bash
# Just ask Claude to apply frameworks
"Use the strategy-review framework on this document: [paste content]"
```

## Scenario 1: Strategy Document Review

**Situation**: You have a Q4 strategy document in Google Docs that needs review

**Step-by-step:**
1. Copy the strategy document from Google Docs
2. In Claude Code, type: `/strategy-review`
3. Press Enter
4. Paste the document content
5. Claude applies good-strategy-framework and identifies:
   - Vague problem diagnosis ("need to improve user experience")  
   - Goals masquerading as strategy ("increase engagement 15%")
   - Incoherent action list without connecting logic
6. Get specific rewrite suggestions using Rumelt's kernel

## Scenario 2: Feature Specification Creation

**Situation**: You have a rough feature idea that engineering needs as a clear PRD

**Step-by-step:**
1. Type: `/feature-spec`
2. Press Enter
3. Describe your feature idea: "We need to improve user onboarding because too many people drop off during setup"
4. Claude structures it into:
   - **Problem**: New users abandon setup because current flow has 7 steps
   - **Solution**: Build 3-step guided onboarding with progress indicators  
   - **Success**: 80% setup completion (vs current 45%)
   - **Trade-off**: Won't build advanced customization to ship faster
5. Copy the structured output back to your PRD document

## Scenario 3: Stakeholder Email Draft

**Situation**: You need buy-in from legal team for data collection feature

**Step-by-step:**
1. Type: `/stakeholder-sync`
2. Press Enter  
3. Describe the situation: "I need legal approval for user analytics feature we want to build"
4. Claude creates structured email with:
   - **Clear ask**: "Need legal review of user event tracking by Friday"
   - **Context**: Specific data types and usage  
   - **Dependencies**: "Need your sign-off to proceed with engineering"
   - **Next steps**: "I'll schedule 30min review Thursday if questions"
5. Copy the email draft and send

## Scenario 4: Research Planning  

**Situation**: You need to understand why enterprise customers are churning

**Step-by-step:**
1. Type: `/research-plan`
2. Press Enter
3. Describe your research goal: "We want to understand why enterprise customers churn"
4. Claude forces clarity by asking:
   - **Decision this informs**: Should we build admin dashboards or improve onboarding?
   - **What would change mind**: If customers leave due to pricing not features  
   - **Research question**: "Why did you stop using our tool?" (not leading)
   - **Bias check**: Are we assuming it's a feature problem?
5. Use the structured plan for your research interviews

## Key Workflow Tips

**Copy/Paste is Your Friend:**
- Most PM work happens in Google Docs, Notion, or email
- Copy content → Use slash command → Paste improved version back

**Chain Commands Together:**
- `/research-plan` → conduct research → `/data-analysis` → `/feature-spec` → `/stakeholder-sync`
- Strategy informs features, features need stakeholder buy-in, buy-in requires research insights

**File vs. Text Input:**
- Have a saved file? Use `/command filename.md`  
- Working with Google Docs? Use `/command` then paste content
- Quick question? Just ask "Apply the X framework to this: [content]"