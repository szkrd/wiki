# enzyme

[Scary monster](http://guyver.wikia.com/wiki/Enzyme_I). Guyver rocks.

react e2e testing - https://github.com/airbnb/enzyme

* `shallow` - string, isolated
* `full` - jsdom, full lifecycle (mount, unmount)
* `static` - cheerio only (no interaction)

## tricks

* enzyme change checkbox: `.simulate('change', {target: {checked: true}})`
* get value: `expect(wrapper.find('#user-id').get(0).value).to.equal('123')`

[e2e], [test], [react]
