# How to Contribute to Open Source

In this chapter, we'll guide you through the process of contributing to open source projects.

## Finding Projects to Work On

One of the first challenges you might face when getting started with open source is finding a project to contribute to. Here are some tips to help you discover projects that align with your interests and skills:

1. **Browse GitHub and GitLab**: Both GitHub and GitLab host a vast number of open source projects. You can use their search functionality to find projects based on specific keywords, programming languages, or topics.

2. **Follow your interests**: Think about the tools, frameworks, and libraries you use or are interested in learning more about. Many of these projects are open source and welcome contributions from the community.

3. **Join open source communities**: There are numerous online communities, forums, and chat platforms dedicated to open source development. By joining these communities, you can connect with other developers, discover new projects, and find collaboration opportunities. In the [OpenSauced Discord](https://discord.com/invite/U2peSNf23P), for example, we share good first issues, cool GitHub projects, and issues we have open on our repositories.

4. **Leverage OpenSauced**: [OpenSauced](https://opensauced.pizza/) is a platform that helps developers discover and contribute to open source projects. By using OpenSauced, you can find projects that align with your interests, skills, and goals.

### Discovering Open Source with OpenSauced

OpenSauced is a powerful tool for finding open source projects to contribute to. To get started with OpenSauced, follow these steps:

1. **Sign up for an account**: Visit https://www.opensauced.pizza/ and sign up for an account using your GitHub credentials.

   ![Image](./images/opensauced-signup.png)

   During the signup process, you'll be asked to pick some interests and set your timezone. This will help OpenSauced recommend projects that align with your interests and schedule.

2. **Explore the dashboard**: Once you've signed up, you'll be taken to your dashboard, where you can view your current projects, goals, and contributions. Clicking "Explore" in the header will enable you to browse projects based on your interests and skills.

3. **Search for projects**: In Explore, you can see a list of repositories and their relevant activity levels and engagement levels that are currently trending. You can also search for projects by typing in the search bar. You can search for projects by name, description, or topic and use this tool to find something that resonates with you.

   ![Explore](./images/opensauced-explore.png)

4. **Save projects to your Insights pages**: When you find projects you're interested in, you can add them to "Insights" pages that give you more details about the activity over the projects. Or, if you'd rather just dive in and contribute, you can skip to the next step.

5. **Start contributing**: When you click on the name of a repository, you'll be taken to its GitHub page, where you can explore issues that are open and ready for contribution, knowing that the community around this project is active and your contributions will be welcomed.

By using OpenSauced, you can streamline the process of finding open source projects to work on and focus on contributing to the projects that align with your interests and goals.

## Onboarding in a New Project

When you're interested in contributing to a new open source project, it's important to familiarize yourself with the project's guidelines, conventions, and workflow and take the initiative to onboard yourself.

Here are some tips to help you onboard successfully:

1. **Read the project's documentation**: Read the README file, Contributing Guidelines, and Code of Conduct to familiarize yourself with the project. This will help you understand the project's goals, requirements, and expectations for contributors.

2. **Start small**: When you're new to a project, it's a good idea to start with small, manageable tasks, such as fixing bugs, adding tests, or updating documentation. This will help you become familiar with the codebase and development workflow without getting overwhelmed.

3. **Join the community**: Many open source projects have online communities, forums, or chat platforms where developers can ask questions, share knowledge, and collaborate. By joining these communities, you can connect with other contributors, learn from their experiences, and get help with any issues you encounter.

4. **Ask for help**: If you need clarification or encounter a problem, don't hesitate to ask for help. Open source communities are generally supportive and welcoming; other contributors will gladly assist you.

5. **Be patient and persistent**: Onboarding in a new project can be challenging, especially if you're new to open source development. Be patient, and don't be discouraged by setbacks or mistakes. You'll become more comfortable and confident in your contributions with persistence and practice.

## Getting Started With Contributing

So, you've onboarded yourself in the project. Now, you can prepare to contribute by following these steps:

1. **Read the Contributing Guidelines**: Investigate how the project receives contributions by reading the CONTRIBUTING file. You want to ensure that you follow the project's contributing rules.

2. **Find or create an issue**: Look for issues labeled as "good first issue" or "beginner-friendly" that are suitable for your skill level. Alternatively, identify a feature or improvement you'd like to work on. Check if it aligns with the project's roadmap and create an issue. This could include documentation updates, bug fixes, content changes, and more.

3. **Ask to be assigned the issue**: When making your first contribution to a project, it's a good idea to ask the maintainers to assign the issue to you. This will ensure that you're not duplicating work and that your contribution is aligned with the project's goals and requirements.

   If there are no directions in the CONTRIBUTING file, you can leave a comment on the issue, "Can I please be assigned this issue?" When the maintainer has assigned you, you'll notice that your username is now under the "Assignees" section.

   ![issue assigned screenshot](./images/issue-assign.png)

## Contribution Workflow

Once a maintainer has assigned you an issue, the next step is to work on the changes. Here's a general workflow of the process:

1. **[Fork the repository](https://docs.github.com/en/get-started/quickstart/fork-a-repo#forking-a-repository)**: Forking a repository means creating a copy of the repository under your GitHub account. It allows you to push changes to the remote codebase without affecting the original project.

2. **[Clone your forked repository](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository#cloning-a-repository)**: Make a copy of your forked repository to your local machine. Run the following command in your terminal:

   ```
   git clone https://github.com/YOUR-USERNAME/REPOSITORY-NAME.git
   ```

   Replace "YOUR-USERNAME" with your GitHub username and "REPOSITORY-NAME" with the repository's name.

3. **Create a new branch**: Before making any changes, create a new branch in your local repository to work on your contribution. Creating a new branch is the best practice in open source because it keeps your changes separate from the `main` branch.

   You can create a new branch using the following command:

   ```
   git checkout -b YOUR-BRANCH-NAME
   ```

   Replace "YOUR-BRANCH-NAME" with a descriptive name for your branch, such as "fix-bug-123" or "add-new-feature".

4. **Make your changes**: Now that you have a new branch, you can make changes to the codebase. Always follow the project's coding guidelines and conventions, and test your changes to ensure they work as expected.

5. **Add and commit your changes**: Once you've made your changes, add your changes to the staging area and commit them with these commands:

   ```
   git add .
   git commit -m "Your commit message"
   ```

   Replace `"Your commit message"` with a brief description of your changes.

6. **Push your changes**: Push your changes to your forked repository on GitHub by running the following command:

   ```
   git push origin YOUR-BRANCH-NAME
   ```

   Replace "YOUR-BRANCH-NAME" with the name of your branch.

7. **[Create a pull request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request-from-a-fork)**: Once you've pushed your changes, navigate to the original project's repository on GitHub and click the "Compare & pull request" button. Fill in the required information and submit your pull request by clicking the "Create pull request" button.

8. **Respond to feedback**: After submitting your pull request, the project maintainers may provide feedback or request changes. Be sure to respond promptly and address any concerns or suggestions they may have.

By following these steps, you'll be able to submit your contributions to open source projects and collaborate with other developers to improve the codebase.

## What Happens Next?

After your contribution has been submitted and reviewed, one of the following outcomes may occur:

1. **Your contribution is accepted**: If your contribution is approved by the project maintainers, it will be merged into the main branch of the codebase. <br>
   Congratulations! Your work is now part of the project, and you've made a valuable contribution to the open source community.

2. **Your contribution requires changes**: Sometimes, the project maintainers may request changes to your contribution before it can be accepted. This could be due to coding issues, conflicts with other changes, or a need for additional documentation. In this case, make the requested changes and resubmit your pull request.

3. **Your contribution is rejected**: In some cases, your contribution may not align with the project's goals or requirements, or it may not be the best solution to a problem. If your contribution is rejected, don't be discouraged. Take the feedback you received as an opportunity to learn and improve. You can always try contributing to another project or submitting a different contribution to the same project.

## Let's Get Practical

Now that you know how to find and contribute to open source projects, it's time to put your skills into practice. Let's do this by contributing to OpenSauced's [guestbook repository](https://github.com/open-sauced/guestbook).

### Prerequisite

You'll need to have these tools donwloaded and installed on your local machine:

- [Node.js](https://nodejs.org)
- [Visual Studio Code (VS Code)](https://code.visualstudio.com/)

### Getting Started

1. Create an issue by clicking the "New issue" button in the "Issues" tab and complete the form.
2. Fork the [guestbook repository](https://github.com/open-sauced/guestbook).
3. Clone your forked repository to your computer.
4. Run `npm install` to install the dependencies.
5. Create a new branch and use a descriptive name related to your contribution — for example, `feat/add-alice`.
6. Add yourself to the guestbook.

   There are two ways you can complete this activity:

   - Using the CLI tool.
   - Manually editing the `.all-contributorsrc` file.

   Although adding yourself to the guestbook with the CLI tool is simpler, we recommend manually editing the file to get more experience adding and committing your changes, creating pull requests, and pull request reviews. Below, you'll find the directions for each method:

   **CLI Tool**

   - Run `npm run contributors:add` in your terminal.

     Follow the instructions to add yourself to the guestbook. After you finish and click enter, you must click enter again to confirm your choices.

   **Manual Addition**

   - Open the `.all-contributorsrc` file.
   - Go to the last contributor in the contributors' array.
   - Add a comma after the last closing curly bracket ( `},` ).
   - Copy and paste the template below:

     ```javascript
     {
        "login": "",
        "name": "",
        "avatar_url": "",
        "profile": "",
        "contributions": []
     }
     ```

   - Add yourself manually to the guestbook by updating this information:

     - **login**: Your GitHub's username.
     - **name**: Your name.
     - **avatar_url**: URL to your avatar on GitHub.

       In your browser, copy and paste the link of your GitHub profile, append `.png` at the end (for example, `https://github.com/USER_NAME.png`), and click enter. Copy and paste the link here.

     - **profile**: Link to your website (if you include it in your GitHub profile) **or** your GitHub profile.
     - **contribution**: Type of your contributions.

       Refer to the types (in the first column) in this [emoji key and contribution types](https://allcontributors.org/docs/en/emoji-key) to fill in the values.

       !> You have to strictly use the types in the list to avoid breaking the whole project.

       The result would be like this:

       ```javascript
       {
         "login": "github-username",
         "name": "User Name",
         "avatar_url": "https://avatars.githubusercontent.com/u/xxxxxxxx?v=x",
         "profile": "URL link",
         "contributions": [
            "question",
            "blog",
            "code"
         ]
       }
       ```

       > ⚠️ **Remember to add a comma after the quotes, except for the last one in the array and the last closing curly bracket.**

7. Run `npm run contributors:generate` in your terminal to generate the guestbook on the README.
8. Copy and paste the Markdown of the README in [Markdown Live Preview](https://markdownlivepreview.com/) and take a screenshot of your profile being generated. You will need this later when creating a pull request.

   ?> If you don't see your profile in the "Contributors" section, zoom out the screen until you can see it before taking a screenshot.

9. If you used the CLI tool method in step 5 to add yourself to the guestbook, **skip this step**. Otherwise:

   Add and commit your changes by running the following command:

   ```bash
   git commit -am "Your commit message"
   ```

   Replace `"Your commit message"` to your own message. For example, `"Add Alice as a contributor"`.

   !> Unlike the `git add .` and `git commit -m "Your message"` approach, in the `git commit -am` command, adding `-a` flag to `git commit` skips the staging process. The `-a` flag automatically stages all your changes in _committed_ files. Combining it with the `-m` flag allows you to write the commit message.

10. Run `git log` to check if you have committed your changes. Press `Q` to close the log.

If you add yourself using the CLI tool, it automatically adds and commits your changes. So you will see this automated commit message:

```bash
docs: add @your_username as a contributor
```

11. Push the commit to your forked repository with this command:

```bash
git push -u origin branch-name
```

12. Go to your forked repository on GitHub and create a pull request with the title `feat: Add <@github-username> as a contributor`.

Congratulations on your first contribution! 🎉

## Keeping Branches Up to Date

It is highly recommended that you update your remote and local branches habitually. That way, your branch will have the latest update when merged into the `main` branch of the original (`upstream`) repository.

The best times to update your branches are before you push your changes to the remote repository and while you're waiting for your pull request to be reviewed.

### Updating Branches

First, you must update your forked (`origin`) repository:

1. Go to your forked repository on GitHub.
2. Click the "Sync fork" button.
3. Click the green "Update branch" button.

Then, pull the latest changes in the `main` branch in the `origin` repository to update your local working branch by following these steps in your terminal:

1. Go to your working branch.

   ```bash
   git checkout YOUR-BRANCH-NAME
   ```

2. Pull the latest changes with this command:

   ```bash
   git pull origin main
   ```

## Merge Conflicts

Merge conflicts are something you'll commonly encounter when contributing to an open source project. When two branches have made different changes to the same line(s) in the same file(s), Git cannot automatically determine which change to keep, resulting in a conflict.

When a merge conflict occurs, Git adds conflict markers (`<<<<<<<`, `=======`, and `>>>>>>`) to indicate the conflicting lines from different branches. Everything between the `<<<<<<<` and `=======` is the changes that you worked on (current changes). And everything between the `=======` to `>>>>>>>` is the incoming changes from the remote `main` branch.

You need to pay attention to the conflicts and decide how you want to resolve them. You can keep only your change, incoming change, or both changes.

### Tips to Prevent Resolving Merge Conflicts Repeatedly

Some open source repositories, such as OpenSauced's [guestbook](https://github.com/open-sauced/guestbook) and [pizza verse](https://github.com/open-sauced/pizza-verse) repositories, have high contribution activities in the same files that can cause merge conflicts.

Below are some tips to prevent you from resolving merge conflicts repeatedly when contributing to open source projects:

#### 1. Following Instructions

Ensure you follow the instructions in the project's README or Contributing Guide, and don't miss any step.

#### 2. Pull Request Form

Complete the template form and fill in all areas when creating a pull request.

If a repository doesn't provide you with a pull request template, you need to have these in your pull request form:

- **A descriptive title**: A descriptive title would help maintainers and other contributors gain an idea of what your contribution is. <br>
  Consider using the following method to write your title: `type: brief description of your contribution`. For example, `fix: color contrast issue on the navbar`, `feat: create a warning button`, etc.

- **A clear description of your pull request**: Describe your pull request clearly. Consider explaining your changes, thoughts behind the solution, etc. A clear description gives maintainers and other contributors insight into the details of your changes. Here is [an example of a clear description in a pull request](https://github.com/open-sauced/intro/pull/10).

- **The [link to the related issue](https://docs.github.com/en/issues/tracking-your-work-with-issues/linking-a-pull-request-to-an-issue)**: Linking a pull request to the addressed issue will close the linked issue automatically when the pull request gets merged. This makes it easier for maintainers to keep their projects organized.

- **A screenshot or screen recording when you make a UI change**: Providing screenshots or screen recordings will make it easier for maintenance to visualize your changes and review your pull request.

#### 3. Resolving Merge Conflicts Immediately

If a branch has merge conflicts that must be resolved, the merge button is automatically disabled. So, maintainers are not able to merge the pull request.

When you notice merge conflicts in your pull request or if a maintainer asks you to resolve merge conflicts, fix them immediately. The sooner you resolve the conflicts, the sooner maintainers can review and merge your pull request.

### Merge Conflicts in the Guestbook Repository

Since the primary purpose of the guestbook is to add your name to `.all-contributorsrc` and the `README.md` files, there is a high chance that you will encounter merge conflicts.

The conflicts happen when maintainers have merged pull requests before yours while you're working on your changes or waiting for your pull request to be reviewed. And you need to resolve them before your pull request can be merged.

#### Resolving Merge Conflicts

Before resolving merge conflicts, you must first [update your branches](#updating-branches). Then, follow these steps:

1. In the `.all-contributorsrc` file:

   - Click the "Accept Both Change" option on the top of your workspace in VS Code.
   - Move your profile details to the end of the contributors' array and fix anything necessary.

2. In the `README.md` file:

   - Click the "Accept Incoming Change" option on the top of your workspace in VS Code for each conflict in this file.

3. Run `npm run contributors:generate`.

   You will now see that the all contributors badge has been incremented, and your profile is generated at the end of the contributors' list in the `README.md` file.

4. Add and commit your changes.

   ```bash
   git commit -am "Resolve merge conflicts"
   ```

5. Push your commits to your remote branch.

   ```bash
   git push
   ```

<hr>

As you continue to contribute to open source projects, you'll gain valuable experience, develop new skills, and build a strong portfolio of work. In the next chapter, we'll discuss some strategies for getting started with open source contributions, gaining traction in your contributions, and developing your open source resume using OpenSauced.

<!-- [Next Section ->](../intro-oss/06-the-secret-sauce.md) -->

<a href="https://github.com/open-sauced/intro/blob/main/05-how-to-contribute-to-open-source.md">
  ✏️  Edit this page
  </a>
