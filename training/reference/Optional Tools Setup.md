# Optional Tools Setup

These tools extend what you can do with Claude Code. They're not required, but useful when you need them.

---

## Pandoc - File Format Converter

Pandoc converts documents between formats. Useful when you need to share markdown files as Word docs, or convert received documents into markdown for easier processing.

### What It Does

| Conversion | Direction | Example |
|------------|-----------|---------|
| MD ↔ DOCX | Both ways | Convert PRD to Word for stakeholders |
| MD ↔ PPTX | Both ways | Turn markdown notes into slides |
| MD ↔ HTML | Both ways | Create web-ready docs from markdown |
| CSV/XLSX → MD | One way | Turn spreadsheets into markdown tables |

### Setup

Ask Claude:

> "Please set up Pandoc so I can convert files between formats - ref https://pandoc.org/"

Claude will install it via Homebrew (Mac) or the appropriate package manager.

### Add to Your CLAUDE.md

After setup, add this to your CLAUDE.md so Claude remembers how to use it:

```markdown
## Tools

**Format conversion:** Use Pandoc for file format conversions. Bidirectional: MD↔DOCX, MD↔PPTX, MD↔HTML. One-way: CSV/TSV/XLSX→MD (spreadsheets to tables). Usage: `pandoc input -o output` (format from extension). Use `-t gfm` for GitHub-flavoured markdown output.
```

### Usage Examples

Once installed, just ask naturally:

- "Convert my PRD to a Word doc"
- "Turn this spreadsheet into a markdown table"
- "Make a PowerPoint from my notes.md"
- "Convert this HTML page to markdown"

The command Claude will use: `pandoc input.md -o output.docx`

For GitHub-flavoured markdown output: `pandoc input.docx -t gfm -o output.md`

---

## More Tools

*(Additional optional tools will be documented here as they're identified)*
