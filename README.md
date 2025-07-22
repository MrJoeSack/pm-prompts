# PM Claude Code Library

PM frameworks and commands for Claude Code. Structured prompts based on established methodologies.

## What This Does

This library adds PM-specific commands to Claude Code. You get quick access to frameworks like RICE prioritization, feature specs, and stakeholder communication.

## How PMs Use This

After IT installs this, PMs chat with Claude Code using simple commands:

### The Workflow:
1. Open Claude Code (it's a terminal but you just chat)
2. Type `/feature-spec` or describe what you need
3. Paste your rough notes
4. Copy the structured output back to your document

### Example:
```
You: /feature-spec
You: [paste messy notes about login feature]
Claude: [returns complete PRD with user stories]
```

## Quick Start

**Prerequisites:** Install Claude Code first ([installation guide](docs/installation.md))

**Setup (IT runs once):**
```bash
git clone https://github.com/MrJoeSack/pm-prompts.git .pm-library
cp .pm-library/CLAUDE.md ./CLAUDE.md
cp -r .pm-library/.claude ./
```

Done. PMs can now use Claude Code with PM commands.

👉 Questions? Check the [FAQ](docs/FAQ.md).

## Available Commands

**Core PM Tasks**
- `/strategy-review` - Analyze strategy documents
- `/feature-spec` - Create feature specifications  
- `/stakeholder-sync` - Draft stakeholder communications
- `/research-plan` - Structure user research
- `/prioritization` - Apply RICE, ICE, Kano scoring
- `/customer-feedback` - Synthesize feedback
- `/okr-planning` - Set objectives and key results
- `/competitive-analysis` - Market intelligence
- `/product-launch` - Launch planning

**Complete list:** Type `/pm-help` in Claude Code

## Installation Options

### Project-Specific (Recommended)
```bash
git clone https://github.com/MrJoeSack/pm-prompts.git .pm-library
cp .pm-library/CLAUDE.md ./CLAUDE.md
cp -r .pm-library/.claude ./
```

### Global Access
```bash
mkdir -p ~/.claude-global
git clone https://github.com/MrJoeSack/pm-prompts.git ~/.claude-global/pm-library
# Create symlinks for each project
```

## Documentation

**Getting Started**
- [Installation Guide](docs/installation.md) - Claude Code setup + PM library
- [FAQ](docs/FAQ.md) - Common questions
- [Usage Examples](docs/usage-examples.md) - Step-by-step workflows

**PM Skills**
- [Economical Writing](core/economical-writing.md) - McCloskey's clarity principles
- [Feature Planning](core/feature-planning.md) - Specifications with feasibility
- [Prioritization Methods](core/prioritization-methods.md) - RICE, ICE, Kano
- [Stakeholder Communication](core/stakeholder-communication.md) - Alignment
- [User Research](core/user-research.md) - Research discipline
- [Data Analysis](core/data-analysis.md) - Signal vs noise

**Strategy & Planning**
- [Good Strategy Framework](strategy/good-strategy-framework.md) - Rumelt's kernel
- [Strategic Planning](strategy/strategic-planning.md) - Document structure
- [Roadmap Planning](strategy/roadmap-planning.md) - Systematic roadmapping
- [OKR Framework](strategy/okr-framework.md) - Objective setting
- [Quarterly Planning](strategy/quarterly-planning.md) - Strategic planning
- [Competitive Analysis](strategy/competitive-analysis.md) - Market intelligence

**Product Delivery**
- [PRFAQ Generation](product-delivery/prfaq-generation.md) - Amazon-style announcements
- [Product Launch](product-delivery/product-launch.md) - Launch planning
- [Customer Feedback](product-delivery/customer-feedback.md) - Jobs-to-be-Done
- [Go-to-Market](product-delivery/go-to-market.md) - GTM strategy
- [Focus Discipline](product-delivery/focus-discipline.md) - Prioritization

**Special Situations**
- [Crisis Communication](special-situations/crisis-communication.md) - Crisis response
- [Difficult Conversations](special-situations/difficult-conversations.md) - Challenging discussions
- [Executive Presentations](special-situations/executive-presentations.md) - Executive alignment
- [Stakeholder Mapping](special-situations/stakeholder-mapping.md) - Influence analysis
- [Team Alignment](special-situations/team-alignment.md) - Cross-functional coordination

## What's Included

- **15 Slash Commands** - Quick access to PM tasks  
- **PM Frameworks** - Based on established methodologies  
- **Core Skills** - Writing, planning, prioritization, communication
- **Strategy Tools** - Roadmapping, OKRs, competitive analysis
- **Delivery Support** - PRFAQs, launches, GTM planning
- **Special Situations** - Crisis communication, difficult conversations

## For Teams Considering This

### Benefits
- Faster document creation through templates
- Consistent PM methodology application
- Less time on routine writing

### Implementation
- Natural language interface (no coding)
- IT sets up once
- Start with volunteers

### Evaluation
- Test with small group first
- Measure time savings and quality
- Gather feedback before rollout

---

*PM frameworks and tools for Claude Code.*

## License

MIT License. See LICENSE file.

## Disclaimer

Community project. Not affiliated with Anthropic.