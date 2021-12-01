# Passing Functions as Props #


## List and keys ##
- What does .map() return?
the map method creates a new array populated with results of calling a provided function on every element in the calling array.

- If I want to loop through an array and display each value in JSX, how do I do that in React?
map() method is the most cmonnly used function to iterate over an array in JSX. You can attach map() to the array and pass a callback.
- Each list item needs a unique ____.
Key
- What is the purpose of a key?
Keys help React identify which items have changed, are added, or are removed. Keys give the elements inside the array a stable identity.

## Spread Operator ##

-What is the spread operator?
It allows an iterable, like an array or string to be expanded in places where arguments or elements are expected.

-List 4 things that the spread operator can do.
Copy an array, Concatenate or combine arrays, Math functions, Use array as arguments.
-Give an example of using the spread operator to combine two arrays.
```Javascript
const firstArr = [1,2,3]
const secondArr = [4,5,6]
const combinedArr = [...firstArr,...secondArr]
console.log(combinedArr) //1,2,3,4,5,6
```
-Give an example of using the spread operator to add a new item to an array.
```Javascript
const firstArr = [1,2,3]
const secondArr = [4,5,6,...firstArr]
console.log(secondArr) //4,5,6,1,2,3

```
-Give an example of using the spread operator to combine two objects into one.

```javascript
const cold = {cold:"brew"}
const hot = {hot:"brew"}
const coldHot = {...cold,...hot}
console.log(coldHot)
```


# How to pass Functions Between components #

-In the video, what is the first step that the developer does to pass functions between components?

-In your own words, what does the increment function do?
Takes in an object from the state and increments the count of the person. Then it updates the state at the end.
-How can you pass a method from a parent component into a child component?
By using the passed function as a prop with the help of another function.
-How does the child component invoke a method that was passed to it from a parent component?
By using "this.props." and calling the method that is being passed from the parent.