# jupyterlab-vim-jk-swap

Personal fork of [jupyterlab-contrib/jupyterlab-vim](https://github.com/jupyterlab-contrib/jupyterlab-vim) with j/k keys swapped.

## Changes from upstream

- `j` moves up, `k` moves down (swapped from default)
- Applies to vim normal/visual mode, Jupyter command mode, and Shift+J/K selection

## Install

```bash
git clone https://github.com/alsibassi/jupyterlab-vim-jk-swap.git
cd jupyterlab-vim-jk-swap
pip install -e .
jupyter labextension develop . --overwrite
jlpm run build
```

## Syncing with upstream

```bash
# Add upstream remote (one time)
git remote add upstream https://github.com/jupyterlab-contrib/jupyterlab-vim.git

# Fetch and merge upstream changes
git fetch upstream
git merge upstream/main

# Rebuild after merge
jlpm install
jlpm run build
```
