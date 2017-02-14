# tricky calls

- `have.been.calledWith` - what the heck was the call? `console.log(mySpy.getCall(0))`
- the above w a jQuery spy: `$.fn.height.getCall(0).thisValue[0]`
- exact deep calledWith for last call: `expect(mySpy.lastCall).to.be.calledWith({x: true, y: true})`

[sinon], [test]
