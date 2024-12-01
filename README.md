# macOS Programming Environment Setup

---

## Dock Setup

1. Shift the Dock to the left side of the screen.
2. Enable auto-hide for the Dock.
3. Set smaller Dock icons.

---

## Hot Corners Setup

- **Top Left**: Launchpad
- **Bottom Left**: Desktop

---

## Essential Applications

- **Rectangle**: A window management tool to organize your workspace.

---

## Terminal Setup

### Install Iterm2
```bash
brew install --cask iterm2
```

### Install coolnight colour scheme
```bash
curl https://raw.githubusercontent.com/josean-dev/dev-environment-files/main/coolnight.itermcolors --output ~/Downloads/coolnight.itermcolors
```

### Install Homebrew
```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

## For Script setup for ZSH

### Install Zinit
```bash
bash -c "$(curl --fail --show-error --silent --location https://raw.githubusercontent.com/zdharma-continuum/zinit/HEAD/scripts/install.sh)"
```

### Install fzf
```bash
brew install fzf
```

## For manual Installation
### Install Powerlevel10k
```bash
brew install powerlevel10k
echo "source $(brew --prefix)/share/powerlevel10k/powerlevel10k.zsh-theme" >>~/.zshrc
```
[Powerlevel10k Guide](https://github.com/romkatv/powerlevel10k?tab=readme-ov-file#meslo-nerd-font-patched-for-powerlevel10k)

### Install Zsh Plugins

#### zsh-autosuggestions
```bash
brew install zsh-autosuggestions
```
Add the following to `~/.zshrc`:
```bash
source $(brew --prefix)/share/zsh-autosuggestions/zsh-autosuggestions.zsh
```

#### zsh-autocomplete
```bash
brew install zsh-autocomplete
```

#### zsh-syntax-highlighting
```bash
brew install zsh-syntax-highlighting
```

---

## VS Code Setup

### Theme
- One Dark Pro

### Extensions
- Code Runner
- GitLens
- Indent Rainbow
- Prettier
- Copilot
- Java Support:
  - Language Support for Java
  - Debugger for Java
  - Extension Pack for Java

---

## IntelliJ IDEA Setup

### Extensions
- Prettier
- Rainbow Brackets
- Indent Rainbow
- Git Blame ([Git Toolbox](https://plugins.jetbrains.com/plugin/7499-gittoolbox/versions/stable))
- Jump to Line
- Maven Helper
- Translation
- .env Files Support
- Database Navigator

---
