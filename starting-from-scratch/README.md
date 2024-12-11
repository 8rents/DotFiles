# Starting from Scratch

> *Creating a bare git repository to hold dotfiles from scratch*

---

## Getting started

I'm going to create a side git repo called `~/dotfiles` to hold all my dotfiles.

We are going to set the "working tree" (aka where the files are actually stored and read from) to your `$HOME` (aka `~/`) folder.

Then we are going to set git config to not show untracked files when called

```bash
# Create a bare git repo to hold all your dotfiles
git init --bare $HOME/dotfiles

# create a git alias called config
alias config='/usr/bin/git --git-dir=$HOME/dotfiles/ --work-tree=$HOME'

# Set the config alias you just made to not show untracked files when status is called
config config --local status.showUntrackedFiles no

# add an alias to your bashrc file too
echo "alias config='/usr/bin/git --git-dir=$HOME/dotfiles/ --work-tree=$HOME'" >> $HOME/.bashrc
```

*more on this later...*

---

(<3) 2024 8rents 