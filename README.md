# PM Claude Code Library

A Claude Code prompt library for product managers. Improve your PM workflow with structured prompts, custom commands, and proven frameworks.

## Why This Exists

Product management requires clear thinking under pressure. This library integrates PM frameworks into Claude Code to support better decision-making.

## 🎯 How PMs Actually Use This (No Command Line Required!)

After one-time setup by IT/Engineering, PMs use Claude Code just like ChatGPT or Slack:

### The Simple Workflow:
1. **Work in your normal tools** (Google Docs, Notion, Jira, etc.)
2. **Open Claude Code** when you need help (it has a chat interface, not a terminal!)
3. **Type a slash command** like `/feature-spec` or `/stakeholder-sync`
4. **Paste your rough notes** or describe what you need
5. **Copy the polished output** back to your document

### Visual Example:
```
[Google Doc with rough notes] → [Claude Code chat: "/feature-spec"] → [Polished PRD]
```

**No coding. No terminal. Just chat and slash commands.**

## 📅 A PM's Typical Day with Claude Code

**9:00 AM - Sprint Planning**
- Copy backlog items into Claude Code
- Type `/prioritization`
- Get RICE scores and recommendations
- Paste organized priorities back into Jira

**11:00 AM - Customer Call Notes**
- Paste messy interview notes
- Type `/customer-feedback`
- Get structured insights with themes and quotes
- Add to research repository

**2:00 PM - Feature Request from Sales**
- Draft rough feature idea
- Type `/feature-spec`
- Receive complete PRD with user stories
- Share with engineering team

**4:00 PM - CEO Asks for Update**
- Brain dump current status
- Type `/stakeholder-sync`
- Get executive-ready email
- Send polished update

## 🚀 Quick Start (One-Time Setup)

**For PMs:** Ask your engineering team to run this one-time setup:

```bash
# Engineering team runs this once
git clone https://github.com/MrJoeSack/pm-prompts.git
cd pm-prompts
# Claude Code automatically loads everything
```

**That's it!** Now any PM can use the slash commands in Claude Code's chat interface.

## Core Capabilities

**🧠 Thinking Frameworks**
- Strategy analysis using Rumelt's Good Strategy principles
- McCloskey's economical writing for clear communication
- User research question discipline
- Data analysis clarity tools

**⚡ Claude Code Integration** 
- Custom slash commands for instant PM workflows
- Automated document review and improvement
- Context-aware prompt application
- Memory integration for consistent project knowledge

**🔄 Workflow Automation Commands**
- `/strategy-review` - Analyze and improve strategy documents
- `/feature-spec` - Transform ideas into complete specifications  
- `/stakeholder-sync` - Create executive-ready communications
- `/research-plan` - Structure user research approaches
- `/roadmap-planning` - Systematic roadmap creation and prioritization
- `/prioritization` - RICE, ICE, and Kano model scoring
- `/customer-feedback` - Synthesize and analyze feedback
- `/okr-planning` - Set objectives and key results
- `/competitive-analysis` - Market intelligence and positioning
- `/product-launch` - Plan and coordinate launches

## Installation Options

### Option 1: Project-Specific (Recommended)
```bash
# IT/Engineering runs this once per project
git clone https://github.com/MrJoeSack/pm-prompts.git .pm-library
cp .pm-library/CLAUDE.md ./CLAUDE.md
cp -r .pm-library/.claude ./
```

### Option 2: Global Access
```bash
# IT sets this up once for all projects
mkdir -p ~/.claude-global
git clone https://github.com/MrJoeSack/pm-prompts.git ~/.claude-global/pm-library
# Create symlinks for each project
```

### Option 3: Direct Integration
```bash
# Quick setup via curl
curl -sSL https://raw.githubusercontent.com/MrJoeSack/pm-prompts/main/install.sh | bash
```

## Navigation

**🚀 Getting Started**
- [Quick Start Guide](quick-start-guide.md) - Get productive in 5 minutes
- [Installation Guide](installation.md) - Setup options and troubleshooting  
- [Usage Examples](usage-examples.md) - Step-by-step workflows
- [Google Docs Integration](google-docs-integration.md) - Copy/paste workflows
- [PM Workflows](pm-workflows.md) - How PMs actually use this library

**📋 Core Frameworks** 
- [Economical Writing](economical-writing.md) - McCloskey's clarity principles
- [Good Strategy Framework](good-strategy-framework.md) - Rumelt's strategy kernel
- [User Research](user-research.md) - Research question discipline with qual/quant methods
- [Feature Planning](feature-planning.md) - Clear specifications with technical feasibility
- [Data Analysis](data-analysis.md) - Signal vs noise with A/B testing design
- [Strategic Planning](strategic-planning.md) - Strategy document structure
- [Stakeholder Communication](stakeholder-communication.md) - Effective alignment

**🎯 Product Operations**
- [Roadmap Planning](roadmap-planning.md) - Systematic roadmapping with RICE prioritization
- [Prioritization Methods](prioritization-methods.md) - RICE, ICE, Kano model frameworks
- [Customer Feedback](customer-feedback.md) - Feedback synthesis and Jobs-to-be-Done
- [OKR Framework](okr-framework.md) - Objective setting and key result tracking
- [Product Launch](product-launch.md) - Launch planning, execution, and optimization
- [Competitive Analysis](competitive-analysis.md) - Market intelligence and positioning

**💼 Advanced PM Scenarios**
- [Difficult Conversations](difficult-conversations.md) - Navigate challenging discussions
- [Executive Presentations](executive-presentations.md) - Structure presentations that drive decisions
- [PRFAQ Generation](prfaq-generation.md) - Amazon-style product announcements
- [Quarterly Planning](quarterly-planning.md) - Strategic planning with capacity planning
- [Stakeholder Mapping](stakeholder-mapping.md) - Influence analysis and coalition building
- [Go-to-Market](go-to-market.md) - GTM strategy, execution, and measurement
- [Crisis Communication](crisis-communication.md) - Crisis response and trust preservation
- [Team Alignment](team-alignment.md) - Cross-functional coordination and collaboration

**⚡ Automation**
- [Usage Examples](usage-examples.md) - Real PM scenarios
- [Workflow Automation](workflow-automation.md) - Systematic processes

## What's Included

📋 **15 Custom Slash Commands** - PM workflow automation  
🧠 **17 Core Frameworks** - Structured thinking tools  
🎯 **6 Product Operations** - Roadmapping, prioritization, feedback, OKRs, launches, competitive analysis  
💼 **8 Advanced Scenarios** - Stakeholder management, GTM, crisis communication, team alignment  
⚡ **Automated Reviews** - Apply multiple frameworks to documents  
📖 **Real Examples** - Practical PM scenarios  

## For Management: Why Your PMs Need This

### Time Savings
- **Feature specs**: 3 hours → 30 minutes
- **Executive updates**: 45 minutes → 10 minutes  
- **Prioritization**: 2 hours → 15 minutes

### Quality & Consistency
- Every PM uses the same proven frameworks
- Junior PMs produce senior-level outputs
- Reduces blind spots in strategy and planning

### Easy Adoption
- **PMs need zero technical skills** - it's just like using ChatGPT
- One-time setup by IT (5 minutes)
- ROI visible within first week

---

*The work is difficult. These tools make it systematic.*