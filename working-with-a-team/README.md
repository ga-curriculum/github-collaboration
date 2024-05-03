# ![GitHub Collaboration - Working with a Team](./assets/hero.png)

**Learning objective:** By the end of this lesson, students will be able to describe best practices to work well as a team.

There are many, many, many ways to collaborate with other using Git and GitHub. We are going to focus on just two workflows:

- **Forking and Cloning** - This is the most common way to collaborate with others. You fork a repository, clone it to your local machine, make changes, and then create a pull request to merge your changes back into the main codebase.
- **Collaborators** - This is a more advanced way to collaborate with others. You add collaborators to a repository, they clone the repository to their local machine, make changes, and then create a pull request to merge your changes back into the main codebase.

## Forking and Cloning Git Workflow

Collaborating with others using the forking and cloning workflow is the most common way to work with others. This workflow is used when you want to contribute to a project that you do not have write access to. This is common when working on open source projects or contributing to a project that is maintained by someone else. Let's dive into the forking and cloning workflow.

- **Choose a repository creator:** The repository creator is the person who will be responsible for merging changes back into the main codebase. This person is typically the project lead.
- **Everyone forks the repository:** Each team member will fork the repository to their GitHub account. This creates a copy of the repository on their account.
- **Clone the repository:** Each team member will clone the repository to their local machine. This downloads the repository to their local machine.
- **Create a new branch:** Each team member will create a new branch to work on a new feature or bug fix.
- **Make changes:** Each team member will make changes to the codebase complete the feature or bug fix.
- **Push the branch to GitHub:** Each team member will push the branch to their GitHub account.
- **Create a pull request:** Each team member will create a pull request to merge their changes back into the main codebase.
- **Review and merge:** Using the GitHub website, the repository creator will lead the team in a review of all pull requests. Once the changes have been reviewed, the repository creator will merge the changes back into the main codebase.
- **Pull changes:** Each team member will pull the changes from the main codebase to their local machine.

This can be a lot to take in and a lot to execute. Refer back in this module for more detailed instructions on each step.

## 🎓 You do: Forking and Cloning Git Workflow

In your teams, follow the forking and cloning workflow. Complete the following tasks:

- Choose a repository creator and have them create a new repository on GitHub.
- When the team gets to the steps **Make Changes** everyone should add a new file called `team.md` to the repository. On the first line of this file put your name. (Every first line of `team.md` should be a different name.)
- Refer back to [Resolving Merge Conflicts Remotely](./merging-and-merge-conflicts/README.md) for instructions on how to resolve merge conflicts.

At the end of this exercise, you should have a new file called `team.md` in the repository with everyone's name in it.

## Collaborators Git Workflow

Collaborating with others using the collaborators workflow is a more advanced way to work with others. This workflow is used when you want to contribute to a project that you have write access to. This is common when working on a project that is maintained by a team of developers. The workflow is similar to the forking and cloning workflow, but with a key difference: **you do not fork the repository**. You will still need a repository creator however they will add you as a collaborator to the repository giving you the same access as the repository creator. Let's dive into the collaborators workflow.

- **Choose a repository creator:** The repository creator is the person who will be responsible for merging changes back into the main codebase. This person is typically the project lead.
- **Add collaborators:** The repository creator will add collaborators to the repository. This gives the collaborators write access to the repository.
  - **Adding a collaborator:** Navigate to the repository on GitHub. Click on `Settings` then `Manage access`. Click on the `Invite a collaborator` button and search for the collaborator you want to add.
- **Clone the repository:** Each team member will clone the repository to their local machine. This downloads the repository to their local machine.
- **Create a new branch:** Each team member will create a new branch to work on a new feature or bug fix.
- **Make changes:** Each team member will make changes to the codebase complete the feature or bug fix.
- **Push the branch to GitHub:** Each team member will push the branch to the repository.
- **Create a pull request:** Each team member will create a pull request to merge their changes back into the main codebase.
- **Review and merge:** Using the GitHub website, the repository creator will lead the team in a review of all pull requests. Once the changes have been reviewed, the repository creator will merge the changes back into the main codebase.
- **Pull changes:** Each team member will pull the changes from the main codebase to their local machine.

As we notice the workflow is very similar to the forking and cloning workflow. The key difference is that you do not fork the repository.

## 🎓 You do: Collaborators Git Workflow

In your teams, follow the collaborators workflow. Complete the following tasks:

- Choose a repository creator and have them create a new repository on GitHub.
- When the team gets to the steps **Make Changes** everyone should add a new file called `team.md` to the repository. On the first line of this file put your name. (Every first line of `team.md` should be a different name.)
- Refer back to [Resolving Merge Conflicts Remotely](./merging-and-merge-conflicts/README.md) for instructions on how to resolve merge conflicts.

At the end of this exercise, you should have a new file called `team.md` in the repository with everyone's name in it.

## Forking and Cloning vs. Collaborators

Both of these options are great ways to collaborate with others. The main difference between the two is the level of access you have to the repository. When working on a team it's important to understand the workflow that is being used. This will help you understand how to contribute to the project and what steps you need to take to get your changes merged back into the main codebase.
