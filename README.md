# README.md

`todo` is a Bash script I use to display my Markdown to-do list. `todo` is
written in pure Bash, and assumes that your terminal supports the following:

```bash
head_fmt=$'\e[1m'       # Bold
done_fmt=$'\e[2m\e[93m' # Dim and bright yellow
dtxt_fmt=$'\e[2m\e[9m'  # Dim and strikethrough
todo_fmt=$'\e[93m'      # Bright yellow
ttxt_fmt=$'\e(B\e[m'    # Reset
res_fmt=$'\e(B\e[m'     # Reset
```

## Setup

To use `todo`, you must set and export `$MY_TODO_PATH`. Additionally, you must
set and export either `$VISUAL` or `$EDITOR`.

```text
Options:
  -d, --display-list
    Display a list of tasks
    '$MY_TODO_PATH' must be set and exported

  -e, --edit-list
    Edit a list of tasks
    '$MY_TODO_PATH' must be set and exported
    Either '$VISUAL' or '$EDITOR' must be set and exported

  -h, --help
    Display this message and exit
```
