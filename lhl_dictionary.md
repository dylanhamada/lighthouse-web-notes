# Lighthouse Labs Dictionary

### Anonymous Function

Anonymous functions are functions without names. They can be used as arguments to other functions or as immediately invoked function executions.

An anonymous function stored in a variable:
```javascript
let show = function() {
  console.log("Anonymous function");
}
```

An anonymous function passed as an argument to a higher-order function:
```javascript
setTimeout(function() {
  console.log("Execute after 1 second.");
}, 1000)
```

### API

An **A**pplication **P**rogramming **I**nterface is a construct that allows developers to create complex functionality more easily. They abstract more complex code away from you, providing some easier syntax to use in its place.

There are APIs for manipulating documents, fetching data from a server, drawing and manipulating graphics, manipulating audio and video, and storing data, to give a few examples.

### Array

An array is a type of object that is used to store data. Arrays consist of an ordered collection or list containing zero or more data types, and use numbered indices starting from 0 to access specific items. We use square brackets - `[]` to create an array.

Eg.
```javascript
let oceans = [
	"Pacific",
	"Atlantic",
	"Indian",
	"Arctic",
	"Antarctic",
];
```

### Arrow Function

An arrow function expression is a compact alternative to a traditional function expression. 

They don't have their own bindings to `this`, `arguments`, or `super`. They should not be used as methods.

Eg. of arrow functions
```javascript
() => expression;

() => {
  statements
};

param => {
  statements
};

(param1, param2) => {
  statements
};
```

### Asynchronous Workflow

Asynchronous workflow is basically a form of parallel programming that allows a unit of work to execute or run separately from the primary application code blocks without blocking other operations. This implies that it is a method of writing code to ensure **simultaneous** code execution.

Asynchronous programming in JavaScript is possible and more efficient when working with technologies like **AJAX** and **Fetch API**, which is used to make HTTP requests to files, services, and browser/server APIs internally or externally. There are some key concepts when working with an asynchronous workflow, like callbacks, promises, and async/await.

### Assertion

Assertions are expressions in programming that evaluate whether certain conditions within the code are as expected. If the result is true, the program **continues** to run. However, if an assertion evaluates to false, it indicates bugs or issues that must be addressed. That way, you can avoid potential pitfalls down the road.

Eg. Assertions using the Chai assertion library
```javascript
const chai = require('chai');  // import the chai library
const assert = chai.expect;  // establish a variable to be used in our tests
const validator = require('../javascript/groupValidator.js'); // import the file where our function lives

describe("The function groupValidator()", () => {
  it("should return true if there are between 2 and 5 group members", () => {
    assert(validator.isGroupValid(["a", "b", "c"])).to.be.true
  });
  it("should return false if there are less than 2 group members", () => {
    assert(validator.isGroupValid(["a"])).to.be.false
  });
  it("should return false if there are more than 5 group members", () => {
    assert(validator.isGroupValid(["a", "b", "c", "d", "e", "f"])).to.be.false
  });
});
```

### AJAX

### Behavior Driven Development (BDD)

Behavior Driven Development covers the entire life cycle of the app development process, from planning the project to writing the code. It encourages you to specify the behavior of your app in terms of user stories which are broken down into scenarios that can be built and tested.

### Box Model

A set of properties that characterize the parts of an element that take up space within the web page. It contains content area sizes for the width and height, content, padding, border, and margins. Width and height are a part of the content area, which is the actual element itself.

### Call Stack

A JavaScript call stack is an example of a stack data structure. In a JS call stack, the elements are function invocations. Every time you invoke a function, it’s added to the stack. If it has a nested function, that nested function will get added to the top of the stack as well, and so on. You can think of the call stack as a to-do list of sorts for JavaScript.

### Callback Queue

The Callback queue is a data structure that operates on the **FIFO** (first-in-first-out) principle. Callback functions that need to be asynchronously executed, are pushed onto the callback queue. These are later pushed to the Call stack to be executed (when the event loop finds an empty call stack).

