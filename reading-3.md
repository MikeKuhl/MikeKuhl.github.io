# Lists #
- There are three types of HTML lists ordered,unordered and definition

- Ordered lists use numbers
- Unordered lists use bullets
-Deifinition lists are used to define terminology.
- List can be nested inside one another
```
<ul>Test</ul>
<ol>test</ol>
<dl>test</dl>
<ul>test</ul>
```

# Boxes #

- Everything in CSS has a box around it and CSS treats each HTML element as such.
- CSS can control the box dimensions
- Including borders,margins and padding
- Properties can also hide elements
- Borders can also be images and rounded borders



```
p,
ul {
  border: 2px solid rebeccapurple;
  padding: .5em;
}

.block,
li {
  border: 2px solid blue;
  padding: .5em;
}

ul {
  display: flex;
  list-style: none;
}

.block {
  display: block;
}
```

# Arrays #

- Arrays store lists of values
- Arrays start at [0]
- You can select where you want in an Array by selecting  Such as Array[2] which would take you to the third entry.
- You can also change the values in an array
```
const cars = ["Saab", "Volvo", "BMW"];
```
# Loops and Logic #

- Comparison operators allow you to combine comparison operators.
- If...else allows for multiple conditions to be met
- switch statements allow you to compare a value against possible outcomes.
- Data types can be switched from one to another
- All values can evaluate to either truthy or falsy
- Three types of loops, For Loops, While Loops, Do While loops

```
for (let i = 0; i < cars.length; i++) {
  text += cars[i] + "<br>";
}
```