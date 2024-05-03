# ![GitHub Collaboration - Pull Requests](./assets/hero.png)

**Learning objective:** By the end of this lesson, students will be able to tktk

Pull requests are a way to propose changes to a repository on GitHub. They are a way to review code and discuss changes before merging them into the main codebase. Let's create a pull request.

## Creating a Pull Request

While a lot of the GitHub workflow can be done through the command line, creating a pull request is something that is typically done through the GitHub website. When creating a pull request, you always navigate to **your repository** on GitHub. It does not matter if you have forked a repository or if it is your own repository you will always start off your pull request from your repository. Using the browser, navigate to the repository you have forked, cloned, and pushed the feature branch to.

There are a number of way to navigate to the pull request page:

- **From the terminal** - Everytime you push a new branch to GitHub, the terminal will output a link to the pull request page. You can copy and paste this link into your browser.
- **From the GitHub website** 
  - Navigate to the repository on GitHub and click on the `Pull requests` tab. From there you can click on the `New pull request` button.
  - Sometimes there is a yellow banner at the top of the repository that says `Compare & pull request`. You can click on that banner to start a new pull request.

Whichever way you choose to navigate to the pull request page, you will notice that all locations will take you to the same place.

### Comparing Changes

When you navigate to the pull request page, you will see a few different sections. The first section is the `Comparing changes` section. This section is where you will select the branches you want to compare. There will be two dropdowns that allow you to select the base branch and the compare branch.

- **Base branch** - This is the branch you want to merge your changes into. This is typically the `main` or `dev` branch.
- **Compare branch** - This is the branch you want to merge into the base branch. This is typically the feature branch you have been working on. In our case, it is `feature/new-feature-one`.

> Even if you cannot automatically merge your changes, you can still create a pull request.

The second section is the **Title** and **Description** section. This is where you will give your pull request a title and a description. The title should be short and descriptive. The description should be more detailed and explain what changes you made and why you made them. When leaving a description, it is important to be as detailed as possible. This will help the reviewer understand what changes you made and why you made them.

After you have selected the branches you want to compare and given your pull request a title and description, you can click on the `Create pull request` button. This will create the pull request and take you to the pull request page.

Congrates! You have created a pull request! 🎉

## Examine the Git Workflow so Far

During this lesson we have accomplished the following:

- Forked a repository
  - This creates a copy of the repository on your GitHub account.
- Cloned the repository
  - This downloads the repository to your local machine.
- Created a new branch
  - This allows you to work on a new feature or bug fix without affecting the main codebase.
- Pushed the branch to GitHub
  - This uploads the branch to your GitHub account.
- Created a pull request
  - This allows you to propose changes to the main codebase.

This circle of events is the typical workflow when working with Git and GitHub. You will find yourself doing these steps over and over again as you work on new features and bug fixes.
