# PROJECT-GUIDE.md - FOR CLAUDE ONLY

> **👋 Hey! You can ignore this file.** This is instructions for Claude on how to run the course. Nothing here is for you - go run `/lesson0` to start learning!

---

This is the Claude Code training course for accesso Product Managers. This file documents how the course works so we can maintain consistency when building new lessons.

## Project Structure

**This training folder lives INSIDE the user's vault.** The user runs Claude from inside this folder, but their work files are created in the parent (vault root)

```
user-vault/                          ← VAULT ROOT (parent directory)
├── CLAUDE.md                        ← User's CLAUDE.md (created by Lesson 1 at ../)
├── passport/                        ← User's work folders (created by Lesson 2 at ../)
├── interviews/
├── research/
│
└── accesso-ai-training/             ← THIS TRAINING FOLDER (user runs claude here)
    ├── CLAUDE.md                    # This file - project guide (for development)
    ├── .claude/commands/            # Lesson commands
    │   ├── lesson0.md ... lesson6.md
    │   ├── course-map.md
    │   └── training-helpful-tips.md
    ├── reference/                   # Training reference docs (stay here)
    │   ├── quick-reference.md
    │   ├── useful-commands.md
    │   └── Accesso LLC Organization Chart.md
    └── lessons/                     # Learner progress (stays here)
        └── progress.md
```

### File Location Rules

| What | Where | Path from training folder |
|------|-------|---------------------------|
| User's CLAUDE.md | Vault root | `../CLAUDE.md` |
| User's work folders | Vault root | `../passport/`, `../interviews/`, etc. |
| Lesson progress | Training folder | `lessons/progress.md` |
| Reference docs | Training folder | `reference/` |

**Why this structure:** Users work in their vault root day-to-day. The training folder is just for learning. Their CLAUDE.md and work folders need to be at vault root so Claude sees them when they work outside the training context.

## How Lessons Work

### Lesson Format

Each lesson is a **command file** in `.claude/commands/` that acts as a script for Claude to deliver an interactive wizard.

**Standard structure:**
1. Header with lesson title and instructor role
2. `## Delivery Style` - Guidelines for tone and pacing
3. `## BEFORE YOU START` - Read context from previous lessons
4. `## SECTION N: Title` - Content sections separated by `---`
5. `## Wrap Up & Save Progress` - Update progress files
6. `## Dynamic Adaptation Notes` - How to personalize

**Key patterns:**
- Use `**Ask:**` for questions
- Use `> "quoted text"` for what to say
- Use AskUserQuestion tool for structured choices
- Always "Wait for response" before continuing
- End with `**End the lesson here.**`

### Context Persistence

Learner context is maintained across lessons through two files:

**`CLAUDE.md` (learner's root file)**
- Created in Lesson 1
- Contains: role, products, responsibilities, preferences, workspace structure
- Updated by lessons when relevant (e.g., adding workspace structure)

**`lessons/progress.md`**
- Created in Lesson 0
- Contains: name, completion status, key decisions from each lesson
- Appended to at end of each lesson
- Future lessons read this to avoid re-asking questions

### Lesson Design Principles

1. **No repetition** - Read context from previous lessons, don't re-ask
2. **Dynamic & personal** - Use their actual product names, responsibilities
3. **Start small** - Don't overwhelm; suggest minimal viable structures
4. **Flexible** - Everything can be changed later
5. **Hands-on** - They should DO things, not just read
6. **Plain English** - Avoid technical jargon; PMs don't need syntax

### Mid-Lesson Progress Saving

Lessons support resuming if interrupted. Here's how it works:

**At lesson start (BEFORE YOU START section):**
1. Check if `lessons/progress.md` has an "(In Progress)" entry for this lesson
2. If yes, read the last completed section and offer to resume
3. Use AskUserQuestion: "Resume from [section]?" or "Start fresh?"

**During the lesson (after major sections):**
1. Update progress.md with checkpoint: `**Last checkpoint:** Section X - [topic]`
2. Do this after every 2-3 sections or after hands-on exercises

**At lesson end:**
1. Remove "(In Progress)" marker
2. Replace with completed "✓" entry

**Progress entry format (in progress):**
```markdown
## Lesson N: Title (In Progress)
**Started:** [date]
**Last checkpoint:** Section X - [topic]
**Answers so far:**
- [key answer 1]
- [key answer 2]
```

**Progress entry format (complete):**
```markdown
## Lesson N: Title ✓
**Completed:** [date]
**Key info:** [answers]
```

## Lesson Status

| Lesson | Title                                          | Status     |
| ------ | ---------------------------------------------- | ---------- |
| 0      | Course Introduction                            | ✓ Complete |
| 1      | Setting Up Your CLAUDE.md & Context Mgmt       | ✓ Complete |
| 2      | Workspace Setup & Working with Files           | ✓ Complete |
| 3      | Commands & Power User Features                 | ✓ Complete |
| 4      | Subagents for Parallel Research & Perspectives | ✓ Complete |
| 5      | Atlassian MCP Setup & Usage                    | ✓ Complete |
| 6      | Practical Workflows                            | ✓ Complete |

**Note:** Course streamlined to 6 core lessons + future deep-dives as needed.

## Building New Lessons

When creating a new lesson:

1. **Read existing lessons** for style consistency
2. **Start with `BEFORE YOU START`** section to read learner context
3. **Reference their specifics** - products, role, preferences from CLAUDE.md
4. **Keep it concise** - Lessons 0 & 1 are ~160-240 lines
5. **End with progress update** - Append to lessons/progress.md
6. **Update CLAUDE.md if needed** - When adding structural info

## Reference Materials Needed

These documents are referenced but not yet created:
- Company OKRs
- accesso PLC Company Profile
- Key Competitor Information
- Key Client Profiles
- accesso Product List (Line of business + applications)

## Notes

- Course is designed for ~9.5 hours total across all lessons
- Quick Start path: Lessons 0, 1, 3, 6, 8 (renumbered) for 80% value in ~2 hours
- Lessons are self-paced, typically 1-2 per week
