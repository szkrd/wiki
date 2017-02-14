# npm link

symlink packages w no effort

1. enter foo-models --> `npm link`
2. change to foo-admin (which uses foo-models) -> `npm link foo-models`
3. finally `npm unlink && npm i` and be happy

Don't forget, private package @ may need to be escaped:  
\@hiddenFoo/bar

[npm]
