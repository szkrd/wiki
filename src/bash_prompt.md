# bash prompt

yet another bash prompt

```bash
function parse_git_branch() { git branch 2> /dev/null | sed -e '/^[^*]/d' -e 's/* \(.*\)/ (\1)/' | sed -e 's/feature/F/'; }
PS1='\[\e[0;32m\]\u\[\e[m\] \[\e[1;34m\]\w\[\e[m\]\[\e[0;33m\]$(parse_git_branch) \[\e[1;32m\]\$\[\e[m\] \[\e[0;37m\]'
```

[bash], [prompt]
