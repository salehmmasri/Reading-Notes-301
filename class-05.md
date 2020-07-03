# Heroku Deployment 😎

---

# Defining an application
- Heroku lets you deploy, run and manage applications written in Ruby, Node.js, Java, Python, Clojure, Scala, Go and PHP.
- Dependency mechanisms vary across languages: in Ruby you use a Gemfile, in Python a requirements.txt, in Node.js a package.json, in Java a pom.xml and so on.

### Knowing what to execute
- One requirement is informing the platform as to .

- Heroku is a polyglot[speaking, many languages.] platform it lets you:
    - build
    - run
    - scale applications in a similar manner across all the languages
    - utilizing the dependencies and Procfile.
        - The Procfile exposes an architectural aspect of your application
# Deploying applications 👽
- The Heroku platform uses Git as the primary means for deploying applications (there are other ways to transport your source code to Heroku, including via an API).
- When you create an application on Heroku, it associates a new Git remote, typically named heroku, with the local Git repository for your application. $ git push heroku master
## Build
### Running applications on dynos
- Heroku executes applications by running a command you specified in the Procfile, on a dyno that’s been preloaded with your prepared slug (in fact, with your release, which extends your slug and a few items not yet defined: config vars and add-ons).

`$ heroku ps:scale web=3 queue=2`

## Node.js For Beginners.
#### Deploy Your Blog to Heroku
##### How can I?
1. We will use Node.js for our project.
- is an open source
- cross-platform runtime environment
- allows you to build server-side
- networking applications.
11. Pretty simple, but it's a server!
- First of all, we need to create a JavaScript file. Let's name it server.js:


`http.createServer( function( request, response) {
response.writeHead( 200, {"Content-Type": "text/plain"} );
response.write( "It's alive!" );
response.end();
}).listen(3000);`
- make sure it's working. Run at your terminal: node server.js

    Let's look more closely at our first Node server. This is an example of how Node provides you with non-blocking and event-driven behavior. Let me explain:

`$.post('/some_requested_resource', function(data) { console.log(data);});`

- This code performs a request for some resource
    When the response comes back, an anonymous function is called. It contains the argument data, which is the data received from that request.
- Node allows you to use the so-called event loop, which works faster because of non-blocking behavior.
- Make it worldwide 🌏
- Use Heroku cloud application platform for this

- First step after Heroku installation is to log in to the system from your computer:

- heroku login.

- Create your project directory. And then create the server.js file inside of it.

- First of all, let's declare some variables:

- var http = require("http"); will give the key to Node's HTTP functionality
- var fs = require("fs"); for possibility to interact with the file system
    var path = require("path"); allows you to handle file paths
    var mime = require("mime"); allows you to determine a file's MIME-type it's not a part of Node.js`
    so we need to install third-party dependencies before using it. We need to create the package.json file for that purpose. It will contain project related information:

- name
    version
    description, and so on.
    For our project we will use MIME-types recognition, because it's not enough to just send the contents of a file when you use HTTP. You also need to set the Content-Type header with proper MIME-type. That's why we need this plug-in.