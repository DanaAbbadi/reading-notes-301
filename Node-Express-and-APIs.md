# Introduction to node.js

![node.js](https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcQ5v8DCAvmnAJaw9y2Afv81Gw9ZMW3m4XcVDA&usqp=CAU)

Node.js is an open-source, cross-platform runtime environment used for the development of server-side web applications. Node.js applications are written in JavaScript and can be run on a wide variety of operating systems.
Node.js is based on an event-driven architecture and a non-blocking Input/Output API that is designed to optimize an application's throughput and scalability for real-time web applications.

###### From a web server development perspective Node has a number of benefits:

   * Great performance! Node was designed to optimize throughput and scalability in web applications.

   * Another of Node’s big pluses is that it speaks JSON. JSON is ideally suited for consumption by a JavaScript program, meaning that when you’re working with Node, data can flow neatly between layers without the need for reformatting.
    
   * Code is written in "plain old JavaScript", which means that less time is spent dealing with "context shift"   between languages when you're writing both client-side and server-side code.
   
   * The node package manager (NPM) provides access to hundreds of thousands of reusable packages. It also has best-in-class dependency resolution and can also be used to automate most of the build toolchain.
   
   * Node.js is portable. It is available on Microsoft Windows, macOS, Linux, Solaris, FreeBSD, OpenBSD, WebOS,   and NonStop OS. Furthermore, it is well-supported by many web hosting providers, that often provide specific  infrastructure and documentation for hosting Node sites.
   
   * It has a very active third party ecosystem and developer community, with lots of people who are willing to help.

### The Node.js Execution Model

Web applications were written in a client/server model where the client would demand resources from the server and the server would respond with the resources. The server only responded when the client requested and would close the connection after each response.

In very simplistic terms, Imagine visiting Facebook and you were told to wait for 5 minutes, for thousands of people requesting before you!

There has to be a way to run thousands or at least hundred of requests at once, this is what we call ***Threads***. Threads are a way for systems to run multiple operations concurrently. So every request would open a new thread, every thread had all it required to run the same code to completion, think of it as resturant (the server), each customer(requests on server) will have a waiter(thread).


But this system has a downside. It would get to a point where there’s a lot of requests and starting up new threads would consume a whole lot of memory and system resources. Here’s where ***NodeJs*** comes in. In Node, while the file system is reading the file, Node uses the idle time to handle other requests. When the file system is done, it’s smart enough to tell Node to come take the resource and send to the browser. This is possible because of Node’s event loop.

![node event loop](/img/node.PNG)

The event loop is basically a program that waits for events and dispatches them when they happens. One other important fact you might know is that JavaScript is single thread and so is Node. Unlike other languages that require a new thread or process for every single request, NodeJs takes all requests and then delegates most of the work to other system workers. When the background workers are done doing their work, they emit events to NodeJs callbacks registered on that event.




### Node Package Manager npm

npm is a tool you install on your computer. It’s part of node, so install the LTS version of Node to get both the node and npm commands in your command line. You use npm from the command line to install, uninstall or update packages. 

To use npm packages in a project, your project must contain a file called package.json. This file keeps a list of all the packages you are using, and which version of each one you have chosen to use, you can create one from the command line by running  ``` npm init ```  inside your project.

When you open a project for the first time, you have to install all your packages, run this command ``` npm install ``` . After running ```npm install``` there will be a new folder in your project called node_modules. This folder contains all the code for all the packages you have installed. It also contains all that packages that your packages installed. It can get pretty big.

### Introducing Express

Express is the most popular Node web framework, and is the underlying library for a number of other popular Node web frameworks. It provides mechanisms to:

   1. Write handlers for requests with different HTTP verbs at different URL paths (routes).

   2. Integrate with "view" rendering engines in order to generate responses by inserting data into templates.

   3. Set common web application settings like the port to use for connecting, and the location of templates that are used for rendering the response.

   4. Add additional request processing "middleware" at any point within the request handling pipeline.

### “Hello, World!” the Node.js Way

It is agreed by now that writing web apps with Node involves writing event handlers that get called when certain Node events occur. 

1. Create a new folder, cd into the folder with your terminal or command prompt.

2. Do an npm init, hit enter till you successfully create a package.json file in the root of the folder.

3. Create a server.js file in the root folder, copy and paste the code below.

    ``` 
       const express = require('express);

       // initilize the server
       const server = express();


       // create a PORT number
       const PORT = process.env.PORT || 3000;const 

       server.get('/test',(request,response) => {
           response.send('Hello, World!');
       });

       server.listen(PORT,()=>{
           console.log('Listening on port',PORT);
       });

    ``` 
    
4. In the command prompt, type in ```npm start``` and hit enter.

Now, open your browser and hit *localhost:3000/test*. You should see a Hello world message.

On the first line, we required the express module. The module provides as interface to deal with express operations, express is a NodeJs framework for easily building web apps and APIs..

Secondly, we attach an event handler for requests on the server object. The on method takes a second argument which is a callback. The callback takes two objects as arguments. The requestand responseobjects which have information about incoming request and outgoing responses.
    
  

#### Resources:

1. [What Is Node and When Should I Use It?](https://www.sitepoint.com/an-introduction-to-node-js/)
2. [NodeJs introduction](https://codeburst.io/the-only-nodejs-introduction-youll-ever-need-d969a47ef219)
3. [What the heck is npm?](https://medium.com/@tanya/what-the-heck-is-npm-b8168f61e3b5)
4. [Express/Node introduction](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Express_Nodejs/Introduction)