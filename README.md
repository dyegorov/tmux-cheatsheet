# tmux-cheatsheet

always run tmux -2 for vim colors
### Starting and connecting
`prefix` = `ctrl-b`

`$ tmux -V` version (update on trusty http://witkowskibartosz.com/blog/update-your-tmux-to-latest-version.html#.XJyIAKczYUF)

`$ tmux ls` view running sessions

`$ tmux new -s session_name` create new session

`$ tmux a -t session_name` attach to named session

`$ tmux kill-session -t session-name` kill session

### Sessions
`prefix` and ...

`:new<CR>` new session

`s` list sessions

`$` name session

`d` detach from session

### Windows (tabs)
`prefix` and ...

`c` create

`,` name it

`&` kill

### Panes (splits)
`prefix` and ...

`%` vertical split

`"` horizontal

`z` toggle zoom

`t` show big clock in pane ;)

`x` kill

`<space>` toggle layout (cool feature)

```
PREFIX : resize-pane -D (Resizes the current pane down)
PREFIX : resize-pane -U (Resizes the current pane upward)
PREFIX : resize-pane -L (Resizes the current pane left)
PREFIX : resize-pane -R (Resizes the current pane right)
PREFIX : resize-pane -D 20 (Resizes the current pane down by 20 cells)
PREFIX : resize-pane -U 20 (Resizes the current pane upward by 20 cells)
PREFIX : resize-pane -L 20 (Resizes the current pane left by 20 cells)
PREFIX : resize-pane -R 20 (Resizes the current pane right by 20 cells)
PREFIX : resize-pane -t 2 20 (Resizes the pane with the id of 2 down by 20 cells)
PREFIX : resize-pane -t -L 20 (Resizes the pane with the id of 2 left by 20 cells)
```

### restore session after restart

https://andrewjamesjohnson.com/restoring-tmux-sessions/

https://github.com/tmux-plugins/tpm#installation
```
set -g @plugin 'tmux-plugins/tmux-resurrect'
set -g @plugin 'tmux-plugins/tmux-continuum'

set -g @continuum-restore 'on'
```

# Links
https://gist.github.com/MohamedAlaa/2961058
