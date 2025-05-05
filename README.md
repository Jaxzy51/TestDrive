
# Test-Drive CI-CD

![License](https://img.shields.io/badge/License-MIT-blue.svg)

## Description

This project demonstrates a CI/CD pipeline integration for a full-stack MERN application using GitHub Actions, Cypress, and Render. The setup ensures clean and tested code through component testing on all pull requests to the `develop` branch and automatic deployment to Render when merged into the `main` branch. This workflow aligns with industry standards for Continuous Integration and Continuous Deployment, promoting a robust structure for team collaboration and automated delivery.

---

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Technologies](#technologies)
- [URL Link](#url-link)
- [Contributing](#contributing)
- [Tests](#tests)
- [License](#license)

---

## Installation

1. Clone the repository:
   ```bash
   git clone git@github.com:Jaxzy51/TestDrive.git
   ```

2. Navigate into the project directory:
   ```bash
   cd GitHub-Actions-CI-CD-Setup
   ```

3. Right-click the root `package.json` file and open it in the integrated terminal.

4. Install dependencies:
   ```bash
   npm install
   ```

5. Build the application:
   ```bash
   npm run build
   ```

6. Seed the database:
   ```bash
   npm run seed
   ```

7. Start the application:
   ```bash
   npm run develop
   ```

---

## Usage

To begin working with the CI/CD pipeline:

1. From `main`, create a `develop` branch:
   ```bash
   git checkout -b develop
   ```

2. Make your changes in `develop` or create a feature branch:
   ```bash
   git add .
   git commit -m "your commit message"
   git push
   ```

3. On GitHub:
   - Go to the **Pull Requests** tab.
   - Change the base to `main` and compare to `develop`.
   - Click **Create Pull Request**.

4. GitHub Actions will automatically test the changes before merge.

5. If tests pass, merge the pull request. If not, revise and retry.

---

## Technologies

### Frontend

![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=white)
![React DOM](https://img.shields.io/badge/React%20DOM-61DAFB?style=for-the-badge&logo=react&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-323330?style=for-the-badge&logo=javascript&logoColor=F7DF1E)

### Backend

![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![ts-node](https://img.shields.io/badge/ts--node-3178C6?style=for-the-badge&logo=typescript&logoColor=white)

### Development & Testing Tools

![Concurrently](https://img.shields.io/badge/Concurrently-000000?style=for-the-badge&logo=concurrently&logoColor=white)
![Cypress](https://img.shields.io/badge/Cypress-17202C?style=for-the-badge&logo=cypress&logoColor=white)
![Vitest](https://img.shields.io/badge/Vitest-6E9F18?style=for-the-badge&logo=vitest&logoColor=white)
![npm](https://img.shields.io/badge/npm-CB3837?style=for-the-badge&logo=npm&logoColor=white)

---

## URL Link

[Deployed App on Render](https://ci-cd-setup-r3ls.onrender.com)

---

## Contributing

No contributions are needed for this project.

---

## Tests

To test the GitHub Actions workflow:

1. From `main`, create a `develop` branch:
   ```bash
   git checkout -b develop
   ```

2. Optionally, create another branch from `develop`:
   ```bash
   git checkout -b github/actions/test
   ```

3. Make your code changes and commit them:
   ```bash
   git add .
   git commit -m "Test commit message"
   git push
   ```

4. On GitHub:
   - Go to **Pull Requests**.
   - Compare branches (`main` ← `develop` or `develop` ← `github/actions/test`).
   - Click **Create Pull Request**.

5. Navigate to the **Actions** tab to monitor test results.

6. If tests pass, proceed to merge. If they fail, revise the code and retry.

7. Repeat the process as needed to complete merges to `main`.

---

## License

This project is licensed under the MIT License.