gitster
=======

A fork of shashankmehta's [gitster] theme.

<img width="706" src="https://zimfw.github.io/images/prompts/gitster@2.png">

What does it show?
------------------

  * Red `➜` when last command failed, green otherwise.
  * Current working directory, relative to the git root when in a git repo.
  * Current git branch name, or commit short hash when in ['detached HEAD' state].
  * Yellow `✗` when in a dirty git working tree, green `✓` when in a clean one.

Advanced settings
-----------------

This theme can customized by changing the following git-info module context
formats, after the theme has been initialized:

| Context name | Description       | Default value |
| ------------ | ----------------- | ------------- |
| branch       | Branch name       | `%b`          |
| commit       | Commit short hash | `%c`          |
| clean        | Clean state       | `%F{green}✓`  |
| dirty        | Dirty state       | `%F{yellow}✗` |

Use the following command to change the value of a context format:

    zstyle ':zim:git-info:<context_name>' format '<new_value>'

For detailed information, check the [git-info documentation].

Requirements
------------

Requires Zim's [git-info] module to show git information.

[gitster]: https://github.com/shashankmehta/dotfiles/blob/master/thesetup/zsh/.oh-my-zsh/custom/themes/gitster.zsh-theme
['detached HEAD' state]: http://gitfaq.org/articles/what-is-a-detached-head.html
[git-info documentation]: https://github.com/zimfw/git-info/blob/master/README.md#theming
[git-info]: https://github.com/zimfw/git-info
