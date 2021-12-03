## Putting it all together ##

# Thinking in React

- What is the single responsibility principle and how does it apply to components?
 a component should ideally only do one thing. If it ends up growing, it should be decomposed into smaller subcomponents.


What does it mean to build a ‘static’ version of your application?
- Build a non interative version not using state.
Once you have a static application, what do you need to add?
-add interactivity
What are the three questions you can ask to determine if something is state?
How can you identify where state needs to live?
- Is it passed in from a parent via props?

If so, it probably isn’t state.
Does it remain unchanged over time? If so, it probably isn’t state.

Can you compute it based on any other state or props in your component? If so, it isn’t state.

# High Order Function

What is a “higher-order function”?
- Functions that operate on other functions, either by taking them as arguments or by returning them, are called higher-order functions

Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?
- Comparing if M is greater than or equal to M greate rthan N
Explain how either map or reduce operates, with regards to higher-order functions.
Map or reduce methods transform an array by applying a function to all of its elements and building a new array from the returned values. In a way the content has been mapped to a new form by the function.