# How to Setup your Open Source Project

There are a lot of things to consider when setting up your open source project. In this portion of the guide, we will walk through key components that every project needs to be successful.

## How to Write a Good README

A `README.md` is an introduction into what your open source project is all about. A good `README.md` should be clear, concise, up to date, and detailed. This file is located in your root directory and serves as the first impression for your contributors.

Here are some things to consider inside your `README.md`:

- project title and summary
- brief instructions on how to setup the project
- images of the app and/or code examples
- tech and tools used in the project
- link to the contributing guide
- link to the code of conduct
- link to the open source license
- link to community Discord, Slack group or GitHub discussions

A `README.md` is written in a markup language called [markdown](https://www.markdownguide.org/). This is a popular language used in open source documentation like README's.

Here are a few examples of good `README.md` files:

- [OpenSauced App](https://github.com/open-sauced/app/blob/beta/README.md)
- [Astro documentation](https://github.com/withastro/astro/blob/main/README.md)
- [freeCodeCamp](https://github.com/freeCodeCamp/freeCodeCamp/blob/main/README.md)

## How to Write an Installation Guide for Contributors

When a new contributor is interested in working with your project, they will need a clear step by step guide on how to setup everything locally. This guide should include the following items:

- instructions for forking the repository
- instructions for cloning the repository
- instructions for installing the dependencies
- instructions for setting up the environment variables
- instructions for setting up the database if applicable
- instructions for running the project locally
- instructions for setting up Docker containers if applicable

The best way to test your guide is by setting up the project locally using your guide. You will learn quickly if anything is missing or not clear if you run into issues getting your project to work.

### Where to Place the Installation Guide

The best place for installation instructions should be in your project's `README.md` file. This will be the most accessible file for your contributors. It would good to have a section at the top for setting up the project locally.

Another good place would be in the `CONTRIBUTING.md` file. This file is used to cover topics like installation setup, testing, linting, workflows, etc. You can place the installation instruction towards the top of your `CONTRIBUTING.md` file.

If your project is on the larger side, then you might consider having a separate documentation site and dedicating a section for installation in there. You can use documentation site generators like [docsify](https://docsify.js.org/#/), [Docusaurus](https://docusaurus.io/) or [Starlight](https://starlight.astro.build/).

## How to Choose a License for Your Project

An open source software license dictates how others can use, modify or distribute your software. Every project should have a clearly defined license within a `LICENSE.md` file. This file is usually located in the root directory so it is easily accessible by everyone.

Some licenses are more restrictive like the GNU GPL (General Public License) while others are less restrictive like the MIT license. Here are a few examples of licenses for OpenSauced projects:

- [OpenSauced Docs - MIT license](https://github.com/open-sauced/docs/blob/main/LICENSE)
- [OpenSauced App - Apache License 2.0](https://github.com/open-sauced/app/blob/beta/LICENSE)

To get a better understanding on which license would be work best for your project, please read through this helpful [article](https://www.freecodecamp.org/news/how-open-source-licenses-work-and-how-to-add-them-to-your-projects-34310c3cf94/). For a complete list of Open Source Initiative(OSI) approved licenses, please check out their list [here](https://opensource.org/licenses/).

## How to Write a Code Of Conduct

A code of conduct is an established set of rules and behaviors that all open source participants agree to abide by. This document helps to ensure a healthy and inclusive environment for all involved with the project.

This set of rules and expectations, will go in inside a `CODE_OF_CONDUCT.md` file in the root directory of your project. Most Code of Conducts are broken up into three categories: pledge, standards, and enforcement.

### Project pledge

The opening pledge is a statement of the type of environment that the project wants to create. Here is an excerpt from the [OpenSauced Code of conduct](https://github.com/open-sauced/.github/blob/main/CODE_OF_CONDUCT.md):

In the interest of fostering an open and welcoming environment, we as contributors and maintainers pledge to making participation in our project and our community a harassment-free experience for everyone, regardless of age, body size, disability, ethnicity, sex characteristics, gender identity and expression, level of experience, education, socio-economic status, nationality, personal appearance, race, religion, or sexual identity and orientation.

### Project standards

The standards section explicitly lays out what is considered acceptable and non acceptable behavior by all project participants.

Here is an example from the [OpenSauced Code of conduct](https://github.com/open-sauced/.github/blob/main/CODE_OF_CONDUCT.md):

Examples of behavior that contributes to creating a positive environment
include:

- Using welcoming and inclusive language
- Being respectful of differing viewpoints and experiences
- Gracefully accepting constructive criticism
- Focusing on what is best for the community
- Showing empathy towards other community members

Examples of unacceptable behavior by participants include:

- The use of sexualized language or imagery and unwelcome sexual attention or
  advances
- Trolling, insulting/derogatory comments, and personal or political attacks
- Public or private harassment
- Publishing others' private information, such as a physical or electronic
  address, without explicit permission
- Other conduct which could reasonably be considered inappropriate in a
  professional setting

### Project enforcement

If any member of the project is behaving in a unacceptable way that violates your Code of conduct, then you will want to explicitly state what will happen in that situation.

Here is an example from the [OpenSauced Code of conduct](https://github.com/open-sauced/.github/blob/main/CODE_OF_CONDUCT.md):

Instances of abusive, harassing, or otherwise unacceptable behavior may be reported by contacting the project team at hello@opensauced.pizza. All complaints will be reviewed and investigated and will result in a response that is deemed necessary and appropriate to the circumstances. The project team is obligated to maintain confidentiality with regard to the reporter of an incident. Further details of specific enforcement policies may be posted separately.

Project maintainers who do not follow or enforce the Code of Conduct in good faith may face temporary or permanent repercussions as determined by other members of the project's leadership.

### Contributor Covenant

The Contributor Covenant is a code of conduct that you can use and adapt for your open source projects. To learn more, please visit their [website](https://www.contributor-covenant.org/).

## How create Contributing Guides

A `CONTRIBUTING.md` file, is a guide on how contributors can help with your project. This file is usually located in the root directory of a project so it can be easily accessible by everyone.

Your guide should include the following sections:

- project setup instructions
- guidelines for creating new issues like bug reports and feature requests
- guidelines for which issues are available for contribution
- guidelines for commit conventions for pull requests
- guidelines for code and style conventions
- guidelines for creating pull requests

For an in depth look into how to create a strong `CONTRIBUTING.md` file, please read through this [OpenSauced article](https://dev.to/opensauced/how-to-make-a-delicious-contributing-guide-4bp3).

## How to Create Issue Templates

Issue templates are helpful because you can guide your contributors on how to provide specific and structured information when opening issues in your project. This will help you make sure you are receiving the desired information in order to triage the issue correctly.

You can create a variety of issue templates, like bug reports, feature requests, documentation updates, etc. Inside these templates, you can have required fields like steps on reproducing the bug or a details section for a feature request. You can also attach specific labels like "Needs triage", or "Bug" to certain types of issue templates.

### How to Create Issue Templates Using GitHub's Template Builder

There are two ways to create issue templates. The first way is to use GitHub's template builder. For this option, you will need to go to your project's settings, navigate to the "Features" section and click on Set up templates. Here is a [detailed guide](https://docs.github.com/en/communities/using-templates-to-encourage-useful-issues-and-pull-requests/configuring-issue-templates-for-your-repository#creating-issue-templates) from the GitHub documentation.

### How to Create Issue Templates Using `yaml` Files

You can also create custom issue forms using `yaml`. You would start by creating a folder called `.github` in the root directory. Then you will need to add a folder inside there called `ISSUE_TEMPLATE`. (**Note**: It is important that this folder is in all caps or else it will not work on GitHub.)

Inside the `ISSUE_TEMPLATE` folder, you can create different `yaml` files like a `bug.yml` or `feature.yml` file. Here is an [example bug report](https://raw.githubusercontent.com/open-sauced/.github/main/.github/ISSUE_TEMPLATE/bug_report.yml) used by OpenSauced.

To learn more about issue templates, please review the [documentation](https://docs.github.com/en/communities/using-templates-to-encourage-useful-issues-and-pull-requests/configuring-issue-templates-for-your-repository) on GitHub.

## How to Create PR Templates

Similar to issue templates, pull request templates, allow you to guide your contributors on how to provide specific and structured information when opening pull requests in your project. This template will be in a file called `PULL_REQUEST_TEMPLATE.md` and it is usually located either in the root directory or the `.github` directory.

Here are a few things to consider inside your pull request template:

- section for contributors to detail which changes were made and why
- section for the type of change made (Ex. bug fix, feature, style update, etc)
- section to link corresponding issue tickets to the PR (Ex. closes #123 or fixes #456)
- section to place screenshots and/recordings if applicable

Here is a example of a [good pull request template](https://raw.githubusercontent.com/open-sauced/.github/main/.github/PULL_REQUEST_TEMPLATE.md) used by OpenSauced. To learn more about creating pull request templates, please read through the [GitHub documentation](https://docs.github.com/en/communities/using-templates-to-encourage-useful-issues-and-pull-requests/creating-a-pull-request-template-for-your-repository).

## How to Work with GitHub Project Boards

GitHub project boards are a way for you and your team to structure your list of issues. You can organize your issues in a classic [kanban](https://docs.github.com/en/issues/organizing-your-work-with-project-boards/managing-project-boards/about-project-boards) style by placing your issues in todo, in progress, in review and done columns. This will make it easy for you and your team to track the progress for upcoming releases and new feature work.

To create a new project board for an individual repository, you can navigate to your GitHub profile and click on the projects tab. From there you will see a green "New project" button where you can create a new board and link it to a repository. You can also choose to make this board private to core maintainers or publicly visible to everyone.

To learn more about GitHub project boards, please read through the [documentation](https://docs.github.com/en/issues/organizing-your-work-with-project-boards/managing-project-boards/about-project-boards).
