# JavaScript

JavaScript is a high-level, interpreted programming language used to create interactive and dynamic web pages. It works alongside HTML and CSS to build modern web applications.

---

## Prerequisites

- Basic knowledge of HTML and CSS
- Code Editor (VS Code)
- Modern Web Browser (Chrome, Firefox, Edge)
- Node.js (Optional)

---

## Project Structure

```
javascript/
│
├── index.html
├── style.css
├── script.js
└── README.md
```

---

## How to Run

### Method 1: Live Server (Recommended)

1. Open the project in VS Code.
2. Install the **Live Server** extension.
3. Right-click `index.html`.
4. Select **Open with Live Server**.

### Method 2: Open in Browser

Double-click `index.html` to open it in a browser.

> Note: Some JavaScript features (such as `fetch()` and ES Modules) require a local server.

---

# JavaScript Basics

## Variables

```javascript
let name = "Praveen";
const age = 25;
var city = "Chennai";
```

---

## Data Types

```javascript
let username = "John";   // String
let age = 20;            // Number
let isStudent = true;    // Boolean
let marks = null;        // Null
let address;             // Undefined
```

---

## Operators

### Arithmetic

```javascript
let sum = 10 + 5;
let sub = 10 - 5;
let mul = 10 * 5;
let div = 10 / 5;
let mod = 10 % 3;
```

### Comparison

```javascript
10 == "10"
10 === "10"
10 != 20
10 > 5
10 < 20
```

### Logical

```javascript
&&
||
!
```

---

## Conditional Statements

### if

```javascript
let age = 18;

if (age >= 18) {
    console.log("Eligible");
}
```

### if...else

```javascript
if (age >= 18) {
    console.log("Adult");
} else {
    console.log("Minor");
}
```

### switch

```javascript
let day = 2;

switch(day){
    case 1:
        console.log("Monday");
        break;
    case 2:
        console.log("Tuesday");
        break;
    default:
        console.log("Invalid");
}
```

---

## Loops

### for

```javascript
for(let i=1;i<=5;i++){
    console.log(i);
}
```

### while

```javascript
let i=1;

while(i<=5){
    console.log(i);
    i++;
}
```

### do...while

```javascript
let i=1;

do{
    console.log(i);
    i++;
}while(i<=5);
```

---

## Functions

```javascript
function greet(name){
    return "Hello " + name;
}

console.log(greet("Praveen"));
```

### Arrow Function

```javascript
const add = (a,b) => a+b;

console.log(add(5,10));
```

---

## Arrays

```javascript
const fruits = ["Apple","Orange","Mango"];

console.log(fruits[0]);

fruits.push("Banana");
fruits.pop();
```

---

## Objects

```javascript
const student = {
    name:"Praveen",
    age:25,
    city:"Chennai"
};

console.log(student.name);
```

---

## DOM Manipulation

### Select Elements

```javascript
document.getElementById("title");
document.querySelector(".box");
document.querySelectorAll("p");
```

### Change Content

```javascript
document.getElementById("title").textContent = "Hello";
```

### Change Style

```javascript
document.getElementById("title").style.color = "red";
```

### Event Listener

```javascript
const btn = document.getElementById("btn");

btn.addEventListener("click", function(){
    alert("Button Clicked");
});
```

---

## ES6 Features

### Template Literals

```javascript
let name = "Praveen";

console.log(`Hello ${name}`);
```

### Destructuring

```javascript
const person = {
    name:"John",
    age:20
};

const {name,age} = person;
```

### Spread Operator

```javascript
const arr1 = [1,2,3];
const arr2 = [...arr1,4,5];
```

### Rest Operator

```javascript
function total(...numbers){
    console.log(numbers);
}
```

---

## Promises

```javascript
const promise = new Promise((resolve,reject)=>{

    let success = true;

    if(success){
        resolve("Success");
    }else{
        reject("Failed");
    }

});

promise
.then(result=>console.log(result))
.catch(error=>console.log(error));
```

---

## Async / Await

```javascript
async function getData(){

    try{
        const response = await fetch("https://jsonplaceholder.typicode.com/users");
        const data = await response.json();

        console.log(data);
    }
    catch(error){
        console.log(error);
    }

}

getData();
```

---

## Local Storage

```javascript
localStorage.setItem("name","Praveen");

const name = localStorage.getItem("name");

localStorage.removeItem("name");

localStorage.clear();
```

---

## Common Array Methods

```javascript
map()
filter()
find()
reduce()
forEach()
some()
every()
sort()
```

---

## String Methods

```javascript
length
toUpperCase()
toLowerCase()
trim()
includes()
replace()
slice()
split()
```

---

## Math Methods

```javascript
Math.random()
Math.floor()
Math.ceil()
Math.round()
Math.max()
Math.min()
```

---

## Date

```javascript
const today = new Date();

console.log(today);
```

---

## Console Methods

```javascript
console.log()

console.error()

console.warn()

console.table()

console.time()

console.timeEnd()
```

---

## Best Practices

- Use `let` and `const` instead of `var`.
- Write meaningful variable names.
- Keep functions small and reusable.
- Use strict equality (`===`).
- Handle errors with `try...catch`.
- Comment complex logic when necessary.
- Format your code consistently.

---

## Resources

- MDN Web Docs
- JavaScript.info
- W3Schools
- freeCodeCamp

---

## License

This project is open source and available for learning purposes.