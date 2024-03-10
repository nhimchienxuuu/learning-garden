---
mindmap-plugin: basic
time: 
tags:
---
# info
- source: [https://scrimba.com/learn/learnjavascript](https://scrimba.com/learn/learnjavascript)
- code: /Users/chanity/Documents/Study/CompSci/CS_learnings/JS
# note
## ReferenceError - console log before initializing
#### hoisting method
- In JavaScript, if you try to use a variable before it has been declared or initialized, you’ll get a `ReferenceError`. This is because JavaScript uses a mechanism called “hoisting”, which moves variable and function declarations to the top of their containing scope during the compile phase. However, only the declarations are hoisted, not the initializations.

Here’s an example:

JavaScript

```javascript
console.log(myVar); // Output: ReferenceError: myVar is not defined
var myVar = 5;
```

AI-generated code. Review and use carefully. .

In this case, even though `myVar` is declared and initialized after the `console.log` statement, JavaScript doesn’t know about `myVar` when it tries to log it. This is why you get a `ReferenceError`.

However, if you declare `myVar` before the `console.log` statement, like this:

JavaScript

```javascript
var myVar;
console.log(myVar); // Output: undefined
myVar = 5;
```

AI-generated code. Review and use carefully. .

In this case, `myVar` is `undefined` when it’s logged, because it has been declared but not yet initialized. This is a key aspect of JavaScript’s execution context and hoisting mechanism. It’s always a good practice to declare and initialize your variables before you use them to avoid such errors.

#### compiled language
JavaScript is often referred to as an interpreted language, but in reality, it’s a **Just-In-Time (JIT) compiled language**. This means that JavaScript code is compiled just before it’s executed, rather than being compiled ahead of time like in some other languages.

Here’s a simplified explanation of the process:

1. **Compilation Phase**: The JavaScript engine first scans the code during the “compilation” phase. During this phase, it recognizes variable and function declarations and hoists them to the top of their scope. However, the values aren’t assigned yet, so if a variable is declared using `var`, it’s initialized with a value of `undefined`.
    
2. **Execution Phase**: During the “execution” phase, the JavaScript engine runs through the code line by line, this time assigning values to the variables and executing the functions.
    

The concept of hoisting, which I mentioned in the previous message, happens during the compilation phase. But the actual assignment of values happens during the execution phase, which is why you get a `ReferenceError` if you try to use a variable before it’s been declared, or `undefined` if it’s been declared but not yet initialized.

So, while JavaScript uses an interpreter for executing code, the behavior of variables and functions is determined during the compilation phase, which is why understanding this aspect of JavaScript’s execution model is important for avoiding common pitfalls and writing effective code.

## DOM - document object model
#### description of DOM - document object model
- how you use JavaScript to modify a website
- **document**: the html is a document we are working on
- **object**: the html orders are transformed into object in js (?)
- **model**: a representation
	- real thing: `<h2 id="count-el">0</h2>`
	- model: `document.getElementById("count-el").innerText = count`

## the difference between innerText vs textContent
- source: https://www.geeksforgeeks.org/difference-between-textcontent-and-innertext/
#### description
- [graph](https://i.imgur.com/2apgSs3.png)
## javascript random number
#### description
```javascript
firstCard = Math.floor(Math.random() * 10) + 2;
secondCard = Math.floor(Math.random() * 10) + 2;
console.log(firstCard, secondCard)
```
- `Math.random()` js function, generate random float numbers `[0,1)` 
- `Math.random() * 10` multiplies random number by 10, result in random float `[0,10)`
- `Math.floor()` function rounds down input to nearest whole number -> `Math.floor(Math.random() * 10)` generate random whole number btw 0 and 9

## javascript object
- a pair of key-value just like python
- preferred when having to store a lot of complex types data
```javascript
let player = {
name: "DePauw",
chips: 145,
sing: function(){ // a method
	console.log("mot con vit xoe ra 2 cai canh")
	} 
}

playerEl.textContent = player.name + ": $" + player.chips + player.sing()
```



## create input element
- `<input type="text" id="input-el">`
- self closing tag
## const vs let
- If possible, use const. If not, use let.

## add HTML into js code
1) innerHTML
	- `ulEl.innerHTML += "<li>" + myHitList[i] + "</li>"`
2) createElement() then append()
```js
for (let i = 0; i < myLeads.length; i++) {
    ulEl.innerHTML += "<li>" + myLeads[i] + "</li>"
    // create element
    // set text content
    // append to ul
    const li = document.createElement("li") // for every element in myLeads, append a "li" to it
    li.textContent = myLeads[i]
    ulEl.append(li)
}
```
- NOTE: DOM manipulation comes with a cost -> should not let in renders in a for loop
```js
for (let i=0; i<myHitList.length; i++) {
	ulEl.innerHTML += "<li>" + myHitList[i] + "</li>"
}
```

## clear input field on focus
`<input type="text" onfocus="this.value=''" value="Blabla">`

## open in a new tab & click to open a link with `<a>` tag
- open link in new tab: use `target='_blank'`
`<a target='_blank' href='" + myHitList[i] + "'>" + myHitList[i] + "</a>"`

## template string/literals
- use 
```js
this quote `` and have
from this
  
listItems+= "<li><a target='_blank' href='" + myHitList[i] + "'>" + myHitList[i] + "</a>" + "</li>"

to this

listItems+= `
	<li>
		<a target='_blank' href='${myHitList[i]}'>
			${myHitList[i]}
		</a>
	</li>`
```
- benefit
	- break into multiple lines (will also reflected when console.log)
	- just like writing html, if wanted to add js, use `${the-js-piece}`

## json - javascript object notation
- configure app
- provide meta data to it
- #toProceed 

## localStorage
- only support Strings
- setItem: `localStorage.setItem("myHitList", "www.example.com")`
- store array in localStorage:
```js
var names = [];
names[0] = prompt("New member name?");
localStorage.setItem("names", JSON.stringify(names));
// JSON.stringify() to stringify a data type
//...
var storedNames = JSON.parse(localStorage.getItem("names")); // JSON.parse() to convert string to array
```
- use direct access (preferred, as less words :D)
```javascript
localStorage.names = JSON.stringify(names);
var storedNames = JSON.parse(localStorage.names);
```

## Truthy and falsy values
- 