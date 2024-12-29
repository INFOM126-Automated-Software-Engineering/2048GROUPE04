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
- The project uses GitHub Actions for continuous integration.
- The pipeline automatically compiles the project and executes tests on each push to the repository.

## Contact
For any questions or feedback, please open an issue in the repository or contact the project maintainers.