# Quick Reference Guide

A one-page summary of everything you learned in the Claude Code course.

---

## The Basics

**Talk naturally.** No special prompts needed. Just describe what you want like you're talking to a smart coworker.

**Claude reads your CLAUDE.md automatically.** The more context you put there, the more personalized Claude's help becomes.

**Just ask.** If you want something created, updated, or organized - just tell Claude in plain English.

---

## Essential Commands

| Command | Purpose |
|---------|---------|
| `/help` | See all available commands |
| `/clear` | Fresh start (keeps CLAUDE.md) |
| `/compact` | Save context space (keeps working) |
| `/context` | Check your usage budget |
| `/model` | Switch models (Haiku/Sonnet/Opus) |

**Pro tip:** Type `/` to browse all commands anytime.

---

## Working with Files

| What You Want | How to Ask |
|---------------|------------|
| Find files | "Find my PRDs from last month" |
| Read content | "What's the main point of this doc?" |
| Extract info | "Pull out the action items from this" |
| Synthesize | "What themes do you see across these files?" |
| Process images | "Extract the text from this screenshot" |
| Web research | "Look up [competitor]" |

---

## Subagents (Parallel Work)

**Run multiple things at once:**
- "Research competitors A, B, and C and compare their pricing"
- "Analyze these 5 interviews and find common themes"

**Get multiple perspectives:**
- "Give me technical, user, and business perspectives on this idea"
- "What would engineering likely say about this?"
- "Play devil's advocate - why might this fail?"

**Remember:** Perspectives help you PREPARE. They don't replace talking to real people.

---

## Jira & Confluence

Claude always asks before creating or updating anything.

| What You Want | How to Ask |
|---------------|------------|
| Create story | "Create a story for [description]" |
| Search issues | "Show me open bugs in [project]" |
| Issue details | "What's the status of [ISSUE-KEY]?" |
| Create page | "Create a Confluence page titled [title]" |

---

## Common Workflows

### Meeting Notes
"Here are my meeting notes. Extract the action items and key decisions."

### User Stories
"Write a user story for [feature idea]" - then "Create this in Jira" when ready.

### PRD Drafting
"Create a PRD outline for [feature]" or "Turn these notes into a PRD"

### Competitive Research
"Compare [A], [B], and [C] on pricing" - runs parallel research

### Interview Prep
"Generate interview questions about [problem/hypothesis]"

### Feedback Synthesis
"Here's customer feedback - what are the main themes?"

---

## Context Management

| File | Purpose |
|------|---------|
| `CLAUDE.md` | Your profile, preferences, reference docs |
| `lessons/progress.md` | Your course journey and decisions |

- Keep CLAUDE.md concise (~300 lines)
- Link to other files for detailed instructions
- Just ask Claude to update these files

---

## Models

| Model | Use For |
|-------|---------|
| **Haiku** | Quick questions, simple formatting |
| **Sonnet** | Most daily work (default) |
| **Opus** | Complex analysis, nuanced writing |

---

## Key Principles

1. **This workspace is your source of truth** - Jira/Confluence is where things go when ready
2. **Perspectives prepare, validation confirms** - Always talk to real people
3. **Start small, expand as needed** - You can always add more structure later
4. **Just ask** - Claude handles file management, commands, organization

---

## Resources

- **Subagent Library:** https://github.com/VoltAgent/awesome-claude-code-subagents
- **Command Marketplace:** accesso.io
- **Course Help:** `/training-helpful-tips`
- **All Lessons:** `/course-map`
