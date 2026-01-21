# accesso AI Training - Project Guide

This is the Claude Code training course for accesso Product Managers. This file documents how the course works so we can maintain consistency when building new lessons.

## Project Structure

```
/
├── CLAUDE.md                    # This file - project guide
├── Course Curriculum.md         # Full course outline and lesson descriptions
├── Quick Start Guide.md         # Fast-track path for learners
├── .claude/
│   └── commands/
│       ├── lesson0.md           # Course Introduction
│       ├── lesson1.md           # Setting Up Your CLAUDE.md
│       ├── lesson2.md           # Workspace Setup & Working with Files
│       ├── lesson3.md           # Commands & Power User Features
│       ├── lesson4.md           # Subagents for Parallel Research & Perspectives
│       ├── lesson5.md           # Atlassian MCP Setup & Usage
│       ├── lesson6.md           # Practical Workflows
│       ├── lesson[N].md         # Future deep-dive lessons
│       ├── course-map.md        # Table of contents for all lessons
│       └── training-helpful-tips.md  # FAQ & troubleshooting guide
├── reference/
│   ├── Accesso LLC Organization Chart.md
│   └── Optional Tools Setup.md      # Pandoc, etc.
├── examples/                    # Example artifacts (to be built)
├── lessons/                     # Created per-learner for progress tracking
└── templates/                   # Reusable templates (to be built)
```

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
