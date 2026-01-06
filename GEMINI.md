# Project: Zsh Configuration

## Overview
This directory (`/home/daniel/Projects/zsh-config`) houses the user's custom Zsh shell configuration, built on top of **Oh My Zsh**.
The primary goal is to version control and modularize the shell environment.

## Current Status
- **Foundation:** Oh My Zsh is installed (`~/.oh-my-zsh`).
- **Configuration:** The active `.zshrc` has been imported from `~/.zshrc` into this directory.

## Recommended Structure
To keep the configuration modular and maintainable, the following structure is recommended for future development:

```text
zsh-config/
├── .zshrc          # Main entry point (sources other files)
├── aliases.zsh     # Custom command aliases
├── exports.zsh     # Environment variables
├── functions/      # Directory for custom function definitions
├── plugins/        # Manual plugins or plugin manager configuration
└── themes/         # Custom themes or prompts
```

## Getting Started
1.  **Link:** Symlink the file to the home directory to make this project the source of truth:
    ```bash
    ln -sf /home/daniel/Projects/zsh-config/.zshrc ~/.zshrc
    ```
2.  **Customize:** Edit `.zshrc` in this directory.
3.  **Modularize:** Extract aliases and functions into separate files and source them from `.zshrc`.

## Conventions
- **Shell:** Zsh (Z Shell).
- **Framework:** Oh My Zsh.
- **Paths:** Use absolute paths or `$HOME` relative paths where necessary.
- **Comments:** Comment complex aliases or functions to explain their utility.
