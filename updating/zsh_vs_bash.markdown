# Zsh v.s. Bash

Reasons I prefer Zsh over Bash:

 *  Zsh can bind array to scalar variable like `$path` and `$PATH` with
    `typeset -T`.
 *  Zsh has many [hook functions][1]; Bash only has `$PROMPT_COMMAND` which does
    the same as `precmd` hook in Zsh (other functionality may be simulated with
    hack, e.g. [`preexec`][2]).
 *  Zsh completion can have one-line note for each candidates. In most cases
    this saves a manual check.
 *  [Fish like syntax highlight][3].

Reasons I prefer Bash over Zsh:

 *  Availability. For example, available on most Linux distributions
    out-of-the-box. This is critical when working on a system without super-user
    permission being granted.

[1]: http://zsh.sourceforge.net/Doc/Release/Functions.html#Hook-Functions
[2]: http://superuser.com/questions/175799/does-bash-have-a-hook-that-is-run-before-executing-a-command
[3]: https://github.com/zsh-users/zsh-syntax-highlighting
