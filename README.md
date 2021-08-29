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

You can customize how the current working directory is shown with the
[prompt-pwd module settings].

The git indicators can customized by changing the following git-info module
context formats:

| Context name | Description       | Default format |
| ------------ | ----------------- | -------------- |
| branch       | Branch name       | `%b`           |
| commit       | Commit short hash | `%c`           |
| clean        | Clean state       | `%F{green}✓`   |
| dirty        | Dirty state       | `%F{yellow}✗`  |

Use the following command to override a git-info context format:

    zstyle ':zim:git-info:<context_name>' format '<new_format>'

For detailed information about these and other git-info settings, check the
[git-info documentation].

These advanced settings must be overridden after where the theme is initialized.

Requirements
------------

Requires Zim's [prompt-pwd] module to show the current working directory, and
[git-info] to show git information.

[gitster]: https://github.com/shashankmehta/dotfiles/blob/master/thesetup/zsh/.oh-my-zsh/custom/themes/gitster.zsh-theme
['detached HEAD' state]: http://gitfaq.org/articles/what-is-a-detached-head.html
[prompt-pwd module settings]: https://github.com/zimfw/prompt-pwd/blob/master/README.md#settings
[git-info documentation]: https://github.com/zimfw/git-info/blob/master/README.md#settings
[prompt-pwd]: https://github.com/zimfw/prompt-pwd
[git-info]: https://github.com/zimfw/git-info
