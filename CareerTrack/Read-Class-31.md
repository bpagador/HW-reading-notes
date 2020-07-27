#### hooks api
- hooks don't contain any breaking changes, they're "backwards compatible"
- you can use them without rewriting any existing code 
- provide a more direct API to props, state, context, refs, and lifecycle (have we heard about this one yet? idk)
- hooks offer a powerful way of combining all of them aforementioned
- example of a hook: useState
    -which can be used more than once in a single components
#### state hook
- hooks don't work inside classes, they can be used IN PLACE OF classes
- note: in a function component you don't have "this" so you can't assign or read this.state
    - instead: useState
    - which declares a state variable
    - the only argument to the useState() hook is the init state
    - the state does NOT have to be an object, we can keep a number or string in there no prob
    - useState() returns 1. the current state and 2. the function that updates it 
#### effects hook
- let's you perform side effects in func components
- example: useEffect()
    - this is you telling React that your components needs to do something after render 
    - placing useEffect inside the comonent lets us access any props right from the effect (it's already in the fucn scope)

