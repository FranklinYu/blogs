# Zsh v.s. Bash

Reasons I prefer Zsh over Bash:

* Zsh has native arrays. In bash we have to simulate arrays with space/colon
  separated string, but it is difficult to modify, considering all the edge
  cases.
* Zsh has many [hook functions][1]; Bash only has `$PROMPT_COMMAND` which does
  the same as `precmd` hook in Zsh (other functionality may be simulated with
  hack, e.g. [`preexec`][2]).

Reasons I prefer Bash over Zsh:

* Availability. For example, available on Linux out-of-the-box. This is critical
  when working on a system without super-user permission being granted.

[1]: http://zsh.sourceforge.net/Doc/Release/Functions.html#Hook-Functions
[2]: http://superuser.com/questions/175799/does-bash-have-a-hook-that-is-run-before-executing-a-command
