<h1>
  <span class="headline">GitHub Collaboration</span>
  <span class="subhead">Collaborator Method Working with a Team</span>
</h1>

**Learning objective:** By the end of this lesson, students will be able to use the GitHub workflow to work well as a team.

## GitHub collaboration workflow

You've now seen the collaboration workflow - let's review it:

### Do these things once

- **Choose a GitHub Manager**: The GitHub manager is responsible for merging changes back into the main codebase. This person typically has the most time available to contribute to a project.
- **Add programmers (collaborators)**: The GitHub manager will add collaborators to the repository, giving them write access to the repo.
- **Clone the repository**: Each team member will clone the repository to their local machine.

### Repeat these steps for every new feature

- **Create a new branch**: Each team member will create a new branch to work on a new feature or bug fix.
- **Make changes**: Write code! Build features, fix bugs, and so on.
- **Add, commit, and push the branch to GitHub**: Each team member will push their branch to the repository.
- **Create a pull request**: Each team member will create a pull request to merge their changes into the main codebase.
- **Review and merge**: The GitHub manager will lead the team in reviewing all pull requests. Once the changes have been reviewed, the GitHub manager will merge them into the main codebase.
- **Pull changes**: Each team member will pull the changes from the main codebase to their local machine.

## 🎓 You do

In your teams, follow the GitHub collaboration workflow. Complete the following tasks (***read every step before you begin***):

- Choose a GitHub manager and have them create a new repository on GitHub.
- Complete the steps above. Follow along with the lecture notes to help you complete the steps. Please do not attempt to do this from memory after only seeing it once; you will not have a fun time.
- When the team gets to the **Make Changes** step above, everyone should add a new file called `team.md` to the repository. On the first line of this file, add your name. (Every first line of `team.md` should be a different name.)
- Complete the flow above to push and merge your changes with a pull request.

At the end of this exercise, you should have a new file called `team.md` in the repository with everyone's name in it.

Tip: use this command to view changes to a repo through time:

```bash
git log --decorate --all --graph --oneline
```
