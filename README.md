# Postman Autotest JavaScript

## Summary of Repo

This repository contains API integration tests written in Postman, executed via Newman, and backed by a local mock server using yaml-server. The project targets a RESTful API (e.g., users, orders) and validates various functional and performance aspects. All test scripts follow the AAA pattern (Arrange, Act, Assert).

## Requirements

- Node.js (latest LTS version recommended)
- Postman (for authoring and debugging requests)
- Newman (for CLI-based test runs)
- Allure Reporter (for rich test reporting)
- yaml-server (mock REST API server)
- GitHub + GitHub Pages (to run CI/CD and host reports)

## Install

1. Clone the repository:
   ```sh
   git clone https://github.com/Anna-Ruban-ua/Postman-Newman-Automation
   ```
2. Navigate to the project directory:
   ```sh
   cd Postman-Newman
   ```
3. Install dependencies:
   ```sh
   npm install
   ```
4. Start the local API server:
   ```sh
   npm run tern-on-api
   ```

## Run tests

1. Run tests with Newman:
   ```sh
   npm run tests:newman
   ```

## CI/CD pipeline is set up via GitHub Actions:
- Installs dependencies
- Starts the local server
- Executes Newman tests
- Generates Allure report
- Deploys the report to GitHub Pages