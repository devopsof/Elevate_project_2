MyApp

A simple Node.js web app displaying random cat images using TheCatAPI. Dockerized for easy deployment with a Jenkins CI/CD pipeline.

Files

- app.js – Express server
- index.html – Frontend page
- Dockerfile – Docker setup
- package.json & package-lock.json – Node dependencies
- Jenkinsfile – CI/CD pipeline

Setup

1. Clone repo:
   git clone https://github.com/devopsof/Elevate_project_2.git
2. Install dependencies:
   npm install
3. Run locally:
   node app.js (http://localhost:3000)

Docker

- Build: docker build -t myapp .
- Run: docker run -d -p 8888:3000 myapp (http://localhost:8888)

Notes

- Dockerfile exposes port 3000; map correctly with -p  
- JSON files must list dependencies for npm install
