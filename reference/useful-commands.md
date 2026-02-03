# Useful Commands & Resources

Quick reference for commands, shortcuts, and resources you can use anytime.

---

## Built-in Slash Commands

| Command | What it does | When to use it |
|---------|--------------|----------------|
| `/help` | Shows all available commands | When you forget what's available |
| `/clear` | Clears the conversation | Starting fresh on a new topic |
| `/compact` | Compresses conversation history | When context gets too long |
| `/rewind` | Go back to a previous point | Claude went wrong direction, want to retry |
| `/context` | Shows how much context you've used | Checking if you're running low |
| `/cost` | Shows token usage and cost | Curious about usage |
| `/model` | Switch between Claude models | Need faster (Haiku) or smarter (Opus) |
| `/memory` | Shows your CLAUDE.md and memory files | Checking what Claude remembers |
| `/status` | Shows current session info | General health check |

---

## Keyboard Shortcuts

| Shortcut | What it does |
|----------|--------------|
| `Escape` | Cancel current action / interrupt Claude |
| `Ctrl+C` | Stop Claude mid-response |
| `Up Arrow` | Recall previous message |
| `Tab` | Accept autocomplete suggestion |

---

## Course Commands

| Command | Description |
|---------|-------------|
| `/lesson0` | Course Introduction |
| `/lesson1` | Setting Up Your CLAUDE.md |
| `/lesson2` | Workspace Setup & Working with Files |
| `/lesson3` | Commands & Power User Features |
| `/lesson4` | Subagents for Parallel Research & Perspectives |
| `/lesson5` | Atlassian MCP Setup & Usage |
| `/lesson6` | Practical Workflows |
| `/course-map` | See all lessons and what each covers |
| `/training-helpful-tips` | Troubleshooting, file conversions, getting unstuck |

---

## When to Use What

| Situation | What to Do |
|-----------|------------|
| Switching to a different task | `/clear` |
| Running low on context but want to keep working | `/compact` |
| Claude went the wrong direction, want to retry | `/rewind` |
| Check if you have room for a big task | `/context` |
| Need the best quality output | `/model` → Opus |
| Need a quick answer | `/model` → Haiku |
| Want to work on two things at once | Open a new terminal window |

---

## Key Differences

- **`/clear`** = Start completely over (keeps CLAUDE.md)
- **`/compact`** = Keep going with more room (summarizes conversation)
- **`/rewind`** = Go back to a specific point and try again

---

## Custom Commands

- Custom commands live in `.claude/commands/` as markdown files
- Run them with `/command-name`
- Ask Claude to create one: "Create a command that does [X]"
- Browse & share commands at **accesso.io** (new and growing!)

---

## Model Comparison

| Model | Speed | Best For |
|-------|-------|----------|
| **Haiku** | Fastest | Quick questions, simple formatting, brainstorming |
| **Sonnet** | Balanced | Most daily work, good default |
| **Opus** | Most capable | Complex analysis, nuanced writing, tough problems |

---

## Subagent Trigger Phrases

These phrases tell Claude to work in parallel:

- "Compare these..."
- "Analyze all of these..."
- "Research [multiple items]..."
- "Look at each of these and..."

---

## Perspective Prompts

| Situation | Prompt |
|-----------|--------|
| Quick check | "What would engineering likely say about this?" |
| Full analysis | "Give me technical, user, and business perspectives on this idea" |
| Identify questions | "Analyze from multiple angles and tell me what I should validate" |
| Pre-meeting | "What concerns will [stakeholder] likely have about this?" |
| PRD review | "Review this PRD from a technical perspective" |
| Stress test | "Play devil's advocate - why might this fail?" |

---

## Jira Commands (natural language)

| What You Want | How to Ask |
|---------------|------------|
| Create a story | "Create a story for [description]" |
| Create a bug | "Log a bug for [issue]" |
| Search issues | "Show me open bugs in [project]" |
| Get issue details | "What's the status of [ISSUE-KEY]?" |
| Update an issue | "Update [ISSUE-KEY] to add [details]" |

---

## Confluence Commands

| What You Want | How to Ask |
|---------------|------------|
| Create a page | "Create a Confluence page titled [title]" |
| Find pages | "Find pages about [topic]" |
| Read a page | "What does the [page name] page say?" |

---

## Useful External Resources

- **Subagent Library:** https://github.com/VoltAgent/awesome-claude-code-subagents
- **accesso Command Marketplace:** accesso.io (new and growing!)
- **Claude Code Documentation:** https://docs.anthropic.com/claude-code

---

## Tips

1. **Talk naturally** - No special prompts needed, just describe what you want
2. **Be specific** - Instead of "summarize this," try "give me the top 3 takeaways"
3. **Chain requests** - "Find all my meeting notes from this week and pull out the action items"
4. **Reference folders** - "Look at everything in my interviews folder"
5. **Ask Claude to build commands** - "Create a command that does X" - Claude handles the file management
