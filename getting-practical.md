# Let's Get Practical: Starting Your Project

Now that you've gone through the course and understand what it takes to be a successful maintainer, let's get practical and start your first open source project as a maintainer!

## Prerequisites

You'll need to have the following:

- [Visual Studio Code (VS Code)](https://code.visualstudio.com/)
- A [GitHub Account](https://github.com)

## Choosing Your Project 

Sometimes the hardest part is deciding what you're going to work on. Here are some general ideas to get you started:
   - Identify a problem or need in the open source community.
   - Think about a topic you're passionate about that others might be interested in as well.
   - Think about a problem that you've had to solve that others can benefit from.

Don't think too hard about it now. You can always go back and update things later. For now, if you need a place to get started, let's create a repository about your favorite open source resources.

## Create Your Repository

We're going to walk through the steps to set up your project in GitHub. This isn't the only way to get started with a project, but it's the way we're going to demonstrate. 

   - Go to [GitHub](https://github.com) and sign in.
   - Click on the "+" icon in the upper right corner and select "New repository."
   - Enter a repository name, description, and choose whether the repository should be public or private.
   - Initialize the repository with a README file and add a license.
   - Click "Create repository."

   ![setting up a repo](./assets/gifs/set-up-repo.gif)

If you're using our starter idea, you could use the following:

    - Name: favorite-open-source-resources
    - Description: A markdown file of resources I've found to be most helpful. 

## Adding Repository Documentation

Now that you have the repository, you can either edit it directly in GitHub or clone the project and work on it locally. We previously learned about how to create good READMEs, Contributing Guides, and Code of Conducts in [How to Set Up Your Project](how-to-setup-your-project.md/how-to-setup-your-project.md). If you need a reminder, take a look back at that chapter.


 ## Set Up Contributing Guidelines
   - Create a new file named `CONTRIBUTING.md` in your repository.
   - Outline the process for submitting issues and pull requests.
   - Include coding standards, style guides, or any specific requirements.
   - Mention how contributors can ask for help or clarification.

## Issue Forms, Pull Request Templates, and Labels

Creating good issues and using labels will help to create a strong project. Before creating your first issue, start by creating issue templates to make the process of submitting an issue clear to your contributors. 

### Creating Issue Forms

In this section, we're going to create an issue template for a bug report. You can create templates for other types of issues as well, such as feature requests, questions, or documentation requests. Below are the steps to create the template. After the steps, we'll give you what we use at OpenSauced. Feel free to copy and paste that information into your own repository and update it as needed.

   - Create a new folder named `.github` in the root of your repository.
   - Within that folder, create a new folder named `ISSUE_TEMPLATE`.
   - In the `.github/ISSUE_TEMPLATE` directory, create a new file named `bug_report.yml`.
   - Add a title and description to the template.
   - Add a checklist of steps to reproduce the bug.
   - Add a section for the expected behavior and actual behavior.
   - Add a section for screenshots, if applicable.
   - Add a section for additional context, if applicable.

Here's what we use at OpenSauced:

```yml
name: 🐛 Bug report
description: Create a bug report to help us improve Open Sauced 🍕
title: "Bug: "
labels: [👀 needs triage, 🐛 bug]
body:
  - type: markdown
    attributes:
      value: |
        Thanks for taking the time to fill out this bug report!
  - type: textarea
    attributes:
      label: Describe the bug
      description: A clear and concise description of what the bug is.
    validations:
      required: true
  - type: textarea
    attributes:
      label: Steps to reproduce
      description: Describe how to reproduce the behavior.
      placeholder: |
        1. Go to '...'
        2. Click on '...'
        3. Scroll down to '...'
        4. See error
    validations:
      required: true
  - type: dropdown
    attributes:
      multiple: true
      label: Browsers
      description: Select the browsers where the issue can be reproduced (that you know of).
      options:
        - "Chrome"
        - "Firefox"
        - "Safari"
        - "Edge"
        - "Opera"
        - "Other (add additional context)"
  - type: input
    id: context
    attributes:
      label: Additional context (Is this in dev or production?)
      description: Add any other context about the problem or helpful links here.
  - type: checkboxes
    id: terms
    attributes:
      label: Code of Conduct
      description: By submitting this issue, you agree to follow our [Code of Conduct](https://docs.opensauced.pizza/contributing/code-of-conduct/)
      options:
        - label: I agree to follow this project's Code of Conduct
          required: true
  - type: checkboxes
    id: contribution
    attributes:
      label: Contributing Docs
      description: If you plan on contributing code please read - [Contribution Guide](https://docs.opensauced.pizza/contributing/introduction-to-contributing/)
      options:
        - label: I agree to follow this project's Contribution Docs
          required: false
```

Now let's follow the same process and make a feature request template. 

   - In the `.github/ISSUE_TEMPLATE` directory, create a new file named `feature_request.yml`.
   - Add a title and description to the template.
   - Add a checklist of steps to reproduce the bug.
   - Add a section for the expected behavior and actual behavior.
   - Add a section for screenshots, if applicable.
   - Add a section for additional context, if applicable.

Here's what we use at OpenSauced:

```yml
name: 🚀 Feature request
description: Suggest an idea for this project 💡
title: "Feature: "
labels: [👀 needs triage, 💡 feature]
body:
  - type: markdown
    attributes:
      value: |
        Thanks for taking the time to fill out this feature request!
  - type: dropdown
    attributes:
      multiple: false
      label: Type of feature
      description: Select the type of feature request, the lowercase should also be the PR prefix.
      options:
        - "🍕 Feature"
        - "🐛 Fix"
        - "📝 Documentation"
        - "🎨 Style"
        - "🧑‍💻 Refactor"
        - "🔥 Performance"
        - "✅ Test"
        - "🤖 Build"
        - "🔁 CI"
        - "📦 Chore"
        - "⏩ Revert"
    validations:
      required: true
  - type: textarea
    attributes:
      label: Current behavior
      description: Is your feature request related to a problem? Please describe.
    validations:
      required: true
  - type: textarea
    attributes:
      label: Suggested solution
      description: Describe the solution you'd like.
  - type: input
    id: context
    attributes:
      label: Additional context
      description: Add any other context about the problem or helpful links here.
  - type: checkboxes
    id: terms
    attributes:
      label: Code of Conduct
      description: By submitting this issue, you agree to follow our [Code of Conduct](https://docs.opensauced.pizza/contributing/code-of-conduct/)
      options:
        - label: I agree to follow this project's Code of Conduct
          required: true
  - type: checkboxes
    id: contribution
    attributes:
      label: Contributing Docs
      description: If you plan on contributing code please read - [Contribution Guide](https://docs.opensauced.pizza/contributing/introduction-to-contributing/)
      options:
        - label: I agree to follow this project's Contribution Docs
          required: false
```

Write your first issue
   - In your repository, click on "Settings" and then "Issues."
   - Set up issue templates for bug reports, feature requests, etc.
   - Add labels to your repository like "good first issue," "enhancement," "bug," etc.



## Promote Your Project
    - Share your project on social media, forums, and relevant communities.
    - Write blog posts or tutorials about your project.
    - Present your project at meetups, conferences, or online webinars.
    - Create a Highlight


## Recognize All Contributions
    - Use tools like the [All Contributors](https://allcontributors.org) bot to acknowledge different types of contributions.
    - Highlight contributors in your README or on your project's website.
    - Thank contributors publicly for their work.

## Start Contributing to Your Own Project
    - Commit your initial code, documentation, or other materials to the repository.
    - Use the same process you've set up for other contributors to model best practices.
    - Regularly contribute to and update the project.

## Monitor
    - Use tools like OpenSauced Insights to monitor the project's activity.
    - Solicit feedback from users and contributors.
    - Reflect on the project's direction and make adjustments as necessary.

Congratulations on creating your first project! Remember, these steps are guidelines; the key to a healthy open source project is to foster an open, inclusive, and collaborative environment.