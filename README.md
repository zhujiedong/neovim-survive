# Quarto Nvim Kickstarter

Companion to <https://github.com/quarto-dev/quarto-nvim>.

This requires Neovim >= **v0.9.5** (https://github.com/neovim/neovim/releases/tag/stable)

## Videos

Check out this playlist for a full guide and walkthrough:
https://youtube.com/playlist?list=PLabWm-zCaD1axcMGvf7wFxJz8FZmyHSJ7

## Setup

Clone this repo into `~/.config/nvim/` or copy-paste just the parts you like.

If you already have your own configuration, check out `lua/plugins/quarto.lua`
for the configuration of all plugins directly relevant to your Quarto experience.

This configuration can make use of a "Nerd Font" for icons and symbols.
Download one here: <https://www.nerdfonts.com/> and set it as your terminal font.

### Unix, Linux Installation

```bash
git clone https://github.com/jmbuhr/quarto-nvim-kickstarter.git ~/.config/nvim
```

### Windows Powershell Installation

```bash
git clone https://github.com/jmbuhr/quarto-nvim-kickstarter.git "$env:LOCALAPPDATA\nvim"
```

The telescope file finder uses `fzf` for fuzzy finding via the [telescope-fzf-native](https://github.com/nvim-telescope/telescope-fzf-native.nvim) extension.
It will automatically install `fzf`, but needs some requirements which are not pre-installed on Windows.
Check out the previous link for those (or comment out the extension in `./lua/plugins/ui.lua`).

Now you are good to go!

## Updating

Certain updates to plugins may leave behind unused plugin data. If this configuration produces an error on startup, try removing those first, allowing the lazy.nvim package manager to recreate the correct plugin structure:

```bash
rm -r ~/.local/share/nvim
rm -r ~/.local/state/nvim
```

---

以上是安装的插件，多数功能还没搞明白，不过基本生存下来了。
2024-03-29

