# git tips

* reset branch (no push): `git checkout mybranch && git reset --hard origin/mybranch`
* amend: `g commit --amend -m "message" && g push --force`
* `g whatchanged`
* git reflog = reference log, local log (in .git), last resort
* always rebase during pull: `git config pull.rebase true`

[git]
