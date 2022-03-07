# The REST Architecture 
---
REST stands for Representational State Transfer, a term coined by Roy Fielding in 2000. It is an architecture style for designing loosely coupled applications over HTTP, that is often used in the development of web services.

REST is designed for especially working with components such as files, objects, media components on a particular hardware device. Web service defined on principles of REST and can be defined as a RESTful web service. RESTful web service can use normal POST, DELETE, PUT, and HTTP verbs of GET for working with required components. 

## Why REST?
- Due to scalability, the protocol stands out when compared to other API’s. The reason due to the server and client separation. 
- Because of its flexibility and portability. With REST essential data covered in one request not ending at this but also easier to shift the data from one server to another one. It gives access to modifications on - the database at any time. 
- The separation of server and client made it easy for the protocol to work on various development projects independently. It is adaptable to various working syntax and platforms and brings opportunities to work on various projects.

## Architectural Constraints
Here are 6 REST constraints that we can consider as design rules, that must be applied to establish the distinct characteristics of the REST architectural style. In other words, These 6 architectural constraints which make any web service — a true RESTful API:

- **Interface / Uniform Contract:** 
As the constraint name itself applies, we must decide APIs interface for resources inside the system which are exposed to API consumers and follow religiously. A resource in the system should have only one logical URI, and that should provide a way to fetch related or additional data. It’s always better to synonymize a resource with a web page.</br>
All resources should be accessible through a common approach such as HTTP GET and similarly modified using a consistent approach.
  >Once a developer becomes familiar with one of the API, he should be able to follow the similar approach for other APIs.


- **Client-Server:** This constraint essentially means that client applications and server applications must be able to evolve separately without any dependency on each other. A client should know only resource URIs, and that’s all. Today, this is standard practice in web development, so nothing fancy is required from our side. need to keep it simple.
    >Servers and clients may also be replaced and developed independently, as long as the interface between them is not altered.
- **Stateless:** Roy fielding got inspiration from HTTP, so it reflects in this constraint. Make all client-server interactions stateless. The server will not store anything about the latest HTTP request the client made. It will treat every request as new. No session, no history.
    >No client context shall be stored on the server between requests. The client is responsible for managing the state of the application.
- **Cache:** The webpage now we are reading here is also a cached version of the HTML page. Caching brings performance improvement for the client-side and better scope for scalability for a server because the load has been reduced.

    In REST, caching shall be applied to resources when applicable, and then these resources MUST declare themselves cacheable. Caching can be implemented on the server or client-side.
    >Well-managed caching partially or completely eliminates some client-server interactions, further improving scalability and performance.
- **Layered System:** REST allows us to use a layered system architecture where we deploy the APIs on server A, and store data on server B and authenticate requests in Server C, for example. A client cannot ordinarily tell whether it is connected directly to the end server or an intermediary along the way.
- **Code-On-Demand (optional):** Well, this constraint is optional. Most of the time, we will be sending the static representations of resources in the form of XML or JSON. But when we need to, we are free to return executable code to support a part of out application, e.g., clients may call out API to get a UI widget rendering code. It is permitted.


## Benefits of using REST Architecture


- **RESTful as lightweight Web Services:** The RESTful architecture was a reaction to the more heavy-weight SOAP-based standards. In REST web services, the emphasis is on simple point-to-point communication over HTTP using plain XML. In addition, RESTful permits many different data formats whereas SOAP only permits XML.
- **The simplicity of RESTful:** The RESTful architecture is much simpler to develop than SOAP. One of the main reasons for REST popularity is the simplicity and ease of use, as it does an extension of native Web technologies such as HTTP.
- **RESTful architecture is closer in design to the Web:** RESTful is the architectural style of the web itself, so the developer with knowledge in web architecture will naturally develop in the RESTful architecture.
- **Scalability:** As RESTful forbids conversational state, which means we can scale very wide by adding additional server nodes behind a load balancer.
- **Expose APIs as HTTP Services:** When developers need the universal presence with minimum efforts, given the fact that RESTful APIs are exposed as HTTP Services, which is virtually present on almost all the platforms.
## Conclusion
REST is an architectural pattern which is based on HTTP and uses HTTP requests, responses, verbs and status codes to communicate.
With the help of REST, API complications reduce to zero, and things are easier with fewer resources in context. It can manage resources with ease and with few operations.
The fact that REST services use HTTP means they can be consumed by almost any ‘online’ device or application (including IoT devices such as toasters, cars, pedometers etc) no proprietary knowledge of the API is required.

REST is a cool phenomena of Web Technologies and it always exciting to develop light-weight and robust systems that are built on top of REST Architecture to interact using Web.

## References
https://www.ics.uci.edu/~fielding/pubs/dissertation/rest_arch_style.htm

https://restfulapi.net/

https://krify.co/advantages-and-disadvantages-of-rest-api/