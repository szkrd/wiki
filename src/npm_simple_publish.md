# npm init, scoped publish

Do setup npm first

```bash
npm set init.author.name "Your Name"
npm set init.author.email "you@example.com"
npm set init.author.url "http://yourblog.com"
npm adduser
```

* to test the binary section: `npm link` (later on `npm unlink .`)
* pakmanager is _chatty_

```bash
npm init --scope=johndoe
npm install -g pakmanager
pakmanager deps
npm publish --access=public
```

[npm]
