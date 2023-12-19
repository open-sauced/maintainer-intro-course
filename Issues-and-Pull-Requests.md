# How to handle open issues and pull requests

One of the core responsibilities for an open source maintainer is going through the open issues and pull requests. In this section, we will talk about how to best handle open issues, pull requests and security vulnerabilities.

## How to Efficiently Manage and Triage Issues

Issue triage involves going through an existing list of open issues and prioritizing them in order of importance. In this next section we will break down the most common types of issues and how to best triage and respond to contributors.

### How to Triage Issues Labeled as Bug Fixes

Some open issues will be critical bug fixes and should be seen as high priority. In these situations, it is best to label these issues with a `bug`, `critical`, or `high-priority` label so the team knows to address those issues first. You should also think about the types of colors to use for the labels. Using bright red or orange label colors is a good choice because it indicates the level of seriousness and is easier to spot in a list of issues.

Also, for critical bug fixes, it is best to have core team members or contributors work on these issues to ensure that it is done well and in a timely manner. In these situations, you might consider using a label like `core team work` to indicate that this issue is only open for select members.

For small bug fixes that aren't considered critical, you can open these issues up for anyone to work on. Some of these issues might be small enough that it would be a good opportunity for a new contributor. In this situation, you should label the issue with a `good first issue` or `first timers only` label.

If you are unable to reproduce the bug, then reach out to other teams member to see if they are able to reproduce it on their end. If you are a solo maintainer, then reply back to the original poster of the issue to gain more information and context on the issue.

### How to Triage Issues Labeled as Feature Requests

When triaging feature requests, you want to make sure that it is a good fit for your project. If you are interested in adding that feature, reach out to the original poster of the issue to see if they are interested in working on it. If they are interested, go ahead and assign that issue to them. Otherwise, add a `help wanted` or `accepting PRs` label on it.

If the feature sounds like a good fit for the project, but is complex in nature, you might consider working on it yourself or having a core team member assigned to it. Large features that affect many files and moving parts in your application, should be handled by someone that is very experienced with the codebase and won't create more issues.

Sometimes users will ask for features that are already on the roadmap or in progress by another contributor. If that is the case, then politely respond back to them to let them know it is already being worked on. Here is a template that you can use for a response:

> Thank you for taking the time to open this issue. This feature is currently in the works by another team member and will be added soon. As a result, we are going to close this issue.

If a feature request does not sound like a good fit for your project, then respond back to the original poster and close the issue. Here is a template that you can use for a response:

> Thank you for your interest in our project. The feature you have proposed would not be a good fit for the current scope and direction of this project. At this time, we will not be moving forward with this feature.

### How to Triage Documentation Issues

If the issue has to deal with small typos or grammar mistakes, then add a `good first issue` label on it to open it up for new contributors. If the issue is more involved, then you will need to evaluate the level of priority and add a `help wanted` label on it. Also, in these situations you might need to get more information from the original poster before opening it up for contribution.

### How to Deal with Spam Issues

If an issue is clearly a spam or unhelpful message, then do not bother to engage with the poster. Instead, close the issue and add a `spam` label. Here is an example of a spam message:

> This project is terrible! Nothing works, and your code is garbage. I can't believe anyone would use this. Fix it ASAP!!!111!!1!

In that situation, there are no concrete details on the issues and the poster is clearly combative. It is important not to engage with these types of users, but instead just close the issue and move on.

### How to Deal with Issues with Insufficient Information

If the user does not provide concrete details in the issue, then kindly respond back asking them for more information. If it is a bug report, ask for more details on how to reproduce the bug. If it is a feature request, ask for clarification on style or functionality changes.

Some users will be quick to respond back to replies, while others might take longer to reply. If you don't hear a response back within a week, feel free to message them again for more details. If a few weeks passes and the issue is not deemed as critical, go ahead and close the issue.

### How to Deal with Stale Issues

For issues that haven't been worked on for months are considered stale. Sometimes you might be interested in resurrecting this issue and making it a higher priority item. If that is the case, then go through the normal triage process and add the appropriate labels to it.

