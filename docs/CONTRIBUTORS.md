# Contributor Guide

## Table of Contents
- Branch Management Policy
- Commit Messages Conventions
- Code Conventions
- Release Policy
- Managing Issues and Branches
- Continuous Integration
- Contact

## Branch Management Policy
- **Branch Naming**: Branches should be named based on the issue they address. For example, `issue-#123-fix-bug` or `feature-add-new-game-mode`.
- **Branch Placement**: All branches should be created from the `main` branch.
- **Merging**: A branch can be merged into the `main` branch after a pull request has been reviewed and approved by at least one other contributor.

## Commit Messages Conventions
- Use clear and descriptive commit messages.
- Follow the format: `type(scope): description`.
    - **Type**: `feat` (feature), `fix` (bug fix), `docs` (documentation), `style` (formatting), `refactor` (refactoring), `test` (adding tests), `chore` (maintenance).
    - **Scope**: The part of the codebase affected (optional).
    - **Description**: A brief summary of the changes.

### Examples
- `feat(game): add new game mode`
- `fix(ui): resolve button alignment issue`

## Code Conventions
- Follow the Java coding standards.
- Use meaningful variable and method names.
- Write comments to explain complex logic.

## Release Policy
- **Release Pattern**: Follow semantic versioning (e.g., `v1.0.0`).
- **Release Frequency**: Aim for a new release every two weeks.

## Managing Issues and Branches
1. **Creating an Issue**: When you identify a task, create an issue in the repository. Provide a clear description of the task.
2. **Creating a Branch**: Create a new branch from the `main` branch. Name the branch based on the issue (e.g., `issue-#123-fix-bug`).
3. **Working on the Branch**: Make your changes in the branch. Commit your changes with clear and descriptive messages.
4. **Creating a Pull Request**: Once your changes are ready, create a pull request. Link the pull request to the issue it addresses.
5. **Review and Merge**: Another contributor should review your pull request. Once approved, the pull request can be merged into the `main` branch.


## Continuous Integration

This project uses GitHub Actions for continuous integration. 
The CI pipeline is defined in the `.github/workflows/ci.yml` file.

### Triggering a Build

The CI pipeline is automatically triggered on the following events:
- Push to the `main` branch
- Pull request to the `main` branch

### Steps in the Pipeline

1. **Checkout repository**: Clones the repository.
2. **Set up JDK 11**: Prepares the Java environment.
3. **Build with Maven**: Compiles and packages the project.
4. **Run tests**: Executes unit tests.
5. **Static code analysis**: Checks code style and formatting.
6. **Code coverage**: Generates a coverage report.
7. **Package application**: Packages the application into a JAR file.
8. **Deploy to server**: Deploys the application to a live environment.
9. **Telemetry setup**: Sets up telemetry for monitoring.

### Deployment

To deploy the application, the CI pipeline automatically copies the JAR file to the server and runs it. Ensure the server details and paths are correctly configured in the workflow file.

## Contact
For any questions or feedback, please open an issue in the repository or contact the project maintainers.