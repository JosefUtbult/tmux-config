## Setup

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
