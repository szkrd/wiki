# git aliases

```
  aa = add --all
  cl = clone
  f = fetch --prune
  co = checkout
  cob = !sh -c 'git checkout -b $1 && git push -u --no-verify origin $1' -
  cogr = !sh -c 'git branch --all --color=never | grep --color=never $1 | sed -n -e "s-remotes/origin/--p" | xargs git checkout' -
  cof = !sh -c 'git co feature/$1' -
  cod = checkout development
  ci = commit
  cam = commit -am
  camN = commit --no-verify -am
  whoops = commit --amend -all
  caa = !git add --all && git commit
  go = !git add --all && git commit && git push
  br = branch
  brkill = !sh -c 'git branch -D $1 | git push --no-verify origin :$1' -
  rb = rebase
  rbi = rebase --interactive
  rbc = rebase --continue
  rba = rebase --abort
  pop = stash pop
  s = status
  ss = status -s
  pu = push
  puf = push -f
  puN = push --no-verify
  pom = push origin master
  md = merge development
  uncommit = reset --soft HEAD^
  slap = !git clean -fd && git reset --hard && git checkout . && git status
  flush = stash clear
  p = pull
  pr = !git fetch && git pull --rebase
  sp = !git stash && git fetch && git pull && git stash pop
  lg = log --pretty=format:\"%C(auto)%h %Cblue%ad%Creset | %s%d [%Cgreen%an%Creset]\" --graph --date=short
  bra = !git branch --all | perl -pe 's/remotes\\/origin\\//\\033[36mR:\\033[0m /g' | perl -pe 's/\\* (.*)/ \\033[100m\\033[97m[$1]\\033[0m/'
  mergedev = !BRANCH=`git s | head -n 1 | perl -pe 's/On branch //'` && git co development && git pull && git co $BRANCH && git merge development
  prunedev = !git branch --merged development | grep -v ' development$' | xargs git branch -d
  where = !git remote show origin | grep URL | sed -e 's/^ *//'
  cdiff = !git diff --color | diff-so-fancy | less -r
```

[git], [alias], [config], [dotfile]
