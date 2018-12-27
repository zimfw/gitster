gitster
=======

A fork of shashankmehta's
[gitster](https://github.com/shashankmehta/dotfiles/blob/master/thesetup/zsh/.oh-my-zsh/custom/themes/gitster.zsh-theme)
theme.

What does it show?
------------------

  * Red `➜` when last command failed, green otherwise.
  * Current working directory, relative to the git root when in a git repo.
  * Current git branch name, or commit short hash when in
    ['detached HEAD' state](http://gitfaq.org/articles/what-is-a-detached-head.html).
  * Yellow `✗` when in a dirty git working tree, green `✓` when in a clean one.

Usage
-----

If you enabled Zim's [`prompt`](https://github.com/zimfw/prompt) module, you can
set this as your default theme with the following zstyle:

    zstyle ':zim:prompt' theme 'gitster'

Requirements
------------

Requires Zim's [`git-info`](https://github.com/zimfw/git-info) module to show
git information.
