# Building Your Open Source Dream Team

Managing a project in open source requires clear communication, empathy, and technical understanding. You might find that initially, you can do all or most of the work by yourself. That's great! If you want your project to grow and thrive, cultivating a diverse, motivated, and effective team around you can help you do that. This chapter looks at how to effectively collaborate with your team and offers guidance on identifying, onboarding, and empowering your open source squad.

## Types of Teams

Creating teams on GitHub allows you to grant more permissions to a group of people depending on their team status. Here are some common team types and why a maintainer might find them beneficial:

### Triage Team

Triage teams help to efficiently handle incoming issues and pull requests. A triage team categorizes, prioritizes, and assigns issues to appropriate maintainers or contributors, reducing the maintainer's workload and ensuring timely attention to important matters.

**Benefits**: Faster response to users, improved issue tracking, and better allocation of resources.

### Maintainer Team

The maintainer team shares responsibility for code reviews, bug fixes, and feature development. A team of maintainers with specialized skills can handle larger projects, provide broader expertise, and ensure better code quality and consistency.

**Benefits**: Reduced individual workload, faster development cycles, and more diverse perspectives on code and decisions.

### Documentation (Docs) Team

The docs team creates and maintains high-quality documentation for users and contributors. A dedicated documentation team ensures clear and up-to-date information is readily available, reducing support requests and confusion.

**Benefits**: Improved user experience, easier onboarding for new contributors, and less time spent answering basic questions.

### Other Team Variations

- Security Team
- Design Team
- Community Team
- Marketing Team
- Core Team

?> Sometimes the Maintainer Team and the Core Team are the same. Generally speaking, a Core Team often focuses on broader responsibilities like strategy, governance, and community management, providing insight into the direction of the project. Maintainer Team is more likely to focus on day-to-day management and technical aspects of the project.

## Assembling Your A-Team: Adding New Members

Now that you understand a little bit about teams, let's look at how to identify new members for your team.

### Recognizing the Need

Just like a superhero team expands to face escalating threats, your project might reach a point where additional team members are needed. This could be when the workload starts to overwhelm you (solo maintainer) or your existing team or when you are taking on complex challenges that require specialized expertise. Identifying these challenging points is important for ensuring your project's continued momentum.

### Scouting for Superpowers

Your search for new teammates should be deliberate and thoughtful. Look for contributors who have consistently shown their commitment and skills through active involvement in your project. Their contributions to issues, pull requests, and community discussions can help you determine if they understand the project and your vision. Other things to consider are having enthusiasm, a collaborative spirit, and alignment with your project's goals. Open source projects thrive on passion and shared purpose.

### Inviting Your Team

Once you've identified potential team members, extend a formal invitation. This public acknowledgment of their contributions not only shows your appreciation but also serves as an inspiration to other community members. Platforms like GitHub offer streamlined mechanisms for adding team members, making it a seamless process to officially welcome your new team members.

## Granting Team Permissions

Each team should have a specific set of permissions that allow them to do what they need to succeed. Here are some common permissions that teams might need:

### Repository-Specific Permissions

- **Read**: Allow members to view code, issues, and pull requests. <br/>_Suitable for stakeholders, external collaborators, or those needing general visibility._
- **Triage**: Grant permission to manage issues and pull requests (assign, label, comment, close), but not directly modify code. <br/>_Ideal for triage teams and community managers._
- **Write**: Allow members to push code, create branches, and open pull requests. <br/>_Necessary for developers and maintainers actively contributing to the codebase._
- **Maintain**: Grant broader management permissions, including deleting branches, editing protected files, and managing releases. <br/> _Suitable for core maintainers responsible for project health._
- **Admin**: Provide full control over the repository, including sensitive actions like deleting the repository or changing its visibility. <br/>_Reserved for trusted individuals or those with specific administrative needs._<br/>

To access your team's permissions, navigate to your team's page on GitHub and click on the "Settings" tab. From there, you can update your team's permissions in the "Member privileges" section.

Here's what it will look like in GitHub:

![team permissions](/assets/org-permissions.png)

### Additional Permissions to Consider

- **Project Permissions (if using GitHub Projects)**: Grant access to manage projects, tasks, and milestones within a repository.
- **Organization-Wide Permissions**: For organization-wide teams, consider granting permissions to manage members, billing, security settings, and other organization-level features.

### Best Practices for Team Permissions

- **Start with restrictive permissions**: Grant the minimum permissions necessary for a team to perform its tasks.
- **Review permissions regularly**: As projects evolve and team needs change, revisit permissions to ensure they remain appropriate.
- **Utilize code owners**: Assign specific people or teams as code owners for different parts of the codebase to ensure appropriate oversight and review using the special [CODEOWNERS](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-code-owners) file.

