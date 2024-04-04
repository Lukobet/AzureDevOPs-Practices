## Azure DevOps - CI Setup - (PROJECT 2)
things to do are :

Implementing Continuous Integration (CI)

A front-end web app in Python which lets you vote between two options

A Redis which collects new votes

A .NET worker which consumes votes and stores them

A Postgres database backed by a Docker volume

A Node.js web app which shows the results of the voting in real time
![image](https://github.com/Lukobet/AzureDevOPs-Practices/assets/110517150/dad9f400-8a6d-44f8-830c-97a099b60c6f)
**NOTE**: The worker microservice is written in .NET, voting is written in Python while result is written in node.js.


# Step 1 : Using the Example Voting App from DOCKER (https://github.com/dockersamples/example-voting-app)
A simple distributed application running across multiple Docker containers.

**Getting started**
Download Docker Desktop for Mac or Windows. Docker Compose will be automatically installed. On Linux, make sure you have the latest version of Compose.
This solution uses Python, Node.js, .NET, with Redis for messaging and Postgres for storage.

```
-a
```
The vote app will be running at http://localhost:5000, and the results will be at http://localhost:5001.
