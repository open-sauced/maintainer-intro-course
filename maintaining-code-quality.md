# How to Maintain Code Quality and Documentation

When maintaining a project, it is important to keep the code quality high and the documentation up to date. This will help contributors understand the project and make it easier for them to contribute.

In this chapter, we will cover how to maintain code quality and documentation in your open source project.

## Conducting code reviews and ensuring high-quality contributions

Code reviews are an important part of maintaining code quality in an open source project. You will want to take your time to review each pull request and ensure that the proposed changes are high quality and do not introduce any new bugs or issues. You will receive pull requests from contributors who are new to the project and might not be familiar with the codebase. It is important to be patient and provide constructive feedback to help them improve their contributions.

In the following sections, we will cover some best practices for conducting code reviews and ensuring high-quality contributions.

### Implementing Conventional Commits for Pull Requests

Conventional commits is a specification for structuring commit messages. It provides an easy way to understand the type of changes that are being made and helps maintain a clean and organized commit history. It is recommended to use conventional commits in your project to help maintain a clean and organized commit history. In your contributing guidelines, you can ask contributors to use conventional commits when making changes to the project.

Here are some examples of conventional commit messages:

```
feat: add password reset functionality
docs: update installation instructions
chore(build): update dependencies
fix(login): resolve issue with incorrect password validation
refactor(api): streamline error handling in user service
```

You can learn more about conventional commits [here](https://www.conventionalcommits.org/en/v1.0.0/).

### Dealing with Incomplete Pull Requests

The first thing to check for is to make sure that the proposed changes are complete, and that they do not introduce any new bugs or issues. It should be clear what the proposed changes are about and the problem it is trying to solve.

The proposed changes should be linked to an existing issue and all of the necessary information in the pull request template should be filled out. If the pull request is incomplete, reach out to the contributor and ask them to provide the missing information.

Remember that you will be dealing with all levels of contributors. Some might be new to open source and not realize that they are missing information. It is important to be patient and provide constructive feedback to help them improve their contributions.

### Dealing with Large and Unfocused Pull Requests

Sometimes you might get pull requests that are too large and unfocused. Examples of large and unfocused pull requests include:

- Pull requests that try to solve multiple issues at once
- Pull requests that refactor large parts of the codebase
- Pull requests that add a lot of new functionality

In these situations, large pull requests will be difficult to effectively review and will sometimes introduce bugs. It is important to ask the contributor to break down the pull request into smaller, more focused pull requests.

### Setting up Automated Tests

Setting up testing can help ensure that new contributions don't break existing functionality. Automated tests can be run on every pull request to ensure that the new code passes all the tests. This will help maintain the quality of the code and make it easier for contributors to contribute.

If the new pull request is failing some of the tests, reach out to the contributor and ask them to fix the failing tests. Sometimes, the contributor might not understand why the tests are failing. In these cases, work with the contributor to help them understand the problem and fix the failing tests.

To learn more about testing, please refer to this section in the [maintainer power ups chapter](/maintainer-powerups.md#testing).

### Checking For Code Quality

When you are conducting code reviews, it is important to check for code quality and good software engineering practices. This includes checking for things like proper variable naming, adherence to coding standards, and ensuring that the code is easy to read and understand. It is encouraged to have a coding style guide in place to help contributors understand the coding standards of your project.

There are many tools that can help you check for code quality. You can setup linting for your project to ensure there are no syntax errors or style issues. You can also setup code scanning tools to check for security vulnerabilities and other issues in the codebase.

To learn more about these tools, please refer to this section in the [maintainer power ups chapter](/maintainer-powerups.md#code-scanning-tools).

### Setting up branch protection rules

On GitHub, you can set up branch protection rules to ensure that all pull requests are reviewed before they are merged. This can help maintain the quality of the code and ensure that all contributions are reviewed by a maintainer before they are merged into the project.

You can also setup rules to ensure that multiple reviewers are required before a pull request can be merged. This can be helpful for larger projects where multiple maintainers are responsible for reviewing pull requests.

You can learn more about branch protection rules in the official GitHub [documentation](https://docs.github.com/en/repositories/configuring-branches-and-merges-in-your-repository/managing-protected-branches/managing-a-branch-protection-rule#about-branch-protection-rules).

## Maintaining project documentation and keeping it up to date

Documentation is an important part of maintaining an open source project. It helps contributors understand the project and makes it easier for them to contribute. It is important to keep the documentation up to date and ensure that it reflects the current state of the project.

It is recommended to review your project's documentation regularly to ensure that it is up to date and accurate. You can setup a schedule for once a month to manually review your project's documentation. As you are reviewing the documentation, look for ways to improve it and make it easier for contributors to understand the project. Think about times when a new contributor struggled to understand the project and update the documentation to make it easier for them to understand.

Another thing to consider in your review is running through the installation and setup instructions to ensure that they are accurate and up to date. Are there any steps that are missing? Are there any steps that are no longer necessary? If so, update the documentation to reflect the current state of the project.

If you have a more complex project, you might consider adding diagrams or images to help explain the architecture of the project. This can help contributors understand how the project is structured and make it easier for them to contribute.
