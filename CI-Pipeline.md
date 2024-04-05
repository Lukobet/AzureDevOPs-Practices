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
I couldnt pick BUILD AND PUSH IMAGE TO AZURE CONATAINER REGISTRY because my cards are not working on Azure, so i followed the steps stated here on how to  push to dockerhub (https://www.youtube.com/watch?v=KvddwTNaGTo))
![Screenshot from 2024-04-05 21-00-05](https://github.com/Lukobet/Darey.io_pbl/assets/110517150/7fa9fce6-dddc-4692-9975-ee397559743a)
![Screenshot from 2024-04-05 21-09-41](https://github.com/Lukobet/Darey.io_pbl/assets/110517150/b786536e-4ae4-4f36-b232-96c32e2f10b0)




