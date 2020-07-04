<p align=center>
  <img src="https://upload.wikimedia.org/wikipedia/commons/e/e4/Tmux_logo.svg" />
</p>

Prefix for issuing the commands in the `tmux` (standard):

`CTRL + B`

Starting `tmux` session:

```bash
# a "standard" way
tmux

# named instance
tmux new -s <name>
```

Listing the started sessions:

```bash
tmux ls
```

Stopping/killing a named session:

```bash
tmux kill-session -t <name>
```

## Panes/splits

```bash
# horizontal splitting
PREFIX followed by `%`
# results in:
# -------------
# |     |     |
# |     |     |
# |     |     |
# -------------

# vertical splitting
PREFIX followed by `"`
# results in:
# -------------
# |           |
# |-----------|
# |           |
# -------------

# navigate to the tab by numbers
PREFIX followed by `q` and then pressing the number of the pane that shows up
# results in:
# -------------
# |     |  1  |
# |  0  |-----|
# |     |  2  |
# -------------

# move the current pane to the left
PREFIX followed by `{`
# results in (if you're focused in Y pane for example):
# -------------     -------------
# |     |  Y  |     |     |  X  |
# |  X  |-----|  -> |  Y  |-----|
# |     |  Z  |     |     |  Z  |
# -------------     -------------

# move the current pane to the right
PREFIX followed by `}`
# results in (if you're focused in X pane for example):
# -------------     -------------
# |     |  Y  |     |     |  X  |
# |  X  |-----|  -> |  Y  |-----|
# |     |  Z  |     |     |  Z  |
# -------------     -------------
```

## Windows

```bash
# create a new window
PREFIX followed by `c`

# list all windows
PREFIX followed by `w`

# find a window
PREFIX followed by `f`

# navigate to the next window
PREFIX followed by `n`

# navigate to the previous window
PREFIX followed by `p`

# give a name to the window
PREFIX followed by `,`

# kill the window instance
PREFIX followed by `&`
```