### Specific Examples

- Triage Team: Grant "Triage" permission to the triage team's primary repository.
- Maintainer Team: Grant "Write" or "Maintain" permissions to repositories they actively contribute to.
- Documentation Team: Grant "Write" permission to the documentation repository, potentially "Read" access to other relevant repositories.

You can see some of the options here:

![team permissions](/assets/org-permissions.gif)

## Expanding the Horizons: Enlisting Additional Maintainers

### Specialization: The Key to Scale

As your project grows in complexity, the need for specialized attention in specific areas might arise. Documentation might require someone who can write for audiences at all levels of expertise, while community engagement might need a charismatic presence. Identifying these needs and recruiting contributors with relevant expertise allows you to delegate ownership and ensure all aspects of your project receive the dedicated care they deserve.

### Recruiting Maintainers & Team Members

It is certainly possible that there's no contributor with the right skills and passion to take on a specific role. In those cases, you might need to look outside your existing community. Reach out to other projects or communities that might have individuals with the necessary expertise.

One way to look for potential maintainers is to create an [Insight Page](https://docs.opensauced.pizza/features/insights/) with projects with a similar tech stack. This will allow you to see who is contributing to those projects on a regular basis, their most used languages, and more. From there, you can narrow down your search to individuals who are already familiar with your project's stack and have a proven track record of contributions by adding them to a [List](https://docs.opensauced.pizza/features/lists/). Lists will allow you to see more about where they're contributing, their timezone, their activity level, and more.

#### Creating an Insight Page & List

To track repositories, click the "Insights" tab on the dashboard. You will be redirected to a page where you can create your new Insight Page.

There are two ways to add repositories to your Insight Page:

1. **Sync GitHub organization**. Syncing your GitHub organization is a good idea if you want a unified view of your project activities and the list of contributors to your project.
2. **Add individual repositories**. Adding individual repositories is a good idea if you want to look at similar repositories to recruit team members.

From there, you can create a list of contributors you're interested in learning more about or connecting with by selecting them from the contributors tab and creating a new list.

![team insights gif](/assets/list-from-insight.gif)

## Adding Team Members

Once you've identified potential team members, reach out to them, let them know why you're asking them to become a team member and provide them with a clear understanding of what you expect if they accept the role. This will help them make an informed decision and ensure they can meet your expectations.

To learn how to add them to your team on GitHub, check out [this guide](https://docs.github.com/en/organizations/organizing-members-into-teams/adding-organization-members-to-a-team).

## Onboarding New Team Members

To ensure that your new team members are set up for success, it's important to have an onboarding process. This will help them to understand their responsibilities, the project's goals, and how they can contribute.

Here are some things to consider:

- **Roles & Responsibilities:** Clearly define the team member's role and responsibilities. This will help them to understand what they're responsible for and what they can expect from you.
- **Communication:** Establish clear communication channels and expectations. This will help to ensure that everyone is on the same page and that you're able to communicate effectively.
- **Goals:** Clearly define the project's goals and how the team members can contribute. This will help them to understand how they can contribute to the project's success.
- **Timeline:** Set clear expectations for the timeline. This will help them to understand what they need to do and the deadlines.

One way to onboard your new team members is by having clear guidelines and making it part of your documentation. If you need an idea to create one, you can take a look at the [OpenSauced Community Maintainers Guidelines](https://docs.opensauced.pizza/contributing/opensauced-maintainers-guide/community-maintainers-guide/).

## Keeping Track of Your Team

As your team grows, it's important to keep track of your team's participation and contributions. Depending on how many people are on your team,consider creating a [List](https://docs.opensauced.pizza/features/lists/) to keep track of your team's contributions. This will allow you to see who is contributing to your project and how often and to identify when it's time to remove someone from your team.

![docs team list](/assets/docs-team.gif)

## Saying Farewell: Handling Team Departures

As time goes on and people's lives change, you'll find that even the most dedicated teams might face departures. Inactivity, discord with project values, or mutual agreement can lead to changes in your team. It's important to approach these situations with respect and understanding. Privately communicate the reasons behind the decision, acknowledge the individual's contributions, and express gratitude for their time and effort. Remember, fostering a positive and supportive environment, even during departures, contributes to the overall well-being of your project community.

To remove the person from your team in GitHub, check out [this guide](https://docs.github.com/en/organizations/organizing-members-into-teams/removing-organization-members-from-a-team).

## Conclusion

Remember, the team is there to support you and the project and to help you achieve your goals. As you grow your team, keep in mind that you're not just adding people to your project; you're adding people to your community. Make sure that you're adding people who are aligned with your project's values and goals and who will be a positive addition to your community.