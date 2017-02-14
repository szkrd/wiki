# brew

* `brew list --versions` = all installed
* `brew leaves` = top level items
* `brew search node` = search for packages w 'node' in their name
* `brew update`
* `brew doctor`
* `brew upgrade`
* `brew upgrade node4-lts` = upgrade node4-lts package only
* `brew switch node4-lts 4.4.4` = downgrade node lts
* `brew cleanup node4-lts` = remove older versions

Deep removal is not yet implemented. Install rmtree, then `brew rmtree LEAF`

Bleeding edge node: `brew remove nodeX-lts && brew install node` (where X is the lts id)

[brew], [mac], [osx]
