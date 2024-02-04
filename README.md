## Requirements

- `tmux`
- `xsel`

**Ubuntu**

```bash
sudo apt install -y tmux xsel
```

## Setup

Download repository

```bash
git clone git@github.com:JosefUtbult/tmux-config.git --recurse-submodules
cd tmux-config
```

Symlink the config files to your home directory

```bash
ln -s `pwd`/tmux.conf $HOME/.tmux.conf
ln -s `pwd`/tmux $HOME/.tmux
```

Set tmux to your default shell.

In tmux, install plugins by pressing `C-a I`
