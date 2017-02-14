# bashprofile on osx

from 2016 and before (ela/rs)

```bash
alias grep="grep --color=always"
alias ls="ls -G"
alias lls="ls -la"
alias l="lls"
alias la="ls -A"
alias cls="clear"
alias md="mkdir"
alias cdf="echo you are looking for 'fcd' or possibly 'clipcd'"
alias cd..="cd .."
alias cd....="cd ../.."
alias up="cd .."
alias upup="cd ../.."

function fcd () { cd `dirname $1`; }
function clipcd () { fcd `pbpaste`; }
function mdcd () { mkdir -p "$@" && cd "$@"; }

alias showFiles='defaults write com.apple.finder AppleShowAllFiles YES; killall Finder /System/Library/CoreServices/Finder.app'
alias hideFiles='defaults write com.apple.finder AppleShowAllFiles NO; killall Finder /System/Library/CoreServices/Finder.app'
alias fuckdock='defaults write com.apple.dock autohide-delay -float 1000 && killall Dock'
alias unfuckdock='defaults delete com.apple.dock autohide-delay && killall Dock'

alias rebash='source ~/.bash_profile'
alias tm="open -a TextMate"
alias finder="open -R ./"
alias g='git'
alias pyhttp='python -m SimpleHTTPServer 1337'
alias stree='open -a SourceTree'

PS1='\[\e[0;32m\]\u\[\e[m\] \[\e[1;34m\]\w\[\e[m\] \[\e[1;32m\]\$\[\e[m\] \[\e[0;37m\]'

export HISTCONTROL=ignoredups
PATH=$PATH:~/bin:/usr/local/sbin
EDITOR=sublime
LANG=en_EN.UTF-8
LC_ALL=en_US.UTF-8
LC_ctype=en_US.UTF-8
export JAVA_HOME=`/usr/libexec/java_home`
export NPM_TOKEN=xxxxxxx1-x111-1xxx-1xx1
export HOMEBREW_GITHUB_API_TOKEN="xxxxxxxxxxxxxxxxxx"
```

[bash], [dotfile]
