# NodeJS-Portfolio-Application
## 🌐 Node.js Portfolio Website — AWS CodePipeline CI/CD (Elastic Beanstalk Deployment)

![Build Status](https://codebuild.us-east-1.amazonaws.com/badges?uuid=eyJlbmNyeXB0ZWREYXRhIjoiUnVQUWZQaGwybE5UNXcvWUFER0ZkUExtMzMvaThjMmNVSm13UytkNkJ6V0N0UnRmV2RWWVdZUVZjekdzYVBTTm1aQUdlZ0ZsamtJSmZ2S1graHQxK2tBPSIsIml2UGFyYW1ldGVyU3BlYyI6IlRoc1RJb0ZyN1VVeUxPV28iLCJtYXRlcmlhbFNldFNlcmlhbCI6MX0%3D&branch=main)

This repository demonstrates a fully automated CI/CD pipeline for deploying my Node.js portfolio website to AWS Elastic Beanstalk using AWS CodePipeline and CodeBuild.
It is a practical DevOps example showing how modern cloud applications can be built and deployed automatically with zero manual steps.
________________________________________
🚀 Project Overview
This project includes:
•	A Node.js (Express) portfolio website
•	An automated deployment pipeline using AWS CodePipeline
•	Build automation via AWS CodeBuild
•	Deployment directly to Elastic Beanstalk
•	GitHub-triggered CI/CD workflow
Every time I push changes to the main branch, the application is rebuilt and redeployed to my Elastic Beanstalk environment immediately.
________________________________________
🧰 Technologies Used
Application Stack
•	Node.js (Express.js)
•	HTML/CSS/JavaScript UI for the portfolio
AWS Services
•	AWS CodePipeline – Orchestrates the full CI/CD flow
•	AWS CodeBuild – Installs dependencies + builds the app
•	Elastic Beanstalk (EB) – Application hosting + environment management
•	Amazon S3 – Stores build artifacts
•	CloudWatch – Build logs and monitoring
•	IAM – Secure pipeline roles
________________________________________
🔁 Pipeline Workflow
1️⃣ Source Stage — GitHub
•	Pipeline triggers automatically on every push
•	CodePipeline downloads the latest commit
2️⃣ Build Stage — CodeBuild
•	Installs Node.js dependencies
•	Runs optional test scripts
•	Creates the deployment artifact
•	Uploads the artifact to S3
3️⃣ Deployment Stage — Elastic Beanstalk
•	CodePipeline sends the build artifact to Elastic Beanstalk
•	Elastic Beanstalk:
o	Updates the environment
o	Deploys the new application version
o	Performs rolling updates for stability
________________________________________
🏗️ Architecture Summary
GitHub (Source)
        ↓
AWS CodePipeline
        ↓
AWS CodeBuild (Build & Package)
        ↓
Amazon S3 (Artifacts)
        ↓
AWS Elastic Beanstalk (Deployment)
This represents a complete automated delivery workflow from source control → build → deploy.
________________________________________
🖥️ Portfolio Website
The deployed Node.js application serves as my personal portfolio, showcasing:
•	AWS Cloud projects
•	Hands-on labs
•	Certifications
•	Articles & write-ups
•	Contact information
Elastic Beanstalk ensures:
•	Scalable hosting
•	Health monitoring
•	Zero-downtime updates
•	Automatic load balancing (if configured)
________________________________________
🛡️ Why This Project Matters
This project demonstrates real-world cloud engineering skills:
•	Building CI/CD pipelines
•	Deploying Node.js applications to Elastic Beanstalk
•	Automating delivery workflows
•	Using GitHub + AWS integrations
•	Implementing production-grade DevOps practices
This is the kind of setup used by modern engineering teams to ship updates quickly and safely.
________________________________________
🏁 Conclusion
This project brings together the full power of AWS developer tools to automate deployments for my Node.js portfolio website.
With CodePipeline and Elastic Beanstalk, I can deliver updates reliably, consistently, and without manual intervention.

