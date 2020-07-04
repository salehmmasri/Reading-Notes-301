# Node, Express, and APIs 

---

### What Is Node and When Should I Use It? 
#### What Is Node.js? Node.js is an

- event-based
- non-blocking
- asynchronous I/O runtime
- uses Google’s V8 JavaScript engine and libuv library.

#### Node Is Built on Google Chrome’s V8 JavaScript Engine

- The V8 engine is the open-source JavaScript engine
    - runs in Google Chrome and other Chromium-based web browsers.
    - responsible for compiling JavaScript directly to native machine code that your computer can execute.
*Node is built on the V8 engine ⚙️ dosen't mean that Node programs are executed in a browser They aren’t.*

- V8 engine enhanced with various features, such as :

    - a file system API
    - an HTTP library
    - a number of operating system–related utility methods.
- Node.js is a program we can use to execute JavaScript on our computers it’s a JavaScript runtime.

- npm package manager that comes bundled(To tie or wrap together.) with Node.

- use a version manager => This is a program that allows you to install multiple versions of Node and switch between them at will. advantages to using a version manager:

    1. it negates potential permission issues when using Node with npm.
    1.2 lets you set a Node version on a per-project basis.
- check that Node is installed on your `system => node -v`

*Node.js Has Excellent Support for Modern JavaScript Node has excellent support for ECMAScript 2015 (ES6) and beyond.*
- this means that you can write your JavaScript using the latest and most modern syntax. 🎸
- It also means that you don’t generally have to worry about compatibility issues, as you would if you were writing JavaScript that would run in different browsers. 

---

### What Are the Advantages of Node.js? 🔆
- speed and scalability
- it speaks JSON.
- ubiquitous
- Other Uses of Node 🏁 And it doesn’t stop at the server. There are many other exciting and varied uses of Node.js! For example:

    it can be used as a scripting language to automate repetitive or error prone tasks on your PC.
    It can also be used to write your own command line tool, such as this** Yeoman-Style generator** to scaffold out new projects.
    Node.js can also can be used to build cross-platform desktop apps and even to create your own robots
    
    ---

### npm 
#### Introducing npm, the JavaScript Package Manager 📁 check which version you have installed on your system, type npm -v.

1. the package manager for JavaScript
1. the world’s largest software registry

#### how we would use npm to install a package.

- Installing a Package Globally npm install -g jshint
    - This will install the jshint package globally on your system. We can use it to lint the index.js file
    
- Installing a Package Locally npm init -y

    - This will create and auto-populate a package.json file in the same folder.
    - install the lodash package and save it as a project dependency npm install lodash --save
- Working with the package.json File

    - node_modules folder => This is where npm has saved lodash and any libraries that lodash depends on.