
# CICD Pipeline

![Static Badge](https://img.shields.io/badge/License-MIT-green)

## Description

- **Motivation**: The motivation behind building this project was to automate the testing and deployment process, ensuring that our application is always up-to-date and stable. By integrating GitHub Actions with Cypress component tests, we can efficiently test the code and automatically deploy the application when changes are merged into the main branch.
- **Why build This Project**: I built this project to demonstrate and implement a Continuous Integration/Continuous Deployment (CI/CD) pipeline that integrates automated component testing using Cypress and seamless deployment through GitHub Actions. The goal was to improve code quality by automating tests, and streamline the deployment process by pushing updates to the live application once the code passes all tests.
- **What problem's did it solve**: This project solves the problem of manual testing and deployment by automating the entire workflow. By running Cypress component tests automatically on every Pull Request to the develop branch and deploying the application when the code is merged to main, we ensure consistent quality and faster delivery to production.
- **Lesson's Learned**: Through building this project, I learned how to configure and optimize GitHub Actions for automated testing and deployment. I also learned how to integrate Cypress for end-to-end testing of components, and how to use this setup to automate the process of merging code and pushing to production environments like Render.
- **What makes your project stand-out**: This project stands out because it offers a fully automated CI/CD pipeline that integrates component testing and deployment. The use of Cypress tests ensures that the code is verified before merging, and the pipeline automates deployments directly to Render when the code is merged into the main branch, saving time and reducing human error.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Credits](#credits)
- [License](#license)
- [Features](#features)
- [How to Contribute](#how-to-contribute)
- [Tests](#tests)
- [Questions](#questions)
- [Links](#links)

## Installation
1. Clone this repository to your local machine:
```
git clone git@github.com:sidhuad/CICDProject.git
```

2. Install the necessary dependencies:
```
npm install
```

3. To set up GitHub Actions:
    - Ensure that you have GitHub Actions enabled in your repository.
    - Set up the appropriate workflow files under .github/workflows/.
    - Create a deploy.yaml file for deployment settings to Render

4. For Cypress tests:
    - Create a test-pr.yaml file for testing upon pull request to develop branch

## Usage
1. Create a new Pull Request (PR) from your feature branch to the develop branch.
2. GitHub Actions will automatically trigger Cypress component tests on the PR.
3. If the tests pass, the action will merge the develop branch into main.
4. GitHub Actions will automatically deploy the application to Render after the merge.

## Credits
- **GitHub Actions** for providing the automation framework
- **Cypress** for end-to-end testing.
- **Render** for seamless hosting and deployment.

## License
A short and simple permissive license with conditions only requiring preservation of copyright and license notices. Licensed works, modifications, and larger works may be distributed under different terms and without source code. https://choosealicense.com/licenses/mit/

## Features
- **Parallel testing:** Speed up the Cypress tests by running them in parallel.
- **Notification on failure:** Set up Slack or email notifications for test failures.
- **Branch protection:** Enforce rules where only passing tests can be merged to main.

## How to Contribute
1. Fork the repository.
2. Create a feature branch.
3. Commit your changes.
4. Submit a Pull Request.
5. All contributions are welcome, and you can suggest new features or improvements.

## Tests
```
This project uses Cypress for component testing. All tests are automatically run by GitHub Actions when a pull request is made to the develop branch.

npm run test
npm run test-component
npm run test-gui

```

## Questions
- For Further Questions and Bug reports Please reach out to me at Github [sidhuad](https://github.com/sidhuad) or email me at adarshsidhu83@gmaail.com

## Links
- [Deployed link](https://cicdproject-vu6h.onrender.com/)
- [Github repo](https://github.com/sidhuad/CICDProject)