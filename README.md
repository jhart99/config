# Dotfiles
My dotfiles for setting up new machines

To install just do the following:
```
alias config='/usr/bin/git --git-dir=$HOME/.cfg/ --work-tree=$HOME'
echo ".cfg" >> .gitignore
git clone --bare <git-repo-url> $HOME/.cfg
config checkout
```
And then to get everything up and going you need to source the Xresources using this
```
xrdb .Xresources
```
If the files already exist, you need to move them or remove them first.

Based off of https://developer.atlassian.com/blog/2016/02/best-way-to-store-dotfiles-git-bare-repo/

[![Analytics](https://ga-beacon.appspot.com/UA-110461825-1/config?pixel)](https://github.com/jhart99/config)
