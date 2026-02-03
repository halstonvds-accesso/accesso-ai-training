# Getting Started: Install Claude Code

> **Read this first before starting the course**

This guide walks you through installing everything you need to use Claude Code. Pick your operating system and follow the steps.

---

## Table of Contents

**Mac Users:** [Jump to Mac Installation](#mac-installation)

**Windows Users:** [Jump to Windows Installation](#windows-installation)

---

# Mac Installation

## Step 1: Install Obsidian & Create Your Vault

Obsidian is where your workspace (vault) lives. This is where you'll work with Claude.

### Download Obsidian

1. Go to https://obsidian.md/download
2. Click **"Download for macOS"**
3. Open the downloaded `.dmg` file
4. Drag Obsidian to your **Applications** folder
5. Open Obsidian from Applications

### Create Your Vault

1. Launch **Obsidian**
2. Click **"Create new vault"**
3. **Name your vault:** You can use your team, product name, or anything else you feel like. (e.g., `accesso-handheld`, `passport-services`, `commerce`)
4. **Choose location:** Pick somewhere easy to find
   - Examples: `/Users/[YourName]/Documents/[vault-name]`
   - Examples: `/Users/[YourName]/Desktop/[vault-name]`
1. Click **"Create"**

Your empty vault is ready! Claude will populate it during our course.

---

## Step 2: (Optional) Transcription Tools

If you want to use voice input - dictating notes, transcribing meetings, or speaking to Claude - here are your options:

### Built-in Mac Dictation (Free, Already Installed)

macOS has dictation built in. To enable:

1. Open **System Settings** > **Keyboard**
2. Click **Dictation**
3. Turn it **On**
4. Press **Fn Fn** (function key twice) to start dictating anywhere

Great for quick notes and speaking instead of typing.

### Mac Whisper (Free, Mac Only)

High-quality local transcription using OpenAI's Whisper model. Runs entirely on your Mac - no data sent anywhere.

- **Download:** https://goodsnooze.gumroad.com/l/macwhisper
- **Best for:** Transcribing meeting recordings, audio files
- **Note:** Free version available, paid version has more features

### Whisper Flow (Paid)

Real-time transcription that works system-wide.

- **Download:** https://whisperflow.co/
- **Best for:** Live transcription while you speak

**Skip this step if you don't need voice input** - you can always add it later although it is **EXTREMELY** useful for transcriptions during meetings (those can also be taken from Microsoft Teams though.

---

## Step 3: Install Node.js

Claude Code requires Node.js 18 or higher. Open your terminal. Check if you already have it:

```bash
node --version
```

If you see `v18.x.x` or higher, skip to Step 4. Otherwise, install Node:

### Option A: Using Homebrew (Recommended)

```bash
# Install Homebrew if you don't have it
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

# Install Node.js
brew install node

# Verify installation
node --version
```

### Option B: Direct Download

1. Go to https://nodejs.org/
2. Download the **LTS version** for macOS
3. Open the downloaded `.pkg` file
4. Follow installation prompts
5. Open Terminal and verify: `node --version`

---

## Step 4: Install Claude Code

Open Terminal and run:

```bash
curl -fsSL https://claude.ai/install.sh | bash
```

**Verify it works:**

```bash
claude --version
```

---

## Step 5: Download the Course Files

1. Reference the instr
---

## Step 6: Install the Course with Claude

1. Open **Terminal**
2. Navigate to your vault folder:
   ```bash
   cd path/to/vault
   ```
   *(Replace `path to vault` with your vault name)*
3. Start Claude Code:
   ```bash
   claude
   ```
4. **Copy and paste this prompt to install the course:**

```
I just downloaded the accesso AI training course ZIP file to my Downloads folder.
Please unzip it and set up my vault with all the course materials including:
- The lesson commands in .claude/commands/
- The reference documents
- Any other course files

The ZIP file should be at ~/Downloads/accesso-ai-training.zip (or similar name).
```

5. Claude will unzip the files and set up your vault
6. Once complete, type `/lesson0` to begin the course!

---

# Windows Installation

## Step 1: Install Obsidian & Create Your Vault

Obsidian is where your workspace (vault) lives. This is where you'll work with Claude.

### Download Obsidian

1. Go to https://obsidian.md/download
2. Click **"Download for Windows"**
3. Run the installer (`.exe` file)
4. Follow installation prompts
5. Launch Obsidian from Start menu or desktop shortcut

### Create Your Vault

1. Launch **Obsidian**
2. Click **"Create new vault"**
3. **Name your vault:** Use your team or product name (e.g., `accesso-handheld`, `passport-services`, `commerce`)
4. **Choose location:** Pick somewhere easy to find
   - Example: `C:\Users\[YourName]\Documents\[vault-name]`
5. Click **"Create"**

Your empty vault is ready! Claude will populate it during the course.

---

## Step 2: (Optional) Transcription Tools

If you want to use voice input - dictating notes, transcribing meetings, or speaking to Claude - here are your options:

### Built-in Windows Dictation (Free, Already Installed)

Windows has dictation built in. To use:

1. Press **Win + H** to start voice typing
2. Speak, and Windows will transcribe
3. Works in any text field

Great for quick notes and speaking instead of typing.

### Whisper Flow (Paid)

Real-time transcription that works system-wide.

- **Download:** https://whisperflow.co/
- **Best for:** Live transcription while you speak

### Other Transcription Options

Most high-quality local transcription tools (Mac Whisper, Whisper Flow) are Mac-only. For Windows:

- **Microsoft Teams transcription** - If you use Teams for meetings, enable transcription in meeting settings
- **Otter.ai** - Cloud-based transcription service (https://otter.ai)
- **OpenAI Whisper** - Can be installed manually if you're technical (https://github.com/openai/whisper)

**Skip this step if you don't need voice input** - you can always add it later.

---

## Step 3: Install Node.js

Claude Code requires Node.js 18 or higher. Check if you already have it:

```powershell
node --version
```

If you see `v18.x.x` or higher, skip to Step 4. Otherwise, install Node:

### Option A: Using Winget (Windows 10/11)

Open **PowerShell as Administrator** and run:

```powershell
winget install OpenJS.NodeJS.LTS

# Verify installation
node --version
```

### Option B: Direct Download

1. Go to https://nodejs.org/
2. Download the **LTS version** for Windows
3. Run the installer (`.msi` file)
4. Follow installation prompts (keep default settings)
5. **Important:** Make sure "Add to PATH" is checked
6. Open **Command Prompt** and verify: `node --version`

**Note:** You may need to restart your terminal or computer after installation.

---

## Step 4: Install Claude Code

Open **PowerShell** and run:

```powershell
irm https://claude.ai/install.ps1 | iex
```

**Verify it works:**

```powershell
claude --version
```

---

## Step 5: Download the Course Files

1. Download the course ZIP file from: **[COURSE DOWNLOAD LINK]**
   *(Ask Halston or check #ai-enablement-product if you don't have the link)*
2. Save it to your **Downloads** folder
3. Don't unzip it - Claude will do that for you!

---

## Step 6: Install the Course with Claude

1. Open **PowerShell** or **Command Prompt**
2. Navigate to your vault folder:
   ```powershell
   cd C:\Users\[YourName]\Documents\accesso-handheld
   ```
   *(Replace `[YourName]` with your username and `accesso-handheld` with your vault name)*
3. Start Claude Code:
   ```powershell
   claude
   ```
4. **Copy and paste this prompt to install the course:**

```
I just downloaded the accesso AI training course ZIP file to my Downloads folder.
Please unzip it and set up my vault with all the course materials including:
- The lesson commands in .claude/commands/
- The reference documents
- Any other course files

The ZIP file should be at C:\Users\[YourName]\Downloads\accesso-ai-training.zip (or similar name).
```

5. Claude will unzip the files and set up your vault
6. Once complete, type `/lesson0` to begin the course!

---

# Troubleshooting

## "node: command not found"

- **Mac:** Make sure Homebrew installed correctly, then run `brew install node` again
- **Windows:** Restart your terminal/computer after installing Node.js

## "claude: command not found"

- Try closing and reopening your terminal
- Re-run the install command from Step 4

## Obsidian won't open the vault

- Make sure you're opening the folder that contains your vault, not a subfolder
- Try creating a new vault if the first one has issues

## Can't find my vault folder in Terminal

- **Mac:** Your Documents folder is at `~/Documents/`
- **Windows:** Your Documents folder is at `C:\Users\[YourName]\Documents\`
- Use `ls` (Mac) or `dir` (Windows) to see what's in the current folder

## Need help?

- **Office Hours:** Tuesdays & Thursdays 2-3pm with Halston
- **Slack:** #ai-enablement-product
- **1:1:** Schedule with Halston or Brian

---

# Summary

Here's what you've done:

1. ✅ Installed Obsidian and created your vault
2. ✅ (Optional) Set up transcription tools
3. ✅ Installed Node.js
4. ✅ Installed Claude Code
5. ✅ Downloaded the course files
6. ✅ Had Claude install the course in your vault

**You're ready!** Type `/lesson0` in Claude to begin the course.

Welcome to Claude Code!
