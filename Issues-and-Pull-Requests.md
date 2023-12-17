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

If the feature sounds like a good fit for the project, but is complex in nature, you might consider working on it yourself or having a core team member assigned to it. Large features that affect many files and moving parts in your application, should be handled by someone that is very experienced with the codebase and won't create more issues in the codebase.

Sometimes users will ask for features that are already on the roadmap or in progress by another contributor. If that is the case, then politely respond back to them to let them know it is already being worked on. Here is a template that you can use for a response:

> Thank you for taking the time to open this issue. This feature is currently in the works by another team member and will be added soon. As a result, we are going to close this issue.

If a feature request does not sound like a good fit for your project, then respond back to the original poster and close the issue. Here is a template that you can use for a response:

> Thank you for your interest in our project. The feature you have proposed would not be a good fit for the current scope and direction of this project. As this time, we will not be moving forward with this feature.

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

For issues that haven't been worked on for months are considered stale. Sometimes you might be interested in resurrecting this issue and consider a higher priority item then before. If that is the case, then go through the normal triage process and add the appropriate labels to it.

But other times, you might realize this is an issue that will not be worked on. If that is the case, go ahead and close it for good. Some maintainers will choose to automate this process by using a GitHub action bot like this [one](https://github.com/actions/stale).

## How to Review Pull Requests

### How to Deal with Spam Pull Requests

### How to Deal with Failing Tests

### How to Deal with Missing information in the Pull Request Body

## How to Highlight an Issue or PR with OpenSauced

## How to Provide Prompt Responses and Address Concerns

## How to Prioritize Tasks and Setting Realistic Timelines

## How to Handle Security Vulnerabilities Responsibly
