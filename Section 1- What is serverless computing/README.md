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
