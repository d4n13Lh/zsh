# Project: Zsh Configuration

## Overview
This directory (`/home/daniel/Projects/zsh-config`) houses the user's custom Zsh shell configuration, built on top of **Oh My Zsh**.
The primary goal is to version control and modularize the shell environment.

## Current Status
- **Foundation:** Oh My Zsh is installed (`~/.oh-my-zsh`).
- **Theme:** Powerlevel10k is installed and configured (`.p10k.zsh`).
- **Plugins:** `git`, `z`, `zsh-autosuggestions`, `zsh-syntax-highlighting` are active.
- **Configuration:** The active `.zshrc` and `.p10k.zsh` are version controlled here.

## Recommended Structure
To keep the configuration modular and maintainable, the following structure is recommended for future development:

```text
zsh-config/
├── .zshrc          # Main entry point (sources other files)
├── .p10k.zsh       # Powerlevel10k theme configuration
├── aliases.zsh     # Custom command aliases
├── exports.zsh     # Environment variables
├── functions/      # Directory for custom function definitions
├── plugins/        # Manual plugins or plugin manager configuration
└── themes/         # Custom themes or prompts
```

## Getting Started
1.  **Link:** Symlink the files to the home directory:
    ```bash
    ln -sf /home/daniel/Projects/zsh-config/.zshrc ~/.zshrc
    ln -sf /home/daniel/Projects/zsh-config/.p10k.zsh ~/.p10k.zsh
    ```
2.  **Customize:** Edit `.zshrc` or `.p10k.zsh` in this directory.
3.  **Modularize:** Extract aliases and functions into separate files and source them from `.zshrc`.

## Conventions
- **Shell:** Zsh (Z Shell).
- **Framework:** Oh My Zsh.
- **Paths:** Use absolute paths or `$HOME` relative paths where necessary.
- **Comments:** Comment complex aliases or functions to explain their utility.
