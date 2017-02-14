# semver release

1. `npm version major/minor/patch -m 'message'`
2. `ccl` (conventional changelog)
3. `g push --tag`

OR just use semantic-release(with karma/angular/semver style commit messages)

## other note (pm's version)

1. `git pull --rebase)`
2. in package.json modify version
3. `ccl` (same as: git fetch --tags && conventional-changelog -i CHANGELOG.md -o CHANGELOG.md)
4. commit (add --all, commit -m '…')
5. add chore message: _"chore(package): bump version to 1.2.3"_
6. on github: "Draft new release"

[semrel], [semver], [release]
