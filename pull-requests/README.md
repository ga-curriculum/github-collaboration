# ![GitHub Collaboration - Pull Requests](./assets/hero.png)

**Learning objective:** By the end of this lesson, students will be able to submit pull requests.

Pull requests are a way to propose changes to a repository on GitHub. They are a way to review code and discuss changes before merging them into the main codebase. Let's create a pull request.

## Creating a Pull Request

Creating a pull request on GitHub is typically done through the GitHub website, not the command line. Here’s how you can start:

1. **Open Your Repository**: Go to the GitHub website and navigate to your repository. This could be a repository you own or one you have forked.
2. **Access the Pull Request Page**: You have a couple of options to do this:
   - **Using the terminal**: After you push a new branch to GitHub, the terminal will display a URL for creating a pull request. Copy this URL and paste it into your browser.
   - **Using the GitHub website**:
     - Click on the `Pull requests` tab located at the top of your repository page, then click the `New pull request` button.
     - Alternatively, if you see a yellow banner saying `Compare & pull request` at the top of your repository page, click on it to start the process.

No matter which method you choose, all these options lead to the same pull request creation page.

### Comparing Changes

When you navigate to the pull request page, you will see a few different sections. The first section is the `Comparing changes` section. This section is where you will select the branches you want to compare. There will be two dropdowns that allow you to select the base branch and the compare branch.

- **Base branch** - This is the branch you want to merge your changes into. This is typically the `main` or `dev` branch.
- **Compare branch** - This is the branch you want to merge into the base branch. This is typically the feature branch you have been working on. In our case, it is `feature/new-feature-one`.

> Even if you cannot automatically merge your changes, you can still create a pull request.

### Add details

The second section is the **Title** and **Description** section. This is where you will give your pull request a title and brief summary.

1. **Title**: The title should be short and descriptive. The description should be more detailed and explain what changes you made and why you made them.

2. **Description**: When leaving a description, it is important to be as detailed as possible. This will help the reviewer understand what changes you made and why you made them.

After setting up the title and description, and selecting the branches you want to compare:

- Click on the `Create pull request` button. This will create the pull request and take you to the pull request page.

Congrats! You have created a pull request! 🎉

## Reviewing our Git workflow

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

This series of steps is the typical workflow when working with Git and GitHub. You will find yourself doing these steps over and over again as you work on new features and bug fixes.
