# ![GitHub Collaboration - Fork Method - Pull Requests](./assets/hero.png)

**Learning objective:** By the end of this lesson, students will be able to submit pull requests.

## What's a pull request?

Pull requests (often abbreviated as PRs) allow developers to propose changes to a branch in a repository on GitHub. They are a way to review code and discuss changes before merging them into the main codebase. Pull requests are a central component of collaboration and allow developers to contribute their code to a larger project.

After pushing your code to a branch in a repo on GitHub (as we've already done), the next step is to integrate it into the `main` branch of the original repo by creating a pull request.

## Creating a pull request (***GitHub managers*** and ***programmers***)

> ⚠️ Both ***GitHub managers*** and ***programmers*** should complete this task.

There are many different methods to create a pull request on GitHub. The steps outlined below will ensure a repeatable and consistent experience in as few steps as possible.

You will need:

- The GitHub manager's GitHub username.
- The name of the repository you're working in (`github-collaboration` for this activity).

Navigate to this URL after making the necessary changes to it:

```plaintext
https://github.com/<github-username>/<repo>/compare
```

Replacing `<github-username>` (including the `<` and `>`) with the GitHub manager's GitHub username and `<repo>` (including the `<` and `>`) with the repository name.

> 💡 When working on a project for a prolonged period, it is wise to bookmark this page for easy access!

You should arrive at a page similar to the one shown below.

![Screenshot of the GitHub 'Compare changes' page for the repository 'github-collaboration' in the 'GA-Student' account. The page allows users to compare changes across branches, commits, tags, and more. The user can select a base branch and a comparison branch from dropdown menus.](./assets/github-compare.png)

There are two paths from here. Your role on your team will determine which path you take.

- ***GitHub managers***: Follow the instructions in the **Comparing changes** section below.
- ***Programmers***: Follow the instructions in the **Comparing changes across forks** section below.

### Comparing changes (***GitHub managers*** )

> ⚠️ Only ***GitHub managers***  should complete this task.

When you navigate to the pull request page, you will see the `Comparing changes` section. This section is where you will select the branches you want to compare. Two dropdowns in this section allow you to choose the base branch and the compare branch.

- **Base branch** - This is the branch you want to merge your changes into. This is typically the `main` branch.
- **Compare branch** - This is the branch you want to merge into the base branch. This is typically the feature branch you have been working on. In our case, it is `new-feature`. Note the arrow going from the **compare branch** to the **base branch** - this indicates the flow of your code.

You can see these dropdowns outlined in red in the screenshot below.

![Screenshot of the GitHub 'Compare changes' page for the repository 'github-collaboration' in the 'GA-Student' account. The page allows users to compare changes across branches, commits, tags, and more. The user can select a base branch and a comparison branch from dropdown menus. These are outlined in red.](./assets/github-compare-branches.png)

Select the **compare** dropdown, and select the branch you want to compare to the `main` branch. This is outlined in red in the screenshot below (although the branch name you want to compare to the `main` branch will be different). Note the search feature here - it may be necessary to use this when more branches are made in a repo.

![Screenshot of the GitHub 'Compare changes' page for the repository 'github-collaboration' in the 'GA-Student' account. The 'compare' dropdown menu outlined in red is open, allowing the user to choose a branch or tag to compare with. In the branch list, 'ga-student/new-feature' is outlined in red.](./assets/github-compare-select.png)

After selecting a branch, you'll see the changes made if the pull request is merged. The screenshot below shows that there will be one changed file. One line of code will be added, and no lines will be deleted. After you review the changes, select the **Create pull request** button outlined in red below.

![Screenshot of the GitHub 'Comparing changes' page for the repository 'github-collaboration' in the 'GA-Student' account. The comparison is between the 'main' branch and the 'ga-student/new-feature' branch. The page shows that the branches are 'Able to merge' and the 'Create pull request' button is outlined in red. Below, there is a section displaying '1 commit' and '1 file changed' with '1 addition and 0 deletions.'.](./assets/github-compare-and-pull.png)

Skip to the **Open a pull request** section below.

### Comparing changes across forks (***programmers*** )

> ⚠️ Only ***programmers*** should complete this task.

When you navigate to the pull request page, you will see the `Comparing changes` section.

We want to bring the code that currently only exists in your fork into the ***GitHub manager's*** repo. This means we need to compare across forks. Select the **compare across forks** link outlined in red below.

![Screenshot of the GitHub 'Comparing changes' page for the repository 'github-collaboration' in the 'GA-Student' account. Under the 'Compare changes' header, the 'compare across forks' text is outlined in red.](./assets/github-compare-across-forks.png)

The UI below this link will change slightly. It should now look like the screenshot below. The area that has changed is outlined in red.

![Screenshot of the GitHub 'Comparing changes' page for the repository 'github-collaboration' in the 'GA-Student' account. Under the 'Compare changes' header, the 'compare across forks' user interface is highlighted in red.](./assets/github-compare-across-forks-ui.png)

This section is where you will select the branches you want to compare. Four dropdowns, detailed below, allow you to choose the repositories and branches to compare.

- **Base repository** - This is the repository you want to contribute to. This should be the ***GitHub manager's remote repo***, which you originally forked from.
- **Base branch** - This is the branch you want to merge your changes into. This is typically the `main` branch.

It is unlikely that you will need to modify these from their default value. However, you will likely need to alter the next two dropdowns:

- **Head repository** - This is the repository you want to contribute code from. This is your own ***programmer's remote repo*** (forked from the GitHub manager's repository).
- **Compare branch** - This is the branch you want to merge into the **base branch**. This is typically the feature branch you have been working on. In our case, it is `new-feature`. Note the arrow going from the **head repository**/**compare branch** to the **base repository**/**base branch** - this indicates the flow of your code.

