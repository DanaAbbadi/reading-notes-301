# What Google Learned From Its Quest to Build the Perfect Team

Project Aristotle’s researchers began by reviewing a half-century of academic studies looking at how teams worked. Were the best teams made up of people with similar interests? Or did it matter more whether everyone was motivated by the same kinds of rewards? Based on those studies, the researchers scrutinized the composition of groups inside Google: How often did teammates socialize outside the office? Did they have the same hobbies? Were their educational backgrounds similar? Was it better for all teammates to be outgoing or for all of them to be shy? They drew diagrams showing which teams had overlapping memberships and which groups had exceeded their departments’ goals. They studied how long teams stuck together and if gender balance seemed to have an impact on a team’s success.

### Which group would you rather join?

As the researchers studied the groups, however, they noticed two behaviors that all the good teams generally shared. First, on the good teams, members spoke in roughly the same proportion, a phenomenon the researchers referred to as ‘‘equality in distribution of conversational turn-taking.’’ On some teams, everyone spoke during each task; on others, leadership shifted among teammates from assignment to assignment. But in each case, by the end of the day, everyone had spoken roughly the same amount. ‘‘As long as everyone got a chance to talk, the team did well,’’ Woolley said. ‘‘But if only one person or a small group spoke all the time, the collective intelligence declined.’’



# REST

REST, or REpresentational State Transfer, is an architectural style for providing standards between computer systems on the web, making it easier for systems to communicate with each other. REST-compliant systems, often called RESTful systems, are characterized by how they are stateless and separate the concerns of client and server. 


### Guiding Principles of REST

 1. Client–server – By separating the user interface concerns from the data storage concerns, we improve the  portability of the user interface across multiple platforms and improve scalability by simplifying the server  components.

 2. Stateless – Each request from client to server must contain all of the information necessary to understand the  request, and cannot take advantage of any stored context on the server. Session state is therefore kept entirely on  the client.

 3. Cacheable – Cache constraints require that the data within a response to a request be implicitly or explicitly  labeled as cacheable or non-cacheable. If a response is cacheable, then a client cache is given the right to reuse  that response data for later, equivalent requests.

 4. Uniform interface – By applying the software engineering principle of generality to the component interface, the  overall system architecture is simplified and the visibility of interactions is improved. In order to obtain a  uniform interface, multiple architectural constraints are needed to guide the behavior of components. REST is  defined by four interface constraints: identification of resources; manipulation of resources through  representations; self-descriptive messages; and, hypermedia as the engine of application state.

 5. Layered system – The layered system style allows an architecture to be composed of hierarchical layers by  constraining component behavior such that each component cannot “see” beyond the immediate layer with which they  are interacting.

 6. Code on demand (optional) – REST allows client functionality to be extended by downloading and executing code in  the form of applets or scripts. This simplifies clients by reducing the number of features required to be  pre-implemented.


### Making Requests

  REST requires that a client make a request to the server in order to retrieve or modify data on the server. A   request generally consists of:
  
   1. an HTTP verb, which defines what kind of operation to perform
   2. a header, which allows the client to pass along information about the request
   3. a path to a resource
   4. an optional message body containing data

### HTTP Verbs

  There are 4 basic HTTP verbs we use in requests to interact with resources in a REST system:
  
   1. GET — retrieve a specific resource (by id) or a collection of resources
   2. POST — create a new resource
   3. PUT — update a specific resource (by id)
   4. DELETE — remove a specific resource by id



# SuperAgent

SuperAgent is light-weight progressive ajax API crafted for flexibility, readability, and a low learning curve after being frustrated with many of the existing request APIs.



# Resources

 1. [What Google Learned From Its Quest to Build the Perfect Team](https://www.nytimes.com/2016/02/28/magazine/what-google-learned-from-its-quest-to-build-the-perfect-team.html) 
 2. []A Conversation about REST with my brother(https://gist.github.com/brookr/5977550) 
 3. [What is REST](https://www.codecademy.com/articles/what-is-rest) 
 4. [REST](https://restfulapi.net/) 
 5. [SuperAgent](https://visionmedia.github.io/superagent/)


