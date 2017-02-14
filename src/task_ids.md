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

[bash], [work]
