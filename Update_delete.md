# Sending FORM data


An HTML form on a web page is nothing more than a convenient user-friendly way to configure an HTTP request to send data to a server. This enables the user to provide information to be delivered in the HTTP request.


The form contents are expressed as a property list of attribute names and values. Radio buttons and checkboxes are left out of the list when unchecked. This ensures that only the selected radio button contributes a name=value pair. Omitting the VALUE attribute for a checkbox field causes the field when checked to appear as a name without a value (this is appropriate for Boolean attributes). 


The < form> element defines how the data will be sent. All of its attributes are designed to let you configure the request to be sent when a user hits a submit button. The two most important attributes are action and method.

## Action Attribute

The action attribute defines where the data gets sent. Its value must be a valid relative or absolute URL.

## Method Attribute

The method attribute Tells the browser how to send form data to a web server. Here are the values for the method:

 #### < form method=”GET”>

The method attribute of the form element tells the web browser how to send form data to a server. Specifying value of GET means the browser will add the form contents to the end of the URL. This offers a number oadvantages for simple forms. It allows the browser to cache the results of the form submission, and it alsallows the user to bookmark the page once the form has been submitted. As such, GET is generally used fosimple forms where security is not a concern

GET results in the entire contents of the submission being visible in the URL. If your form contains sensitivdata, you should specify a value of POST for the method attribute. Since GET appends the form data to thcurrent URL, it can only be used where the contents of the submission (including the complete URL) will resulin a string that is 2048 characters long, or less. This is the maximum length of a URL. GET can only be useto send ASCII data.

#### < form method=”POST”>

The method attribute of the form element tells the web browser how to send form data to a server. Specifying a value of POST means the browser will send the data to the web server to be processed. This is necessary when adding data to a database, or when submitting sensitive information, such as passwords

![get](/img/get.PNG)

## On the server side: retrieving the data

The web uses a client/server architecture that can be summarized as follows. a client, like a web browser, sends a request to a server like Apache or Nginx, using the HTTP protocol. The server answers the request using the same protocol.

Whichever HTTP method you choose, the server receives a string that will be parsed in order to get the data as a list of key/value pairs. The way you access this list depends on the development platform you use and on any specific frameworks you may be using with it



     

