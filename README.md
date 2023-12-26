## Requirements

- `tmux`
- `xsel`

**Ubuntu**

```bash
sudo apt install tmux xsel
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

Add tmux as startup on new shell. Add the following to your `.bashrc` or `.zshrc`

```
# Run tmux on startup
if command -v tmux &> /dev/null && [ -n "$PS1" ] && [[ ! "$TERM" =~ screen ]] && [[ ! "$TERM" =~ tmux ]] && [ -z "$TMUX" ]; then
  exec tmux
fi
```

Start a new session, or just run `tmux`

In tmux, install plugins by pressing `C-a I`
