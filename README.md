# Film Tracker App Demo with CI/CD and Testing

January 2024

## Overview

The Film Tracker App is a web application designed to help users keep track of movies they have watched or plan to watch. The app allows users to add, edit, and delete films from their personal watchlist, as well as rate and review them.

## Continuous Integration and Continuous Deployment (CI/CD)

This project utilizes GitHub Actions for CI/CD to ensure code quality and streamline the deployment process. The CI/CD pipeline is configured to run automated tests on every pull request to the `develop` and `main` branches. Only pull requests with passing tests are allowed to be merged.

### GitHub Actions Workflow

1. **Automated Testing**: When a pull request is made to the `develop` or `main` branches, GitHub Actions triggers a workflow that runs the project's test suite. This ensures that any new changes do not break existing functionality.
2. **Branch Protection**: The `develop` and `main` branches are protected, meaning that pull requests can only be merged if all tests pass successfully.
3. **Automatic Deployment**: Upon a successful merge to the `main` branch, the application is automatically deployed to Render. This ensures that the latest version of the app is always live and accessible to users.

## Deployment

The application is deployed to Render, a cloud platform that hosts the app and makes it accessible to users. The deployment process is fully automated, thanks to the CI/CD pipeline set up with GitHub Actions.

## Conclusion

By leveraging GitHub Actions for CI/CD, the Film Tracker App ensures high code quality and a seamless deployment process. This setup allows developers to focus on building features while maintaining confidence that the application remains stable and up-to-date.