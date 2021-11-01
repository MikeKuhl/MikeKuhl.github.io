# Problem Domain and Primitive Values #

- JavaScript currently supports eight data types. All of these data types (Booleans, Null, Undefined, Number, BigInt, String, Symbol) are primitive values except for object references.

- Many common data types such as arrays, functions, and dates are object references under the hood.

- Primitive values can be stored in variables directly. Objects, on the other hand, are stored as references. A variable that has been assigned an object does not store that object directly, it stores the memory address of the location that the object exists at.

- Primitive values are immutable — they cannot be changed after being created. Object references, however, are mutable and can be changed.

- Since objects are stored as references, special care must be taken when duplicating objects and when performing equality checks on objects.


- Understanding how these operations work can be confusing for newcomers to JavaScript, but they make sense once you understand how the language’s type system works.

- Developing a strong grasp of primitive values, object references, and mutability is a critical step in progressing past the beginner stages of JavaScript programming.

- This knowledge will help you identify bugs, understand key differences in programming paradigms, and help you understand your code at a deeper level.

- Problem Domain is more so the understanding of the problem at and clearly and precisecly some things can be vague so having a full understanding of a problem is very helpful when coming to a solution that fully solves a problem. Which can only be helped by communicating and understanding how to make the problem itself easier.

# OBJECTS #

- if a variable is part of an object it is called a "property"
- Properties tell us about the object, such as name of a hotel and how many rooms.
-In an object a function is called a Method. Methods represent a task that are associated with the object.
-methods have  a named and a value or a Key Value Pair.

- Creating the object looks something like this
```js

var hotel = {
    name:'Quary',
    rooms:40,
    booked:25,

    checkAvailability: function(){
        return this.rooms - this.booked;
    }
};
```

```js
var hotelName = hotel.name;
var roomsFree = hotel.checkAvailability

// or

var hotelName = hotel['name']
var roomsFree = hotel['checkAvailability']();
```
- Above the first example is how you normally would access an object using DOT NOTATION. The second style is commonly used when there is a special character or the property is a number.

- the 'new' keyword allows you to create a new object  from an object contsructor.

- You can update an object like so 'hotel.name = ['park']'

- you can delete a property by doing 'delete hotel.name' or clear a property by doing hotel.name=''.


# DOM #

- The browser represents the page using a DOM tree.

- DOM trees have four types of nodes: document nodes, element nodes, attribute nodes, and text nodes

- You can select element nodes by their ID or class attributes by tag name or using CSS selector syntax.

- Whenever a DOM query can return more than one node it will always return a NodeList.

- From an element node, you can ccess sand update its content using properties such as textContent and innnerHTML or using DOM manipulation techniques.

- An element node can contain multiple text nodes and child elements that are sibling of each other.

- in older browsers, implementation of the DOM is inconsistent.

- Browsers offer tools for viewing the DOM Tree