# task ids

```bash
function mytasks () {
  git log --all --pretty=format:"%Cblue%ad%Creset | %s%d" --author="John Doe" --date=short | \
  grep --color=never -E "(feat|chore|docs|fix|refactor| style|test)\(" | \
  grep -v 'Merge branch' | \
  grep --color=always -E "EVILCORP-[0-9]+" | \
  head -n 15;
}
```

replace name and company pls

## tfs id version

```bash
function mytasks () { NAME="John Doe" git log --all --pretty=format:"%Cblue%ad%Creset | %s%d" --author="$NAME" --date=short | grep --color="never" " | #" | grep --color=never -E "(feat|chore|docs|fix|refactor| style|test)\(" | grep -v 'Merge branch' | grep --color=always -E "#[0-9]+ " | head -n 15; }
```

## daily tasklist

```bash
alias taskstoday='mytasks | grep "$(date +%Y-%m-%d)" | grep --color=never -o -E "#[0-9]+" | sort -u  | tr "\n" " " > /dev/clipboard'
```

[bash], [work]
