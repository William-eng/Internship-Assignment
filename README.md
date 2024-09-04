# ToDo App with CI/CD Pipeline

A simple ToDo app built with React and integrated with a CI/CD pipeline using GitHub Actions. The app is automatically deployed to GitHub Pages whenever changes are pushed to the `main` branch.

## CI/CD Workflow

The CI/CD pipeline automates the build and deployment process to GitHub Pages whenever changes are pushed to the `main` branch.

### Workflow Steps

#### Build and Deploy

Whenever there is a push to the `main` branch, the workflow triggers a build job and deploys the app:

## Getting Started

### Prerequisites

- Node.js and npm should be installed.

Explanation of Workflow
Test Job:

Purpose: Runs unit tests to ensure code quality before the build.
Steps:
Checkout Code: Checks out the code from the repository.
Install Node: Sets up Node.js environment.
Install Dependencies: Installs the required dependencies.
Run Unit Tests: Executes the unit tests.
Build Job:

Steps:
Checkout Code: Checks out the code.
Install Node: Sets up Node.js.
Install Dependencies: Installs dependencies.
Build Project: Builds the project.
Upload Artifact: Uploads the build artifact for deployment.
Deploy Job:

Depends on: The build job. This job will only run if the build job is successful.
Steps:
Download Artifact: Downloads the build artifact.
Deploy to GitHub Pages: Deploys the build artifact to GitHub Pages

### Live
Access the live ToDo app [here](https://william-eng.github.io/Internship-Assignment/).

### Installation

   ```bash
   git clone https://github.com/william-eng/Internship-Assignment.git
   cd todo
   npm install
   npm start


Committing and Pushing Changes
Commit Changes:



git add .
git commit -m "message"
Push to GitHub:

bash
Copy code
git push origin main



