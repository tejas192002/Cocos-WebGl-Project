# CI/CD Pipeline Documentation

## Workflow Description

This GitHub Actions workflow is designed to automate the build and deployment process for the Cocos WebGL project. The workflow is triggered by pull requests targeting the dev branch and consists of three stages: build, archive, and deploy.

## Build and Deployment Process

1. The workflow checks out the code from the dev branch.
2. It installs the necessary dependencies using `npm install`.
3. It builds the Cocos WebGL project using `npm run build:webgl`.
4. The build artifacts are archived and stored as `cocos-webgl-build`.
5. The workflow checks out the main branch and copies the build output to the appropriate location.
6. The changes are committed and pushed to the main branch.

## Setup Instructions

To set up and modify the workflow, follow these steps:

1. Create a new file in the `.github/workflows` directory of your repository.
2. Copy the contents of the `cocos-webgl-ci-cd.yml` file into the new file.
3. Modify the workflow as needed to suit your project's requirements.
4. Commit and push the changes to your repository.
