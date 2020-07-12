# EJS

![ejS](/img/ej6.PNG)

EJS simply stands for Embedded JavaScript templates, and we can use it both server-side or client-side.

#### Features of EJS :

  * Fast compilation and rendering
  * Simple template tags: <% %>
  * Both server JS and browser support
  * Static caching of intermediate JavaScript
  * Static caching of templates
  * Complies with the Express view system

#### Basic Syntax(Tags):
  * <% 'Scriptlet' tag, for control-flow, no output
  * <%= Outputs the value into the template (HTML escaped)
  * <%- Outputs the unescaped value into the template


- To install EJS with NPM write this in your terminal : npm install ejs

- Caching : EJS ships with a basic in-process cache for caching the intermediate JavaScript functions used to render templates.

- Layouts : EJS does not specifically support blocks, but layouts can be implemented by including headers and footers.


##### We can use EJS to Template our Node Application

For applications that need quick templating, there are many options that we can use :

  * Jade : comes as the view engine for Express by default
  * EJS : is one alternative does that job well and is very easy to set up