But other times, you might realize this is an issue that will not be worked on. If that is the case, go ahead and close it for good. Some maintainers will choose to automate this process by using a GitHub action bot like this [one](https://github.com/actions/stale).

## How to Review Pull Requests

There are many things to consider when reviewing pull requests. In this next section we are going to talk about how to provide good feedback and work with contributors on their pull requests.

### How to Provide Good Code Reviews

Good code reviews should be informative, constructive and helpful for both the reviewer and author. Remember that contributors have volunteered their time to help your project. So you want to make sure your review is generally a positive and informative one. You should consider using phrases like this:

> "Let's using more descriptive variable names for better readability. Instead of variable d here let's go with days_until_deadline".

While it is important to provide detailed reviews, you want to make sure to specify which changes are absolute fixes versus which ones are suggestions and nitpicks. If something is broken or hard to read/understand, then that should be something fixed in the pull request. You consider saying something like the following:

> "This is a breaking change and was should change it to be this instead."

If your suggested changes are minor suggestions/nitpicks, then make sure to indicate that in your review. That let's the author decide if they want to incorporate those changes in their pull request or not.

### How to Manually Test Pull Requests

If a pull request involves a small change to documentation or code, then there usually is no need to manually test the changes. But if the pull request involves significant changes to the project, it is best to test the changes yourself to ensure that every is working properly.

If you have deploy previews setup through a service like [Netlify](https://docs.netlify.com/site-deploys/deploy-previews/) or [Vercel](https://vercel.com/docs/deployments/preview-deployments), that is a good first step to manually testing the changes. If you don't have previews setup, then you should pull down the project locally to manually test the changes. The reason why it is important to take your time to manually test everything is because you are the last line of defense before a pull request is merged in. Without the proper testing, a new set of changes can break the application.

If the pull request has broken a part of the application, then respond back to the author with detailed account of what went wrong. Sometimes, it helps to include a screenshot and/or recording of what is broken. If your automated tests did not catch the breaking change, then you should open up a separate issue to update your test suite. If you don't have a test suite setup to run on every pull request, then this is a good time to set that up.

### How to Deal with Pull Requests Missing Tests

Not all pull requests will need tests because they are small code changes or updates to documentation. But for larger features or refactors, there should be tests added to help ensure that everything is working as expected. If the pull request author has not setup tests, reach out to them on the PR to let them know what parts need to be tested. It would also be good to make sure this is outlined in your documentation that this is an expectation.

### How to Deal with Spam Pull Requests

There might be times where you will get a spam PR for your project. In these situations, it is best not to respond to the author, but instead close the PR and add a `spam` label on it.

Here are some examples of spam PR's:

- whitespace changes to `README` or other files
- random changes to files without an accompanying issue or explanation
- numerous links to unrelated websites or promotes products/services
- plagiarized content from other sources without permission or proper attribution

### How to Deal with Low Quality PR's

Low quality pull requests unfortunately take a lot of time and energy from the maintainer. Here are a few examples of low quality pull requests:

- pull requests that are incomplete and do not address the entire issue
- pull requests that lack proper documentation of the changes made
- code that does not fit within the established style guide for the project
- incomplete pull request templates that do not provide sufficient information on what changes where made
- pull requests that address multiple issues at once and make it difficult to review

If you receive a pull request that is lower in quality, reach out to the author explaining what is missing and what changes need to be made. A lot of the time contributors might not be aware of these issues and just need to extra explanation and time to improve their PR.

### How to Deal with Failing Automated Tests

Sometimes contributors will open a pull request that fails a few of your automated tests. It is best to wait a few days after the PR is opened to give the contributor a chance to address the failing tests and resolve the issue on their own. If it looks like they are not addressing the issue, reach out to them on the PR and ask if they need help. If they need help, look into why the test is failing and provide constructive feedback on how they can fix it. If the test is failing unrelated to their changes, then let them know that it is safe to ignore it and will be fixed in another PR.

If the author does not address the issue and does not respond back to your initial reply then reply back with suggested fixes and reiterate that you are here to help. If several weeks or months have passed without a response from the author, then close the PR and move on.

If multiple contributors are failing the same set of tests, then this possible that the tests are flaky or broken and need your attention. In those situations, you want to make it clear to contributor that the failing test is not their fault and will be resolved.

### How to Deal With Stale Pull Requests

Sometimes pull requests can be remain open for weeks or months at a time. If the PR has regular updates and conversations, that is not considered a stale PR. If there has been little to no active for several weeks, then you will need to reach out to the contributor to see if they need help or are still interested in working on it.

If you have tried repeatedly to reach out and get no response, then you should either close the PR or take it over. If you are taking it over, then communicate to them that you are bringing this to the finish line because it is blocking other PRs.

## How to Highlight an Issue or PR with OpenSauced

The [Highlights feature](https://docs.opensauced.pizza/features/highlights/) on OpenSauced is a place for you to showcase recent achievements with the open source community. This is a place to introduce your project to potential new contributors and talk about issues that need attention from the community.

### Issue Highlights

When writing issue highlights, you will want to talk about the issue, how the contributor solved it, and the impact that the solution had on the project. Once you post a highlight on OpenSauced, make sure to re share it on other platforms like Twitter or LinkedIn for increased visibility. Regularly acknowledging and thanking your contributors publicly will strengthen their loyalty to the project and attract new contributors.

### PR Highlights

When writing PR highlights, you will want to talk about the changes made in the PR, acknowledge the PR author and showcase how this is an improvement on the project. It would also be good to link to the actual PR for those interested in looking at the changes made. This is another way to gain attention for the project, because it is a first hand look at what types of contributions you are looking for and how well you work with contributors.

To learn more about how the Highlights feature works, please read through the [OpenSauced documentation](https://docs.opensauced.pizza/features/highlights/).

## How to Provide Prompt Responses and Address Concerns

When you have incoming issues and pull requests it is important to schedule time for triage and reviews. Design a regular schedule that works for you so you have during the week to work with contributor issues and provide detailed pull request reviews.

You should not feel pressured to immediately respond to new open issues or pull requests. It is fine if they are left unread for a few days. If a contributor is pushing you for a review or issue comment, politely respond back that you will get to it when you have time. You can also setup your own [GitHub action](https://dev.to/opensauced/github-actions-a-maintainers-best-friend-488n) to automate responses to new issues and PR's letting contributors know you will get to it when available.

If contributors have concerns about the project, then you will want to create a safe space to make them comfortable talking about these issues. If they have concerns about the code or security aspects, feel free to discuss it on an open issue or even privately through Discord or Slack.

## How to Prioritize Tasks and Setting Realistic Timelines

Sometimes it can be difficult to juggle all of the tasks required for maintaining an open source project. You will want to set aside time each week to triage issues and look through the project backlog to prioritize work to be done. You shouldn't feel pressured to label each issue and pull request a high priority. Realistically, there will always be a set of issues that are truly considered top priority while the rest can be addressed at a later time.

When it comes to setting realistic timelines, make sure you add an extra few days to your estimate of work. So if you think that a new set of features will take a couple of weeks, tack on an each week. Issues come up all of the time in projects. So you don't want to timebox yourself to a very strict deadline when it probably wasn't realistic in the first place.

When you are working with other volunteer contributors, allot for extra time to get the work done. If they are volunteering their time, they will probably run into other commitments which will delay their availability for you. It is important to lead with empathy and understanding and not demand that they adhere to a strict deadline like an employee would.

## How to Handle Security Vulnerabilities Responsibly

In case security issues arise within your project, it's essential that your contributors are aware of the optimal methods for reporting them. You should have a `SECURITY.md` file which is a policy for reporting security vulnerabilities. This file is usually located in the root directory or `.github` directory of your project. It would also be good to link to the security file in your `README` for easier access by the community.

A lot of maintainers will choose to go with this template `SECURITY.md` policy.

> GitHub's [Bug Bounty program](https://bounty.github.com) rewards researchers for discovering security vulnerabilities in a number of repositories. The full list of projects that are eligible for rewards are [available on our Bug Bounty site](https://bounty.github.com/#scope).

> If the repository is eligible for rewards, you can submit a report via [HackerOne](https://hackerone.com/github). You can find more useful information in our [rules](https://bounty.github.com/#rules) and [FAQ](https://bounty.github.com/#faqs).

> For repositories not covered by the Bug Bounty program, please open an issue.

### Adding Dependabot to Your Project

Dependabot is a GitHub feature that will monitor your project's dependencies and report any possible security vulnerabilities found. You can configure dependabot to report issues or even create pull requests to update dependencies with security vulnerabilities. To learn more about this feature, please read through the [GitHub documentation](https://docs.github.com/en/code-security/getting-started/dependabot-quickstart-guide).

### Configuring Code Scanning Tools

There are plenty of third party tools that you can integrate into your project to scan your codebase and identity potential security vulnerabilities. GitHub has a automated tool called CodeQL that will run frequent security checks in your codebase. To learn more about code scanning tools, please read through the [GitHub documentation](https://docs.github.com/en/code-security/code-scanning/introduction-to-code-scanning/about-code-scanning-with-codeql).
