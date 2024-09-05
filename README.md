# dotfiles of pika

My personal dotfiles.
These files are only tested on Archlinux with the lastest software.

I have migrated to [chezmoi](https://www.chezmoi.io/).  If you use Archlinux,
then you can install it with `pacman -S chezmoi`.

## How to use
### the first time
```
$ chezmoi init https://github.com/leomao/dotfiles.git
```
### update
```
$ chezmoi update
```

## Zsh

I use [zplug](https://github.com/b4b4r07/zplug) to manage plugins.

### plugins:

- [vim.zsh](https://github.com/leomao/vim.zsh)
- [zsh-completions](https://github.com/zsh-users/zsh-completions)
- [zsh-syntax-highlighting](https://github.com/zsh-users/zsh-syntax-highlighting)

### Related tools

- [fzf](https://github.com/junegunn/fzf)
- [rg](https://github.com/BurntSushi/ripgrep)
- [exa](https://github.com/ogham/exa)
- [delta](https://github.com/dandavison/delta)

### Customization

Put your customization in `~/.zshenv.local` and `~/.zshrc.local`.

## Tmux

I use [tpm](https://github.com/tmux-plugins/tpm) to manage plugins:
- [tmux-copycat](https://github.com/tmux-plugins/tmux-copycat)
- [tmux-yank](https://github.com/tmux-plugins/tmux-yank)
- [tmux-resurrect](https://github.com/tmux-plugins/tmux-resurrect)

## Git

- You will need to install [delta](https://github.com/dandavison/delta).
* One can add custom settings in `~/.gitconfig.local`.

## Fontconfig

This fontconfig is for Traditional Chinese users on Archlinux primarily.
It's not tested on other distros. But it should work on other distros as well
so long as you have the following:

- one of "Noto Sans CJK TC", "Source Han Sans TW", "Source Han Sans TC"
- "Source Code Pro" or "Inconsolata"

For Archlinux users, you can just install required fonts by
```console
# pacman -S noto-fonts-cjk adobe-source-code-pro-fonts
```
