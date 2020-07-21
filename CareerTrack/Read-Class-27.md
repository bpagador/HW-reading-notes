#### setState explained
- only legit way of updating state after the initial state setup = setState()
- setState responds with an answer--otherwise known as reconciliation--when a component passes an object that contains the part of the state we want to update
#### Reconciliation
- the process through which the React updates the DOM
- created a virtual DOM and compares it to the current DOM
    - the virtual DOM contains the new state of the component 
#### Typechecking Props
- a good way to catch a lot of bugs in a growing app
- to run typechecking on the props for a component, you can assign the special propTypes property (this is built in to JS extensions like Flow and Typescript)
#### snapshot testing
- use enzyme and jest to capture and match the rendered output with expected output/previous snapshot
- to update snapshots: jest --updateSnapshot
#### static rendering - enzyme
- uses render() function to generate HTML from your React tree
- renders all children
#### shallow mounting - enzyme
- uses componentDidMount and componentDidUpdate
#### full mounting - enzyme
- ideal for use cases for when you have components that may interact with DOM APIs or need to test components that are wrapped in higher order components