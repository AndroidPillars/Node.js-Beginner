# Node.js

Node.js is a platform it allows you to run a JavaScript code in a computer.

Before Node the JavaScript Code that only run on through browser,

window.alert("Hello World")
<br>
console.log("Hello World")

# Features

- Using JavaScript.
- Extremly Fast.
- Utilize Google's V8 engine writeen in C++.
- V8 compiles JavaScript code in to machine code for computer.
- Build Web, Mobile and Desktop Apps.

# Installation

- https://nodejs.org/en/
- Download the Recommended Version.
- In cmd prompt -> check -> node -v -> To check the current version.
- Eg: In cmd prompt -> check -> node -> print -> console.log("Hello World")

# JavaScript in Browser Environment:

 In the Browser Environment window object is the top level wrapper object and the document object inside window object.
 
- In Browser -> Inspect -> console -> window -> displays windows properties
- window.open("www.AndroidPillars.com")
- window.document -> indicates the current screen of browser.
- document.querySelector("body").style.backgroundColor="red"; -> changes the background color of the screen.

# JavaScript in Node.js Environment:

- Similarly like window object in Node we are having global.
- In cmd prompt -> check -> node -> print -> global -> which lists the properties
- for Exit -> process.exit();

# Getting started with Node.Js:

- Install -> Visual Studio Code -> Create Folder in drive -> Open that Folder through Visual Studio Code.
- Create app.js -> print -> console.log("Hello World"); 
- Go to the App folder -> Enter cmd at the top bar -> In cmd prompt -> node app.js
- O/P -> Hello World

# Functions:

- In JavaScript, Functions are first class objects. which means they can be,
<br> - Stored in a variable, object, or array.
<br> - Passed as an argument to a function.
<br> - Returned from a function.

- In JavaScript we use var/let/const for creating variables.

Syntax:

function sum(a,b){
return a+b;
}

const total = sum(4,5);
console.log("Total: ", total);

O/P -> Total: 9











