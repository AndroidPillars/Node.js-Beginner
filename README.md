# Node.js

- Node.js is a platform it allows you to run a JavaScript code in a computer.
- Before Node the JavaScript Code that only run on through browser,  
  &nbsp;  
  ```ruby
  window.alert("Hello World")
  ```
  ```ruby
  console.log("Hello World")
  ```

# Features

- Using JavaScript.
- Extremly Fast.
- Utilize Google's V8 engine written in C++.
- V8 compiles JavaScript code in to machine code for computer.
- Build Web, Mobile and Desktop Apps.
- We are using npm(i.e)Node Package Manager which is the world's largest library for open sources packages.
- Great for building Real Time Applications.

# Installation

- Visit, https://nodejs.org/en/
- Download the Recommended Version.
- To check the current version  
  &nbsp;  
  ```ruby
  node -v
  ```
- <b>Example</b>,  
  &nbsp;  
  ```ruby
  node
  ```
  ```ruby
  console.log("Hello World")
  ```

# JavaScript in Browser Environment

 - In the Browser Environment window object is the top level wrapper object and the document object will come inside window   object.
- In Browser -> Inspect -> console  
  &nbsp;  
  ```ruby
  window
  ```
    - where, window displays windows properties  
    &nbsp;  
  ```ruby
  window.open("www.AndroidPillars.com")
  ```
  ```ruby
  window.document
  ```
   - window.document indicates the current screen of browser.  
   &nbsp;  
    ```ruby
    document.querySelector("body").style.backgroundColor = "red";
    ```
   - It changes the background color of the screen.

# JavaScript in Node.js Environment

- Similarly like <b>window</b> object in Node we are having <b>global</b> and process for document.  
 &nbsp;  
  ```ruby
  node
  ```
  ```ruby
  global
  ```
  - Which lists the properties
- for <b>Exit</b>,  
  &nbsp;  
  ```ruby
  process.exit();
  ```

# Getting started with Node.Js

- Install -> Visual Studio Code -> Create Folder in required drive -> Open that Folder through Visual Studio Code.
- Create app.js -> print  
  &nbsp;  
  ```ruby
  console.log("Hello World"); 
  ```
- Go to the App folder -> Enter cmd at the top bar -> In cmd prompt -> node app.js
- O/P -> Hello World

# Functions

- In JavaScript, Functions are first class objects. which means they can be,
  -  Stored in a variable, object, or array.
  - Passed as an argument to a function.
  - Returned from a function.
- In JavaScript we use var/let/const for creating variables.  
 &nbsp;  
  ```ruby

  function sum(a,b){
  return a+b;
  }

  const total = sum(4,5);
  console.log("Total: ", total);

  ```
  - To Run in Terminal,  
  &nbsp;  
    ```ruby
    node app.js
    ```
  - O/P -> Total: 9

# Import/Export:

- Seperate the file which we are using as common.
- Create helper.js -> which Export and Import that in -> app.js
- Syntax -> console.log("Process: ", process);
- If we run -> find a object -> Module -> exports -> which is currently empty.
- require -> which is used to load own module or core node js modules as well as third party modules. 

Syntax:

helpers.js:

function sum(a,b){
return a+b;
}

module.exports = {
sum
};

console.log("Process: ", process);

app.js:

const helpers = require("./helpers");

const total = helpers.sum(4,5);

console.log("Total: ", total);

# Arrow Function:

- Compare to Normal functions, Arrow functions don't have their context(i.e)this keyword.

helpers.js:

function sum(a,b){
return a+b;
}

as,

const sum = (a,b) => {
return a+b;
}

or

const sum = (a,b) => a+b;

or

exports.sum = (a,b) => a+b;

# Object Destructuring:

app.js:

const helpers = require("./helpers");

const total = helpers.sum(4,5);

console.log("Total: ", total);

as,

const { sum } = require("./helpers");

const total = sum(4,5);

console.log("Total: ", total);

# Node Js Core Modules:

const { sum } = require("./helpers");

const http = require("http"); //Load from core node module

const server = http.createServer((req,res) => {
 res.end("Hello World");
 });
 
 sever.listen(3000);

const total = sum(4,5);

console.log("Total: ", total);

- Run the cmd prompt O/P
- Now in Browser -> http://localhost:3000/ -> We created the Server using http module.





















