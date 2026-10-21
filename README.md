# tmux

```
set -g mouse on
set-option -g set-clipboard on
setw -g mode-keys vi


bind-key -T copy-mode-vi Enter send-keys -X copy-pipe-and-cancel "xclip -selection clipboard -i"

bind -T copy-mode-vi MouseDragEnd1Pane send-keys -X copy-pipe "xclip -selection clipboard -i"
```
