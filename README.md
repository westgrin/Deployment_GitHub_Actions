# # Mini Project - Deployment Pipelines with GitHub Actions (Local Setup)

## Project Overview
This project automates a CI/CD pipeline for a Node.js application using GitHub Actions, with semantic versioning, automated releases, and deployment to AWS Elastic Beanstalk. Executed on WSL Ubuntu with VS Code and Git Bash.

## Setup
- Initiated on Jul 07, 2025, 11:47 AM WAT.
- Used WSL Ubuntu, VS Code, and Git Bash in `C:\Users\Abraham\Documents\Workspace\Deployment_GitHub_Actions`.

## Execution Steps
1. **Set Up Node.js Application**:
   - Initialized Node.js project, installed Express.js, Jest, and Supertest, and created `index.js` with `/health` endpoint.
   - Added tests in `__tests__/app.test.js` and set up AWS CLI.
   - [Screenshot: `nodejs_npm_version_local.png` - Shows Node.js and npm versions.]
   - [Screenshot: `awscli_version_local.png` - Shows AWS CLI version.]
   - [Screenshot: `npm_install_output_local.png` - Shows dependency installation.]
   - [Screenshot: `npm_test_output_local.png` - Shows test output.]
   - [Screenshot: `nodejs_app_output_local.png` - Shows app output.]
2. **Set Up AWS Elastic Beanstalk**:
   - Initialized Elastic Beanstalk and created environment.
   - [Screenshot: `eb_setup_output_local.png` - Shows `eb init` and `eb create` output.]
3. **Create GitHub Actions Workflow**:
   - Added `.github/workflows/deploy-to-aws.yml` with versioning and deployment.
   - Pushed to `https://github.com/westgrin/deploy-github-actions`.
   - [Screenshot: `github_repo_files_local.png` - Shows repository files.]
   - [Screenshot: `github_secrets_config_local.png` - Shows secrets setup.]
   - [Screenshot: `github_actions_run_local.png` - Shows workflow run.]
   - [Screenshot: `aws_app_output_local.png` - Shows deployed app.]
4. **Side Hustle Task**:
   - Added release creation for tags and tested with a PR.
   - [Screenshot: `github_release_output_local.png` - Shows release page.]

## Learning Summary
This project enhanced my GitHub Actions skills, automating versioning, releases, and AWS deployment. I learned semantic versioning, dependency caching, and cloud integration, aligning with my DevOps goals (June 16, 2025) for efficient automation.

## Tools Used
- **WSL Ubuntu Terminal**: For Node.js, AWS CLI, and Git commands.
- **VS Code**: For editing code and `README.md`.
- **Git Bash**: For GitHub operations.
- **GitHub Actions**: For CI/CD automation.
- **AWS Elastic Beanstalk**: For deployment.

## Project Deliverables
- **Documentation**: This `README.md` with steps and learning summary.
- **Screenshots**:
  - `nodejs_npm_version_local.png`
  - `awscli_version_local.png`
  - `npm_install_output_local.png`
  - `npm_test_output_local.png`
  - `nodejs_app_output_local.png`
  - `eb_setup_output_local.png`
  - `github_repo_files_local.png`
  - `github_secrets_config_local.png`
  - `github_actions_run_local.png`
  - `aws_app_output_local.png`
  - `github_release_output_local.png`
- **Script Link**: [GitHub Repository](https://github.com/westgrin/deploy-github-actions)

## Troubleshooting
- Fixed `ECONNRESET` error by setting DNS to `8.8.8.8` and clearing npm cache.
- Ensured commands were run in `/mnt/c/Users/Abraham/Documents/Workspace/Deployment_GitHub_Actions`.
- Verified AWS credentials in GitHub Secrets.

## Conclusion
This project successfully implemented a CI/CD pipeline with GitHub Actions, automating deployment to AWS. The side hustle task strengthened my release management skills, preparing me for advanced DevOps practices.