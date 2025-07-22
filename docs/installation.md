# Installation & Setup Guide

*Complete setup instructions for Claude Code and the PM library*

## Prerequisites: Installing Claude Code

### Step 1: Get Claude Code (5 minutes)

**For IT/Engineering to install:**

1. **Download Claude Code** from [claude.ai/code](https://claude.ai/code)
   - Available for Mac, Windows, and Linux
   - Requires a Claude Pro or Team subscription

2. **Install the application**
   - Mac: Drag to Applications folder
   - Windows: Run the installer
   - Linux: Follow package manager instructions

3. **Sign in with your Anthropic account**
   - Use your work email if you have a team subscription
   - Or personal Claude Pro account

4. **Verify installation**
   ```bash
   # Open terminal and type:
   claude --version
   ```

### Step 2: Understanding Claude Code

**What PMs need to know:**
- Claude Code opens in a terminal but works like chat
- You type in plain English, not code
- It can read and edit files on your computer
- Everything stays local on your machine

**Quick test:**
1. Open Claude Code (type `claude` in terminal)
2. Ask it something like "What files are in this folder?"
3. It should list your files - that's it!

## Installing the PM Library

Once Claude Code is installed, add the PM frameworks:

### Option 1: Project-Specific (Recommended)
```bash
# In your product management project folder
git clone https://github.com/MrJoeSack/pm-prompts.git .pm-library
cp .pm-library/CLAUDE.md ./CLAUDE.md  
cp -r .pm-library/.claude ./

# That's it! The PM commands are now available
```

### Option 2: Global Access (For Multiple Projects)
```bash  
# Install once, use everywhere
cd ~
git clone https://github.com/MrJoeSack/pm-prompts.git
ln -s ~/pm-prompts/CLAUDE.md ~/.claude/CLAUDE.md
ln -s ~/pm-prompts/.claude/commands ~/.claude/commands
```

### Option 3: Quick Install (No Git Required)
```bash
# Download just the essentials
curl -o CLAUDE.md https://raw.githubusercontent.com/MrJoeSack/pm-prompts/main/CLAUDE.md
mkdir -p .claude/commands
cd .claude/commands
curl -O https://raw.githubusercontent.com/MrJoeSack/pm-prompts/main/.claude/commands/feature-spec.md
curl -O https://raw.githubusercontent.com/MrJoeSack/pm-prompts/main/.claude/commands/stakeholder-sync.md
# Add more commands as needed
```

## Verification

Test that everything works:

1. **Open Claude Code**
   ```bash
   claude
   ```

2. **Try PM commands**
   - Type: `/pm-help` (should list all commands)
   - Type: `/feature-spec` (should ask for feature details)
   - Type: "Help me write a PRD" (should offer to use frameworks)

3. **Check context loading**
   - Ask: "What PM frameworks do you have?"
   - Should list economical writing, good strategy, etc.

## For PMs: Your First Session

1. **Open terminal** (Terminal on Mac, Command Prompt on Windows)
2. **Navigate to your project** 
   ```bash
   cd /path/to/your/product/folder
   ```
3. **Start Claude Code**
   ```bash
   claude
   ```
4. **Try your first command**
   ```
   You: /feature-spec
   You: I need to spec out a user authentication feature
   Claude: [Provides structured PRD template]
   ```

## For IT Administrators

### Deployment Options

**Individual Installation**
- Install Claude Code on each PM's machine
- Clone library to shared location
- Create symlinks for each user

**Team Deployment**
```bash
# Create shared library location
sudo mkdir -p /opt/pm-claude-library
sudo git clone https://github.com/MrJoeSack/pm-prompts.git /opt/pm-claude-library

# For each user
ln -s /opt/pm-claude-library/CLAUDE.md ~/.claude/CLAUDE.md
ln -s /opt/pm-claude-library/.claude/commands ~/.claude/commands
```

### Security Considerations
- Claude Code processes files locally
- You control what data is shared
- Set file permissions appropriately
- Can restrict which folders Claude Code can access
- All actions are logged in terminal history

## Customization

### Add Company-Specific Commands
Create `.claude/commands/your-command.md`:
```markdown
---
name: company-prfaq
description: Generate PRFAQ in our company format
---

Generate a PRFAQ following our company template with sections for:
- Problem Statement
- Customer Benefits  
- Internal Benefits
- FAQ (5-7 questions)

Use our tone: professional but approachable.
```

### Extend PM Context
Add to `CLAUDE.md`:
```markdown
## Company PM Standards
- All PRDs must include success metrics
- Use DACI model for decision docs
- Feature flags required for all launches
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
- Ensure CLAUDE.md is in current directory
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
3. 📖 Read the [Quick Start Guide](quick-start-guide.md)
4. 🚀 Try `/feature-spec` on your next PRD
5. 💡 Check the [FAQ](FAQ.md) for common questions