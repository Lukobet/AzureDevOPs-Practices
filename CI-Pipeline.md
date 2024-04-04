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
### clone the repository into your AZURE DEVOPS since that is what i will be using for the CI/CD process

![Screenshot from 2024-04-04 22-19-47](https://github.com/Lukobet/Darey.io_pbl/assets/110517150/36aefdde-fdc8-469c-b454-c1d1278b77f5)

Change the branch from what it is to the Main branch as the default

##### create 3 pipelines

![Screenshot from 2024-04-04 22-35-37](https://github.com/Lukobet/Darey.io_pbl/assets/110517150/541cdec6-a8bc-48ec-ba6d-299a2d2f2b51)
I couldnt pick BUILD AND PUSH IMAGE TO AZURE CONATAINER REGISTRY because my cards are not working on Azure, so i picked DOCKER (BUILD IMAGES)
![Screenshot from 2024-04-04 22-39-34](https://github.com/Lukobet/Darey.io_pbl/assets/110517150/31a34f33-cb75-4ed0-bfd9-56c71006a0b0)
Download Docker Desktop for Mac or Windows. Docker Compose will be automatically installed. On Linux, make sure you have the latest version of Compose.
This solution uses Python, Node.js, .NET, with Redis for messaging and Postgres for storage.

```
-a
```
The vote app will be running at http://localhost:5000, and the results will be at http://localhost:5001.
