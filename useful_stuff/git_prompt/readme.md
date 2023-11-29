# Shell scripts for git prompt

Reference scripts stolen from somewhere for activating the git-friendly prompt.

For non-login shells just source the `git-prompt.sh` script. E.g. (assuming you have copied the files in the `/path/to/dir` directory) by writing in your `.bashrc`

```
source /path/to/dir/git-prompt.sh
```

For login shells, first enable the git-prompt variable `__git_ps1` by sourcing `enable-git-prompt.sh` then run the `git-prompt.sh` script.
E.g. (assuming you have copied the files in the `/path/to/dir` directory) by writing in your `.bash_profile`:

```
source /path/to/dir/enable-git-prompt.sh
source /path/to/dir/git-prompt.sh
```

## if ``__git_ps1`` is enabled:

```bash
GIT_PS1_SHOWDIRTYSTATE=true
GIT_PS1_SHOWSTASHSTATE=true
GIT_PS1_SHOWUNTRACKEDFILES=true
GIT_PS1_SHOWUPSTREAM="auto"
GIT_PS1_HIDE_IF_PWD_IGNORED=true
GIT_PS1_SHOWCOLORHINTS=true
export PS1="\t \[\033[01;32m\]\w\[\033[01;33m\]\$(__git_ps1)\[\033[01;00m\] $ "
```
