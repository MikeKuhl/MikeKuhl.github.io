# React Lifecycle


[react lifecyle](https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093)
- Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?
Render
- What is the very first thing to happen in the lifecycle of React?
Constructor
- Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates
constructor, render,componentDidMount,ComponentWillUnmount, React Updates
- What does componentDidMount do?
 It's a hook that gets invoked right after a React component has been mounted or the first render.

# Props and State
[react state vs props](https://www.youtube.com/watch?v=IYvD9oBCuJI)

-What types of things can you pass in the props?
Any data type, strings, functions, objects, etc.
-What is the big difference between props and state?
Props are variables passed by the parent components. State while still being a variable are directly initialized and managed by the component.
-When do we re-render our application?
Whenever there is a change in the state.
-What are some examples of things that we could store in state?
 a string, a number or an object, etc. Any data we will be working with.
