
# Task 2: Simple Jenkins CI/CD Pipeline

## Objective
Automate the build, test, and deployment of a simple Node.js application using Jenkins and Docker.

## Tools Used
- Jenkins
- Docker
- GitHub
- Node.js

## Project Files
- `app.js` - Simple web application.
- `package.json` - Application metadata and test command.
- `Dockerfile` - Instructions to build the Docker image.
- `Jenkinsfile` - Jenkins pipeline definition.

## Pipeline Stages
1. Checkout - Retrieves the project from GitHub.
2. Build - Builds a Docker image.
3. Test - Checks JavaScript syntax.
4. Deploy - Runs the application in a Docker container.

## Access the Application
When the pipeline runs successfully, open:
http://localhost:3000

## Result
The Jenkins pipeline automates the build, test, and deployment steps using Docker.