### Callback Functions

A relationship status between functions. A function passed in as an argument to a higher order function is a callback function. A function given to a higher order function in order to make it work.

### Chai

An assertion library. It gives us assertion functions so that we no longer have to use our `assertEqual` and other assertion functions that we implemented previously. Chai assertion functions are deliberately designed to play nice with testing frameworks like Mocha.

### Class

Classes are blueprints (templates) that we use to create *instances* of objects. A class describes that the object is going to be and we can create new objects using the class. 

Classes can contain a constructor method, as well as other methods and properties.

Eg.
```javascript
class Pizza {

  constructor(size, crust) {
    this.size = size;
    this.crust = crust;
    this.toppings = ["cheese"];
  }

  addTopping(topping) {
    this.toppings.push(topping);
  }
}
```

### Client

In web development, 'client side' refers to everything in a web application that is displayed or takes place on the client (end user device). This includes what the user sees, such as text, images, and the rest of the UI, along with any actions that an application performs within the user's browser.

Markup languages like HTML and CSS are interpreted by the browser on the client side. In addition, many contemporary developers are including client-side processes in their application architecture and moving away from doing everything on the server side; business logic for dynamic webpages*, for instance, usually runs client side in a modern web application. Client-side processes are almost always written in JavaScript.

### Code Golfing

Code golf is a type of recreational computer programming competition in which participants strive to achieve the shortest possible source code that solves a certain problem.

### Credentials

In the context of web development, "credentials" typically refer to the information used to **authenticate** a user or a system. These credentials are often required to access restricted resources or perform certain actions on a website or web application.

The most common types of credentials in web development are:

- Username and Password
- API Keys
- Access Tokens
- Session Tokens or Cookies
- Client Certificates
- Biometric Data

### CRUD

Create, Read, Update, and Delete (CRUD) are the four basic functions that models should be able to do, at most. When we are building APIs, we want our models to provide four basic types of functionality. The model must be able to Create, Read, Update, and Delete resources. Computer scientists often refer to these functions by the acronym CRUD. A model should have the ability to perform at most these four functions in order to be complete. If an action cannot be described by one of these four operations, then it should potentially be a model of its own.

### CSS

CSS stands for Cascading Style Sheets. It’s a stylesheet language used to add **layout** and **visual effects** to HTML elements.

CSS is used specifically for markup languages, in this case HTML. A markup language is used to apply structure to a website or text document. The “markup” in this case is a set of tags used to indicate the structure and format of the page.

The “cascading” part of its name refers to how styles are inherited and applied to different elements on a web page based on their relationship to each other in the HTML document. Styles can be applied to a parent element, which will be passed down to its child elements.

### Database

### Dependency

### DOM

### DRY

### Encryption

Don't Repeat Yourself. The principle states that any piece of knowledge or functionality in a software system should be represented in a single place only – essentially, nothing should be repeated.

### Error Handling

### Express

A framework that builds a web server that is able to host HTML pages for clients to view.

### Expression

An expression is any word of group of words or symbols that is a value. In programming, an expression is a value, or anything that executes and ends up being a value.

Eg. 
```javascript
const price = 500;
```

`const`, `price`, `=`, and `500` are expressions because each of them has a definite and unique meaning.

### Event (DOM)

### Event Loop

### FOCAL

An acronym that describes core concepts of programming:

**F**unctions - **O**bjects - **C**onditionals - **A**rrays - **L**oops

### Fork

A fork is a new repository that shares code and visibility settings with the original "upstream" repository. Forks are often used to iterate on ideas or changes before they are proposed back to the upstream repository, such as in open source projects or when a user does not have write access to the upstream repository.

### Function

### Function Declaration

### Function Expression

### Gist

### Global Execution Context

### Hashing

### Higher Order Functions

Functions that take callbacks as parameters. Any functions which **operate** on other functions. If it's called without being passed a function as an argument, it will crash.

