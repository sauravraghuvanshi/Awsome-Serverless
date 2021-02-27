# In this section of the repository will talk about fundamental of Serverless Computing.

## Agenda of this section:-
* What is Serverless Computing?
* How does it work?
* What are building blockes of Serverless Computing?
* How does Serverless Computing differ from traditional computing?
* What are common use cases for serverless computing?
* How to get started?

### What is Serverless Computing:-
* It comes when AWS releases service know as Lambda.
* Lambda runs your code for you.
* We rent the infrastructure to run the code.
* **There are still servers, but these resurces are managed by cloud provider.**
* It is also know as **Function as a Service(FaaS).**
* We only pay for the time our function runs.
* We can expect the service to be highly reliable and highly available.
* We don't manage or own the infrastructure.
* You still need to manage some aspects of serverless function.

### How Does Serverless Computing work?
* It create a container environment to execute our code
* No guarentee your function will run in the same container
* Lambda function are each allocated a  512MB/ tmp directory
* You can check to see if that is available when invoking a new function
* Don't make your code ststem dependent as each time lambda may create a complete different container
* Runtime Language: Node.js, java, python, .Net Core

### How do we Trigger a Lambda function?
* Lambda use invoke function for trigger
* **There are three type of Invocation:-**
  * Request Response(Default)
  * Event
  * Dry Run
* RequestResponse = synchronous = run in real time
* Event: It can be puch or pull based and has 2 mode synchronous and asynchronous
* For puch we have to define method to be synchronous or asynchronous. FOr pull it is defined by AWS Services
* Dry Run: It is just to check things work or not but it will not have a run environment
* There is also HTTPS request which use to invoke Lambda function by sending data in the request body as a parameter to that Lambda function

### What is Rest API?
* **REST =** Representational State Transfer
* Allows a requesting system to access and manipulate textual representaion of web resources using a uniform and predefined set of stateless operations 

### What are building blocks of Function-as-a-Service(FaaS):-
1. The first building block is **RESTful API**. REST is based on HTTP(Hyper Text Transfer Protocal). HTTP is use to  exchange 
 