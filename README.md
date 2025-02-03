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

### Install Homebrew
```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

### Install Iterm2
```bash
brew install --cask iterm2
```

### Install coolnight colour scheme
```bash
curl https://raw.githubusercontent.com/josean-dev/dev-environment-files/main/coolnight.itermcolors --output ~/Downloads/coolnight.itermcolors
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

### Install zoxide
```bash
brew install zoxide
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
### Enable natural text editing for iterm2
* Iterm2-Settings-Profile-keys-presets...-natural text editing  
[Link to issue](https://gist.github.com/seachai/948ed1eeafa32ce03db6685edb879f71)

---

## Productivity Apps Setup
- Raycast
- Hiddenbar

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

### Karabiner rule for home row mods (if needed)
```bash
{
    "description": "Home Row Mods - Shift on F/J, Command on D/K, Option on S/L, Control on A/;",
    "manipulators": [
        {
            "from": {
                "key_code": "f",
                "modifiers": { "optional": ["any"] }
            },
            "parameters": {
                "basic.to_delayed_action_delay_milliseconds": 30,
                "basic.to_if_held_down_threshold_milliseconds": 30
            },
            "to": [
                {
                    "key_code": "left_shift",
                    "lazy": true
                }
            ],
            "to_if_alone": [{ "key_code": "f" }],
            "type": "basic"
        },
        {
            "from": {
                "key_code": "j",
                "modifiers": { "optional": ["any"] }
            },
            "parameters": {
                "basic.to_delayed_action_delay_milliseconds": 30,
                "basic.to_if_held_down_threshold_milliseconds": 30
            },
            "to": [
                {
                    "key_code": "right_shift",
                    "lazy": true
                }
            ],
            "to_if_alone": [{ "key_code": "j" }],
            "type": "basic"
        },
        {
            "from": {
                "key_code": "d",
                "modifiers": { "optional": ["any"] }
            },
            "parameters": {
                "basic.to_delayed_action_delay_milliseconds": 30,
                "basic.to_if_held_down_threshold_milliseconds": 30
            },
            "to": [
                {
                    "key_code": "left_command",
                    "lazy": true
                }
            ],
            "to_if_alone": [{ "key_code": "d" }],
            "type": "basic"
        },
        {
            "from": {
                "key_code": "k",
                "modifiers": { "optional": ["any"] }
            },
            "parameters": {
                "basic.to_delayed_action_delay_milliseconds": 30,
                "basic.to_if_held_down_threshold_milliseconds": 30
            },
            "to": [
                {
                    "key_code": "right_command",
                    "lazy": true
                }
            ],
            "to_if_alone": [{ "key_code": "k" }],
            "type": "basic"
        },
        {
            "from": {
                "key_code": "s",
                "modifiers": { "optional": ["any"] }
            },
            "parameters": {
                "basic.to_delayed_action_delay_milliseconds": 30,
                "basic.to_if_held_down_threshold_milliseconds": 30
            },
            "to": [
                {
                    "key_code": "left_option",
                    "lazy": true
                }
            ],
            "to_if_alone": [{ "key_code": "s" }],
            "type": "basic"
        },
        {
            "from": {
                "key_code": "l",
                "modifiers": { "optional": ["any"] }
            },
            "parameters": {
                "basic.to_delayed_action_delay_milliseconds": 30,
                "basic.to_if_held_down_threshold_milliseconds": 30
            },
            "to": [
                {
                    "key_code": "right_option",
                    "lazy": true
                }
            ],
            "to_if_alone": [{ "key_code": "l" }],
            "type": "basic"
        },
        {
            "from": {
                "key_code": "a",
                "modifiers": { "optional": ["any"] }
            },
            "parameters": {
                "basic.to_delayed_action_delay_milliseconds": 30,
                "basic.to_if_held_down_threshold_milliseconds": 30
            },
            "to": [
                {
                    "key_code": "left_control",
                    "lazy": true
                }
            ],
            "to_if_alone": [{ "key_code": "a" }],
            "type": "basic"
        },
        {
            "from": {
                "key_code": "semicolon",
                "modifiers": { "optional": ["any"] }
            },
            "parameters": {
                "basic.to_delayed_action_delay_milliseconds": 30,
                "basic.to_if_held_down_threshold_milliseconds": 30
            },
            "to": [
                {
                    "key_code": "right_control",
                    "lazy": true
                }
            ],
            "to_if_alone": [{ "key_code": "semicolon" }],
            "type": "basic"
        }
    ]
}
```
