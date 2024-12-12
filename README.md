# Debian DotFiles

> *DotFiles for Debian based Linux Installs*

---

Debain is the most generic type of linux branch and will likely be used to create the later branches instead of starting from scratch

## How to use this repository

This is the branch for use with debian installs that have a desktop.

### Fork this repositiory to your own GitHub Account and clone it

```bash
# 1. Clone this repository to your `~/.config` folder
git clone https://github.com/--your-github-account--/dotfiles $HOME/.config

# 2. change directory into the correct branch
cd ~/.config

# 3. Switch to the Debian branch
git switch debian

# 4. Add this (8rents) dotfiles repository as the upstream repo so you can optionally pull in changes that I make
git remote add upstream https://github.com/8rents/dotfiles
```


### Check that there are more than one gitub remote attached to your repo

```bash
# List remotes attached to this repo
git remote -v
```

You should see:

- origin - Your backup of your dotfiles. (this could be better renamed to `original` or `8rents`)
- upstream - The original repo that you can optionally pull updates from (this could be better renamed to `github` or maybe `backup`)                                         



> You should see something like this:

```bash
> origin    https://github.com/YOUR-USERNAME/dotfiles.git (fetch)
> origin    https://github.com/YOUR-USERNAME/dotfiles.git (push)
> upstream  https://github.com/8rents/dotfiles.git (fetch)
> upstream  https://github.com/8rents/dotfiles.git (push)
```

- fetch is where you pull the repo from
- push is where you send changes to 

---

**(ɔ) 2024 [Brenton Holiday](https://brenton.holiday)**
