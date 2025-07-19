# dotfiles

## Chezmoi

```bash
# Make sure the local bin folder is part of PATH
export PATH=${PATH}:${HOME}/.local/bin

# Install chezmoi
sh -c "$(curl -fsLS get.chezmoi.io/lb)" -- init --apply xjmpereira
```

## Neovim

```bash
curl -s -L https://github.com/neovim/neovim/releases/download/v0.11.3/nvim-linux-x86_64.tar.gz | tar zxvf - --strip-components=1 -C ~/.local
```

## Ripgrep

```bash
curl -s -L https://github.com/BurntSushi/ripgrep/releases/download/14.1.1/ripgrep-14.1.1-x86_64-unknown-linux-musl.tar.gz | tar -zxvf - --strip-components=1 -C ~/.local/bin --wildcards "*/rg"
```

## Starship

```bash
curl -s -L https://github.com/starship/starship/releases/download/v1.23.0/starship-x86_64-unknown-linux-gnu.tar.gz | tar zxvf - -C ~/.local/bin 
```

## Nerd Fonts

```bash
mkdir -p ${HOME}/.local/share/fonts
curl -s -L https://github.com/ryanoasis/nerd-fonts/releases/download/v3.4.0/Meslo.tar.xz | tar -xf - -JC ~/.local/share/fonts
```
