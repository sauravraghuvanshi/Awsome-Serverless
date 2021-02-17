# What we are going to cover it this module?

### An overview of AWS Lambda:-
* A high level explanation of what the service is and how it works. It also covers some of the component of AWS Lambda itself.

### Lambda Functions:-
- How lambda functions are compiled along with each element of the function itself and the configurable options from within the management console.

- **Event Sources:-**
  * What are event source and event source mapping is and the difference between them.
  * The difference between synchronous and asynchronous invocations invocations

- **Monitoring and Troubleshooting AWS Lambda:-**
  * The options available to you when monitoring your lambda and some of the common problems that arises when running your function and what to check.

## What will you gain after competing this section:-
* Explains what AWS Lambda is and what it is used for.
* Define the components used within Lambda
* Explains the different elements of a lambda function through its creations
* Understand the key difference between policies used within lambda
* Understand how events source and event mapping are managed for both synchronous and asynchronous invocations
* Use Amazon Cloud watch to monitor matrices and logs to issolate issues with your features
* Check for common errors that might be cousing your functions to fails

## An overview of AWS Lambda
* It is a serverless compute service that allow you to run your application code without haveing to manage your EC2 instances
* The responsibility to maintain and administer the EC2 instance is passed over to AWS to manage for you
* You only ever have to pay for for compute power when Lambda is in used  via Lambda functions
* AWS Lambda charges compute power per 100ms of use only when your code is running in addetion to number of times your code runs

### There are four steps involved in AWS Lambda
1. You can either upload your code to lambda, or write within the code editors that lambda provides. It supports **Node.js, Java, C#, Python, Go, Powershell, Ruby**
2. Configure your Lambda functions to execute upon specific triggers from supported event source
3. Once the specific trigger is inittiated. Lambda will run your code(as per your lambda function) using only the required compute as defined
4. AWS records the compute time in Milliseconds and the quantity of Lambda functions run to calculate the cost of the service

### Components of AWS Lambda:-
1. A **Lambda Function** is compiled of your own code that you want to execute
2. **Event Source** are AWS services that can be used to trigger your Lambda functions
3. **Downstream** are resources that are required during the execution of your Lambda fuction(that maybe SNS or SQS)
4. **Log Streams** help to identify issues and trubleshoot issues with your Lambda function 

## Demo: Creating a Lambda Function:-
* The lambda function is compiled of your own code that you want to invoke as per the defined trigger
* Prior to creating your function, you need to have some code to add to it
* The deployment package will either be .zip or a .jar file and will contain your code and any dependencies
* How you create these deployment packages depends on the programming language that you decide to use within your function
* Once your deployment package has been created, you will need to modify the permission against your .zip file
* If you write from within Lambda itself, then it would create deployment packages for you.
* You can able to upload your code via SDK, Management Console or AWS CLI

### For creating function we have 3 options in Lambda:-
1. **Author from scratch:-** Here we have to write our own code from scratch
2. **Blueprints:-** From this option we can able to choose from a preconfigured templates which we can able to change the code based on our requirements.

