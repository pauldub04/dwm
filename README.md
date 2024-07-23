# dwm
This is my fork of dwm, first wm that I want to try on my machine

The master branch is where I place my current state of dwm, here I change the config.\
The upstream remote is for the [source code](https://git.suckless.org/dwm/).

[Article](https://dwm.suckless.org/customisation/patches_in_git/) about customization

## add patch
To add a patch I create a fork branch from `upstream/master`, load a new diff file to `patches` dir and then apply it with `patch` or `git apply`. If `config.def.h` is changed, I update `config.h` in the same branch. Then I merge it to master and usually because `config.h` was edited in both branches the conflict arises. I resolve the conflict manually and commit the merge

## update dwm
To update dwm I need to pull changes to the `upstream/master` and then just merge it to master. (or maybe just rebase, later need to try what is better in the case...)
