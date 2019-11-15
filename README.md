gitster
=======

A fork of shashankmehta's [gitster] theme.

![gitster theme]

What does it show?
------------------

  * Red `➜` when last command failed, green otherwise.
  * Current working directory, relative to the git root when in a git repo.
  * Current git branch name, or commit short hash when in ['detached HEAD' state].
  * Yellow `✗` when in a dirty git working tree, green `✓` when in a clean one.

Requirements
------------

Requires Zim's [git-info] module to show git information.

[gitster]: https://github.com/shashankmehta/dotfiles/blob/master/thesetup/zsh/.oh-my-zsh/custom/themes/gitster.zsh-theme
[gitster theme]: https://zimfw.github.io/images/prompts/gitster.png
['detached HEAD' state]: http://gitfaq.org/articles/what-is-a-detached-head.html
[git-info]: https://github.com/zimfw/git-info
