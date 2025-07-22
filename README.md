# PM Claude Code Library

A Claude Code prompt library for product managers. Improve your PM workflow with structured prompts, custom commands, and proven frameworks.

## Why This Exists

Product management requires clear thinking under pressure. This library integrates PM frameworks into Claude Code to support better decision-making.

## 🎯 How PMs Actually Use This (No Command Line Knowledge Required!)

After one-time setup by IT/Engineering, PMs use Claude Code through simple chat:

### What Claude Code Actually Looks Like:
Yes, Claude Code runs in a terminal window, but **you just chat with it** - no coding needed!
- You'll see a command prompt, but you type in plain English
- It responds like ChatGPT, but with PM superpowers
- Slash commands (like `/feature-spec`) are just shortcuts

### The Simple Workflow:
1. **Work in your normal tools** (Google Docs, Notion, Jira, etc.)
2. **Open Claude Code** (yes it's a terminal, but you just chat in it!)
3. **Type a slash command** like `/feature-spec` or just describe what you need
4. **Paste your rough notes** or explain your situation
5. **Copy the polished output** back to your document

### Visual Workflow:
```
┌─────────────────────┐     ┌─────────────────────────┐     ┌─────────────────────┐
│   Google Doc        │     │   Claude Code Terminal  │     │   Google Doc        │
│                     │     │                         │     │                     │
│ "need to spec out   │     │ $ claude                │     │ Feature: User Login │
│  user login feature │     │                         │     │                     │
│  - should be secure │ --> │ You: /feature-spec      │ --> │ Overview:           │
│  - integrate with   │     │      [paste notes]      │     │ Secure auth system  │
│    our SSO"         │     │                         │     │ integrating with    │
│                     │     │ Claude: Here's your PRD:│     │ existing SSO...     │
│                     │     │ [structured output]     │     │                     │
└─────────────────────┘     └─────────────────────────┘     └─────────────────────┘
     Rough Notes              Chat with Claude Code           Polished PRD
```

**Think of it like:** Opening Slack in a terminal - yes it's a terminal window, but you're just chatting!

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

**Prerequisites:** Claude Code must be installed first ([see installation guide](docs/installation.md))

**For PMs:** Ask your engineering team to run this one-time setup:

```bash
# Engineering team runs this once in your project folder
git clone https://github.com/MrJoeSack/pm-prompts.git .pm-library
cp .pm-library/CLAUDE.md ./CLAUDE.md
cp -r .pm-library/.claude ./
```

**That's it!** Now any PM can open Claude Code and start chatting with their AI PM assistant.

👉 **New to Claude Code?** Check our [FAQ](docs/FAQ.md) for why it's better than ChatGPT/Gemini for PM work.

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
- [Quick Start Guide](docs/quick-start-guide.md) - Get productive in 5 minutes
- [Installation Guide](docs/installation.md) - Claude Code setup + PM library install
- [FAQ](docs/FAQ.md) - Why Claude Code? Common questions answered
- [Usage Examples](docs/usage-examples.md) - Step-by-step workflows
- [Google Docs Integration](docs/google-docs-integration.md) - Copy/paste workflows
- [PM Workflows](docs/pm-workflows.md) - How PMs actually use this library

**📋 Core PM Skills**
- [Economical Writing](core/economical-writing.md) - McCloskey's clarity principles
- [Feature Planning](core/feature-planning.md) - Clear specifications with technical feasibility
- [Prioritization Methods](core/prioritization-methods.md) - RICE, ICE, Kano model frameworks
- [Stakeholder Communication](core/stakeholder-communication.md) - Effective alignment
- [User Research](core/user-research.md) - Research question discipline with qual/quant methods
- [Data Analysis](core/data-analysis.md) - Signal vs noise with A/B testing design

**🎯 Strategy & Planning**
- [Good Strategy Framework](strategy/good-strategy-framework.md) - Rumelt's strategy kernel
- [Strategic Planning](strategy/strategic-planning.md) - Strategy document structure
- [Roadmap Planning](strategy/roadmap-planning.md) - Systematic roadmapping with RICE prioritization
- [OKR Framework](strategy/okr-framework.md) - Objective setting and key result tracking
- [Quarterly Planning](strategy/quarterly-planning.md) - Strategic planning with capacity planning
- [Competitive Analysis](strategy/competitive-analysis.md) - Market intelligence and positioning

**🚀 Product Delivery**
- [PRFAQ Generation](product-delivery/prfaq-generation.md) - Amazon-style product announcements
- [Product Launch](product-delivery/product-launch.md) - Launch planning, execution, and optimization
- [Customer Feedback](product-delivery/customer-feedback.md) - Feedback synthesis and Jobs-to-be-Done
- [Go-to-Market](product-delivery/go-to-market.md) - GTM strategy, execution, and measurement
- [Focus Discipline](product-delivery/focus-discipline.md) - Systematic prioritization

**💼 Special Situations**
- [Crisis Communication](special-situations/crisis-communication.md) - Crisis response and trust preservation
- [Difficult Conversations](special-situations/difficult-conversations.md) - Navigate challenging discussions
- [Executive Presentations](special-situations/executive-presentations.md) - Structure presentations that drive decisions
- [Stakeholder Mapping](special-situations/stakeholder-mapping.md) - Influence analysis and coalition building
- [Team Alignment](special-situations/team-alignment.md) - Cross-functional coordination and collaboration

**⚡ Automation**
- [Usage Examples](docs/usage-examples.md) - Real PM scenarios
- [Workflow Automation](docs/workflow-automation.md) - Systematic processes

## What's Included

📋 **15 Custom Slash Commands** - PM workflow automation  
🧠 **17 Core Frameworks** - Structured thinking tools  
🎯 **6 Core PM Skills** - Writing, planning, prioritization, communication, research, analysis
📊 **6 Strategy & Planning** - Strategy frameworks, roadmapping, OKRs, quarterly planning
🚀 **5 Product Delivery** - PRFAQs, launches, feedback, GTM, focus discipline
💼 **5 Special Situations** - Crisis communication, difficult conversations, executive alignment  
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