Select the **head repository** dropdown, and choose the `<your-username>/github-collaboration` repository, replacing `<your-username>` (including the `<` and `>`). This is outlined in red in the screenshot below (although the repository name you want to use will be different).

![Screenshot of the GitHub 'Compare changes' page for the repository 'github-collaboration' in the 'GA-Student' account. The 'compare' dropdown menu outlined in red is open, allowing the user to choose a branch or tag to compare with. In the branch list, 'ga-student/new-feature' is outlined in red.](./assets/github-compare-across-forks-head-select.png)

Select the **compare** dropdown, and select the branch you want to compare to the `main` branch in the base repo (in this case, the `new-feature` branch). This is outlined in red in the screenshot below. Note the search feature here - it may be necessary to use this when more branches are made in a repo.

![Screenshot of the GitHub 'Compare changes' page for the repository 'github-collaboration' in the 'GA-Student' account. The 'compare' dropdown menu outlined in red is open, allowing the user to choose a branch or tag to compare with. In the branch list, 'ga-student/new-feature' is outlined in red.](./assets/github-compare-across-forks-compare-select.png)

After selecting a branch, you'll see the changes made if the pull request is merged. The screenshot below shows that there will be one changed file. One line of code will be added, and no lines will be deleted. After you review the changes, select the **Create pull request** button outlined in red below.

![Screenshot of the GitHub 'Comparing changes' page for the repository 'github-collaboration' in the 'GA-Student' account. The comparison is between the 'main' branch and the 'ga-student/new-feature' branch. The page shows that the branches are 'Able to merge' and the 'Create pull request' button is outlined in red. Below, there is a section displaying '1 commit' and '1 file changed' with '1 addition and 0 deletions.'.](./assets/github-compare-across-forks-and-pull.png)

Continue to the **Open a pull request** section below.

## Open a pull request (***GitHub managers*** and ***programmers***)

> ⚠️ Both ***GitHub managers*** and ***programmers*** should complete this task.

You'll be taken to a new page where you can open your pull request. Here, you will give your pull request a title and brief summary.

1. **Title**: The title should concisely describe the change the pull request will make to the main branch, similar to a commit message. Keep it short but descriptive.

2. **Description**: Detail the changes your code will make here. This will help the reviewer understand what changes you made and why you made them.

After setting up the title and description, select the **Create pull request** button as outlined in red below. This will create the pull request and take you to the pull request page.

![Screenshot of the 'Open a pull request' page on GitHub. The page shows a comparison between the 'main' branch and 'ga-student/new-feature' branch, with a message indicating 'Able to merge'. A green 'Create pull request' button is outlined in red.](./assets/github-create-pr.png)

> 🧠 You can still create a pull request even if you cannot automatically merge your changes.

Congrats! You have created a pull request! 🎉
