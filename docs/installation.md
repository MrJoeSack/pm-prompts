# Installation & Setup Guide

Complete setup instructions for Claude Code and the PM library.

## Step 1: Install Claude Code

**IT/Engineering installs:**

1. **Download** Claude Code from [claude.ai/code](https://claude.ai/code)
   - Available for Mac, Windows, Linux
   - Requires Claude Pro or Team subscription

2. **Install** the application
   - Mac: Drag to Applications
   - Windows: Run installer
   - Linux: Follow package instructions

3. **Sign in** with Anthropic account
   - Use work email for team subscription
   - Or personal Claude Pro account

4. **Verify** installation
   ```bash
   claude --version
   ```

## Step 2: Test Claude Code

**What PMs need to know:**
- Claude Code opens in terminal but accepts natural language
- You type in plain English, not code
- It reads and edits files on your computer
- Everything processes locally

**Quick test:**
1. Open terminal, type `claude`
2. Ask "What files are in this folder?"
3. It lists your files

## Step 3: Install PM Library

Add PM frameworks to Claude Code:

### Option 1: Project-Specific (Recommended)
```bash
# In your product management project folder
git clone https://github.com/MrJoeSack/pm-prompts.git .pm-library
cp .pm-library/CLAUDE.md ./CLAUDE.md  
cp -r .pm-library/.claude ./
```

### Option 2: Global Access
```bash  
# Install once, use everywhere
cd ~
git clone https://github.com/MrJoeSack/pm-prompts.git
ln -s ~/pm-prompts/CLAUDE.md ~/.claude/CLAUDE.md
ln -s ~/pm-prompts/.claude/commands ~/.claude/commands
```

### Option 3: Quick Install
```bash
# Download essentials only
curl -o CLAUDE.md https://raw.githubusercontent.com/MrJoeSack/pm-prompts/main/CLAUDE.md
mkdir -p .claude/commands
cd .claude/commands
curl -O https://raw.githubusercontent.com/MrJoeSack/pm-prompts/main/.claude/commands/feature-spec.md
curl -O https://raw.githubusercontent.com/MrJoeSack/pm-prompts/main/.claude/commands/stakeholder-sync.md
```

## Step 4: Verify Setup

Test everything works:

1. **Open Claude Code**
   ```bash
   claude
   ```

2. **Try PM commands**
   - Type: `/pm-help` (lists all commands)
   - Type: `/feature-spec` (asks for feature details)
   - Ask: "What PM frameworks do you have?"

3. **Check context**
   - Should list economical writing, good strategy, etc.

## For PMs: First Session

1. **Open terminal**
2. **Navigate to project** 
   ```bash
   cd /path/to/your/project
   ```
3. **Start Claude Code**
   ```bash
   claude
   ```
4. **Try first command**
   ```
   You: /feature-spec
   You: I need to spec out user authentication
   Claude: [Provides structured PRD template]
   ```

## For IT: Team Deployment

### Individual Setup
- Install Claude Code on each PM's machine
- Clone library to shared location
- Create symlinks for each user

### Team Deployment
```bash
# Create shared library
sudo mkdir -p /opt/pm-claude-library
sudo git clone https://github.com/MrJoeSack/pm-prompts.git /opt/pm-claude-library

# For each user
ln -s /opt/pm-claude-library/CLAUDE.md ~/.claude/CLAUDE.md
ln -s /opt/pm-claude-library/.claude/commands ~/.claude/commands
```

### Security Considerations
- Claude Code processes files locally
- You control what data gets shared
- Set file permissions appropriately
- Can restrict folder access
- All actions logged in terminal history

## Customization

### Add Company Commands
Create `.claude/commands/your-command.md`:
```markdown
---
name: company-prfaq
description: Generate PRFAQ in our format
---

Generate PRFAQ with:
- Problem Statement
- Customer Benefits  
- Internal Benefits
- FAQ (5-7 questions)

Use professional but approachable tone.
```

### Extend PM Context
Add to `CLAUDE.md`:
```markdown
## Company PM Standards
- All PRDs include success metrics
- Use DACI for decision docs
- Feature flags required for launches
- Include privacy review section
```

## Troubleshooting

**"Command not found: claude"**
- Claude Code not installed or not in PATH
- Try full path: `/Applications/Claude.app/Contents/MacOS/claude`

**Slash commands not working**
- Check `.claude/commands/` directory exists
- Verify commands have `.md` extension
- Restart Claude Code

**"No PM context available"**
- Ensure CLAUDE.md in current directory
- Or in `~/.claude/CLAUDE.md` for global access

**Performance issues**
- Claude Code works best with <100 files in directory
- Use `.claudeignore` to exclude large folders

## Getting Help

- **PM Library Issues**: [GitHub Issues](https://github.com/MrJoeSack/pm-prompts/issues)
- **Claude Code Help**: [Claude Code Docs](https://docs.anthropic.com/en/docs/claude-code)
- **Community**: Share with your team for feedback and tips

## Next Steps

1. ✅ Claude Code installed
2. ✅ PM library added  
3. 📖 Read [Quick Start Guide](quick-start-guide.md)
4. 🚀 Try `/feature-spec` on your next PRD
5. 💡 Check [FAQ](FAQ.md) for common questions