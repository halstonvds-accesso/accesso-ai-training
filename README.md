# accesso AI Training

Claude Code training course for accesso Product Managers.

## Prerequisites

1. **Obsidian installed** - See `training/reference/Getting Started - Install Claude Code & Obisidian.md`
2. **Claude Code** - You can use either:
   - **Claude Desktop (Great for beginners)**  with the **Code** tab selected (top-center of the app. Download here - https://code.claude.com/docs/en/desktop), OR
   - **Claude Code CLI** in your terminal - See `training/reference/Getting Started - Install Claude Code & Obisidian.md`

## Getting Started

1. **Download the course ZIP:**
   - Go to https://github.com/halstonvds-accesso/accesso-ai-training
   - Click **Code** → **Download ZIP**
   - Save it somewhere easy to find (like Downloads)

### Option A: Using Claude Desktop (Code tab)

2. **Open Claude Desktop** and click the **Code** tab in the top-left corner.

3. **Open your Obsidian vault folder** by clicking the folder icon or dragging your vault folder into the window.

4. **Drag the ZIP file into the chat**, then type:
   ```
   Extract .claude/commands/ and training/ from this ZIP into my vault.
   ```

5. **Start a new session** (required for new commands to load):
   - Click **+** to start a new Code session (commands only load at session start)

6. **Start the course:**
   ```
   /lesson0
   ```

### Option B: Using Terminal (Claude Code CLI)

2. **Open terminal and navigate to your Obsidian vault:**
   ```bash
   cd path/to/your-vault
   ```
   Alternatively, you can drag and drop your vault folder after typing `cd`

3. **Start Claude Code:**
   ```bash
   claude
   ```

4. **Drag the ZIP file into the terminal**, then type:
   ```
   Extract .claude/commands/ and training/ from this ZIP into my vault.
   ```

5. **Restart Claude** (required for new commands to load):
   - Type `/exit` to quit Claude
   - Start Claude again: `claude`

   > **Why restart?** Claude only loads commands from `.claude/commands/` when it starts. Anytime you add new commands, you'll need to restart Claude and `cd` back into your vault (if you're not already in your vault). It's a bit annoying, but that's just how it works for now.

6. **Start the course:**
   ```
   /lesson0
   ```

That's it! Your vault is now set up. Your CLAUDE.md, work folders, and everything else will be created as you go through the lessons.

---

## Course Structure

| Lesson | Topic |
|--------|-------|
| 0 | Course Introduction |
| 1 | Setting Up Your CLAUDE.md & Context Management |
| 2 | Workspace Setup & Working with Files |
| 3 | Commands & Power User Features |
| 4 | Subagents for Parallel Research & Perspectives |
| 5 | Atlassian MCP Setup & Usage |
| 6 | Practical Workflows |

## Helpful Commands

- `/course-map` - See all available lessons
- `/training-helpful-tips` - FAQ and troubleshooting

## Folder Structure

After setup, your vault will look like this:

```
my-pm-vault/                   ← You run Claude here
├── .claude/commands/          ← Lesson commands
├── CLAUDE.md                  ← Your profile (created in Lesson 1)
├── passport/                  ← Your work folders (created in Lesson 2)
├── interviews/
├── research/
└── training/                  ← Training materials & progress
    ├── lessons/progress.md
    ├── reference/
    └── PROJECT-GUIDE.md       ← For Claude only, you can ignore
```

## Notes

- **PROJECT-GUIDE.md** is instructions for Claude on how to run the course. You can ignore it.
- **training/** contains course materials and tracks your progress
- Your actual work (PRDs, notes, etc.) lives in folders at the vault root

## Questions?

Reach out to Halston van der Sluys if you get stuck.
