# dotfiles


```bash
# Make sure the local bin folder is part of PATH
export PATH=${PATH}:${HOME}/.local/bin

# Install chezmoi
sh -c "$(curl -fsLS get.chezmoi.io/lb)" -- init --apply xjmpereira
```
