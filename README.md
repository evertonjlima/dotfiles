# Dotfiles

This repository contains configuration files (dotfiles) for my development environment, including settings for tools like Vim, Zsh, Git, and more. Using this setup allows for a personalized and portable development environment.


### Features

- **Vim Configuration** (`.vimrc`): Includes syntax highlighting, relative line numbers, and basic plugin support via Vim-Plug.
- **Zsh Configuration** (`.zshrc`): Contains custom aliases, paths, and plugins, with modular files for easy management.
- **Git Configuration** (`.gitconfig`): Provides shortcuts and customizations for Git.
- **Setup Script** (`setup.sh`): Automates the setup process by creating symlinks and installing necessary tools like Vim-Plug.

## Requirements

Before running the setup script, make sure the following tools are installed on your system:

1. **Homebrew** (optional but recommended for macOS users to manage packages easily)
   - Install Homebrew by running:
     ```bash
     /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
     ```

2. **Vim**
   - Install Vim via Homebrew (or ensure it’s installed on your system):
     ```bash
     brew install vim
     ```

3. **Zsh**
   - Zsh should be available by default on macOS and most Linux distributions. To check if Zsh is installed, run:
     ```bash
     zsh --version
     ```

4. **Git**
   - Git is required to clone this repository and manage your Git configurations. Install Git if it’s not available:
     ```bash
     brew install git
     ```

5. **Curl**
   - Curl is used to download Vim-Plug. It should be pre-installed on most systems. To check, run:
     ```bash
     curl --version
     ```

## Installation

### 1. Clone the Repository

Clone this repository to your home directory or a directory of your choice:

```bash
git clone https://github.com/evertonjlima/dotfiles ~/repository
```

2. Run the Setup Script
The setup.sh script will:

* Create symlinks in your home directory for each tool’s configuration.
* Install Vim-Plug (for managing Vim plugins).
* Update .zshrc with paths to source additional Zsh files.

To run the setup script:

```bash
cd ~/repository/dotfiles
bash setup.sh
```

3. Verify the Setup
After running the setup script:

Open a new terminal to load your new .zshrc configurations.
Launch Vim and run :PlugInstall to install plugins if you added any to the .vimrc.


