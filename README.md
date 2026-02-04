# accesso AI Training

Claude Code training course for accesso Product Managers.

## Prerequisites

1. **Obsidian installed** - See `training/reference/Getting Started - Install Claude Code & Obisidian.md`
2. **Claude Code installed** - See `training/reference/Getting Started - Install Claude Code & Obisidian.md`
3. **Terminal access** - You'll run Claude Code from your terminal

## Getting Started

1. **Download the course ZIP:**
   - Go to https://github.com/halstonvds-accesso/accesso-ai-training
   - Click **Code** → **Download ZIP**
   - Save it somewhere easy to find (like Downloads)

2. **Open terminal and navigate to your Obsidian vault:**
   ```bash
   cd path/to/your-vault
   ```
   Alternatively, you can drag and drop your vaults folder after typing cd

3. **Start Claude Code:**
   ```bash
   claude
   ```

4. **Drag the ZIP file into the terminal**, then type:
   ```
   Extract .claude/commands/ and training/ from this ZIP into my vault.
   ```

5. **Start the course:**
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
