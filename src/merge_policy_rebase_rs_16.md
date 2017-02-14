# rebase centric model

1. g co -b feat/shiny-foo
2. commit stuff to branch
3. github pull request (do NOT push the merge button)
4. set "waiting for review" label
5. if everything's okay, squash children (g rbi 12345EF)
6. force push
7. g co master && gfp && g co feat/shiny-foo && g rb master && g puf
8. g co master && g rb feat/shiny-foo && g push origin master

[git]
