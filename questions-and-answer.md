---
question: In Scrum, should tasks such as development environment set-up and capability development be managed as subtasks within actual user stories ?
[link](https://softwareengineering.stackexchange.com/questions/134664/in-scrum-should-tasks-such-as-development-environment-set-up-and-capability-dev)
---

Sometimes in projects we need to spend time on tasks such as:

1. exploring alternate frameworks and tools
2. learning the framework and tools selected for the project
3. setting up the servers and project infrastructure (version control, build environments, databases, etc)

If we are using User Stories, where should all this work go?

One option is to make them all part of first user story (e.g. make the homepage for application). Another option is to do a spike for these tasks. A third option is to make task part of an [Issue/Impediment](http://msdn.microsoft.com/en-us/library/ff731580.aspx) (e.g. development environment not selected yet) rather than a user Story.

# Answers

We thought about this problem quite a lot in the past year.

While I agree that a basic framework should exist before the project starts, in practical use it can be part of the project itself. So you have to manage somehow.

While mixing project setup with user stories might make sense sometimes we have settled on simple **tasks** that can be added to the product backlog and get the same attention as user stories. We know that these technical tasks are necessary sometimes, but they have to be justified in any case. If the team thinks that they are absolutely necessary to achieve a certain goal, they will be part of a sprint.

It's hard to say what works best for you, so **experiment**! A spike might suffice for now, but I think you'll end up with the same problem later, so plan ahead. Do tasks that are a placeholder for such activities. To separate tasks from stories two I will quickly compare them based on my experience with them.

**Task**: A task is a technical necessity. It might be things for configuration management or general project setup, like setting up a repository for commits, or adding the hottest code review tool you have ever seen to the development process. Tasks should be considered in planning, same as a user story. If the team can convince the product owner that having the latest and greatest code review tool increases performance and ups team communication by eliminating long lasting pair programming sessions or in-person code reviews, then it will get the product owner's attention.

**Stories**: Focused on business perspective only, stories always produce visible value to the customer. Internal quality is something that goes along with producing business value.

We even assign story points to tasks and sometimes work with them the same we would do with stories.

In the end I would go for this solution in your case (which could be applied in general as well):

1. Separate "setup" and technical stuff into tasks (stuff that does not directly produce business value for the product owner).
2. Maybe do a spike prior to project setup to get the most important tools into place (SCM, dev tools, process defintion, coding standards etc.)
3. Accept that these tasks pop up over the duration of the project and plan for this by having a separate "type" of activities other than stories.
