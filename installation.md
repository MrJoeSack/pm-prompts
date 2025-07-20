# Installation & Setup Guide

*Setup instructions for the PM Claude Code library*

## Quick Setup

**Option 1: Project-Specific (Recommended)**
```bash
# In your product management project
git clone https://github.com/MrJoeSack/pm-prompts.git .pm-library
cp .pm-library/CLAUDE.md ./CLAUDE.md  
cp -r .pm-library/.claude ./
```

**Option 2: Global Access**
```bash  
# Clone to home directory
cd ~
git clone https://github.com/MrJoeSack/pm-prompts.git
ln -s ~/pm-prompts/CLAUDE.md ~/.claude/CLAUDE.md
ln -s ~/pm-prompts/.claude/commands ~/.claude/commands
```

**Option 3: Direct Integration**
```bash
# Copy just what you need
curl -o CLAUDE.md https://raw.githubusercontent.com/MrJoeSack/pm-prompts/main/CLAUDE.md
mkdir -p .claude/commands
# Copy individual commands as needed
```

## Verification

Test the installation:
```bash
# Claude Code should recognize custom commands
/feature-spec
/strategy-review  
/prd-review

# And automatically load PM context from CLAUDE.md
```

## Customization

**Add your own commands**: Create `.claude/commands/your-command.md`

**Extend CLAUDE.md**: Add team-specific PM patterns:
```markdown
## Team Conventions
- We use OKRs for quarterly planning
- PRDs must include technical complexity estimates  
- All features require usage analytics
```

**Framework modifications**: Fork the repo and adapt frameworks for your industry/product type.

## Troubleshooting

- **Commands not found**: Check `.claude/commands/` directory exists
- **Context not loading**: Verify `CLAUDE.md` in project root
- **Global not working**: Check Claude Code finds `~/.claude/CLAUDE.md`

The library loads automatically after installation when Claude Code starts.