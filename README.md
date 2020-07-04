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
PREFIX followed by `%`
# results in:
# -------------
# |     |     |
# |     |     |
# |     |     |
# -------------

PREFIX followed by `"`
# results in:
# -------------
# |           |
# |-----------|
# |           |
# -------------
```
