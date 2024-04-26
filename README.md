# Performance - Load Testing with k6 and GitHub Actions

This repository demonstrates how to perform performance testing using k6 and automate the testing process using GitHub Actions.

## Contents

- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Running Locally](#running-locally)
- [GitHub Actions Workflow](#github-actions-workflow)
- [Deployment](#deployment)
- [Customization](#customization)
- [Contributing](#contributing)
- [License](#license)

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (v14 or later)
- [k6](https://k6.io/)

### Running Locally

1. Clone the repository:

   ```bash
   git clone https://github.com/rashmisagar/k6demo.git
   cd k6demo
   
2. Install dependencies:

   ```bash
   npm install -g k6

2. Run the k6 script locally:

   ```bash
   k6 run -o github k6-script.js

## GitHub Actions Workflow

The repository includes a GitHub Actions workflow (defined in .github/workflows/deploy.yml) that automates the performance testing process. The workflow is triggered on each push to the main branch.

The workflow consists of two jobs:

performance-test:
Runs the k6 performance test.
deploy-results:
Deploys k6 test results. Customize the deployment steps based on your needs.

## Deployment

The deploy-results job in the GitHub Actions workflow is responsible for deploying k6 test results. Customize the deployment steps in .github/workflows/deploy.yml to suit your deployment requirements.

## Customization

Feel free to customize the k6 script (k6-script.js) and the GitHub Actions workflow to match your specific use case. Update the k6 script, adjust test scenarios, and modify the deployment steps as needed.

## Contributing

Contributions are welcome! If you find issues or have suggestions, please open an issue or create a pull request.

## License

This project is licensed under the MIT License.