Built-in array functions like `forEach`, `filter`, and others are examples of Higher Order Functions.

### Hoisting

### HTTP

### IP

### JAM Stack

### JQuery

### Library

### Linting

### Loops

### Media Query

### Mocha

A testing framework. Gives us the `describe` and `it` functions. Each `it` is a test, and each test should have at least one *assertion*.

### Module

Every file run by Node has access to a **module** object. Each file that Node runs is actually considered a separate module. Node exports an empty object for each file by default.

A module can be imported using the `require` method. The file extension can be omitted.

```javascript
const sayHelloTo = require('./myModule');
```

A module can be exported by assigning an object to `module.exports`.

```javascript
const sayHelloTo = function(person) {
  console.log(`Hello, ${person}`);
}

module.exports = sayHelloTo;
```

### MVC

### Networking

### Objects

### Operators

### Parameter

### Ports

### Preprocessor

### Promises

### Recursion

A function that calls itself until it doesn't. It will call itself to execute code over and over again, like a loop. Every recursive function **must** stop calling itself at some point, otherwise it's not recursive and will keep being called forever.

The **recursive case** of a recursive function is one that will allow the function to continue calling itself. The **base case** is one that when reached will stop the function from calling itself. In a properly designed recursive function, with each recursive call, the input must gradually resolve toward the base case. A function **must have have at least one recursive case and at least one base case** in order to be recursive.

```javascript
// An example of recursion
// This function counts even numbers from the passed-in number up to 12
function countEvenToTwelve(number) {
  if (number <= 12) {
    console.log(number);
    countEvenToTwelve(number + 2);
  }
}
countEvenToTwelve(0)
```

### Refactor

### Relational Databases

### Return Statement

### Repository

### Responsive Design

### REST

### Routes

### SASS

### Scope

A globally-scoped variable is available everywhere in the code, whereas a locally-scoped variable would only be available within the function in which it's defined.

### Self-documenting Code

### Serialization

The process of serialization converts objects (or data structures) into a format that can be stored or transmitted between computers (typically as a string of text). The opposite, going from string to object, is called deserialization.

### Servers

### Services

### Single-Threaded

### Statement

### String Literal

### Switch Statement

### Syntax

### TCP

### Template Engine

### Test-Driven Development

When writing a feature for implementation, we write the testing code first, with all expected results, ouputs and inputs, etc. We write just a little bit of our feature, just so it can run the tests.

Every test should fail! Now start writing the feature code to start passing each and every test, until all tests pass. Now, the feature is complete!

### Testing

Can be divided into **manual** testing and **automated** testing.

Manual testing involves testing things by hand each time, and becomes tedious and less productive.

Automated testing involves writing code to programmatically test the actual code we want to write. It saves time, makes code more readable and collaborative, and overall improves the quality of code.

Automated testing can be further divided into **unit testing**, **integration testing**, and **functional testing**.

Unit tests apply to small pieces of code, alone and isolated. They essentially give a function that tests some inputs, and checks if what the function outputs is correct. 

Integration tests examine how parts of the system work together. They are similar to unit tests, but while unit tests are isolated from other components, integration tests are not. They are useful because sometimes you need to have tests to verify if multiple systems - like a database and your app - work together correctly.

Functional tests examine the complete functionality of an application. They are high in complexity, so there are usually only a handful compared to unit and integration tests. They effectively should be validated the same way you would validate if you were a user of the app or webpage.

### This

A keyword like `for` or `function`. In JavaScript, the value of `this` is determined at the time of the call and depends on how and where it was called. 

When `this` is used inside a method, it refers to the object that the method was called on. 

Eg.
```javascript
const dog = {
  sound: "woof",
  speak: function() {
    // the value of this refers to the dog object
    console.log(this.sound);
  }
};

dog.speak();
```

### Truthy/Falsy

### Try/Catch

### Type Coercion

### Variable

A variable lets you store a value or a reference of something.

### Version Control

### View Engine

### Web Server

### XML