# workspace

Assorted utilities for navigating various workspaces.

## Installation

```bash
git clone https://github.com/okkays/workspace
./install
```

## Dependencies

Workspace makes use of:

-   [junegunn/fzf](https://github.com/junegunn/fzf)
-   [ggreer/the_silver_searcher](https://github.com/ggreer/the_silver_searcher)
-   [okkays/ghd](https://github.com/okkays/ghd)

## Features

`workspace` looks for the nearest `git` or `hg` root, and does `ls`, `ag`, and a
few other features based on that reference point. It has special considerations
for .g4d. When outside of workspace, `.` is treated as the current workspace (so
ls and ag work as normal).

For more on the use of `workspace`, see `workspace help`.

Workspace also installs the following aliases:

```bash
alias wd="jump_to_workspace_directory"
alias ws=workspace
```
