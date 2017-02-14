# spy or stub?

stub - REPLACES the prop

* `this.sandbox.stub(_, 'debounce', (fn, timeout) => fn)`
* `this.sandbox.stub(Date, 'now', () => 1464984175931)`

spy - WRAPS the prop (can create new fn of course)

* `this.sandbox.spy($.fn, 'off')`
* `myApi = {put: sinon.spy(), dele: sinon.spy()}`

[sinon], [test]
