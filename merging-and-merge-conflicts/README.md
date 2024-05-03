# ![GitHub Collaboration - Merging and Merge Conflicts](./assets/hero.png)

**Learning objective:** By the end of this lesson, students will be able to merge branches and handle merge conflicts.

Merging is the process of combining changes from one branch into another. When you merge branches, Git will automatically determine the best way to combine the changes. However, there are times when Git cannot automatically merge the changes, resulting in a merge conflict. In this section we are going to look at merging both locally and remotely, and how to resolve merge conflicts.

## Merging Remotely

Merging branches remotely is done through a pull request. Which is advantageous because we just so happen to have a pull request ready to go. When we merge remotely, we are going to be using the GitHub website. Navigate to the pull request you created in the previous lesson.

This pull request page will have a lot of information on it that is important to understand:

- **Pull Request Number** - This is the number of the pull request.
- **Number of Commits** - This is the number of commits that are in the pull request.
- **Number of Files Changed** - This is the number of files that have been changed in the pull request.
- **Compare Branches** - This is the base branch and the compare branch. The base branch is the branch you want to merge into and the compare branch is the branch you want to merge into the base branch.

> Always take a moment to verify that the branches you are merging are correct. If they are not correct, you can change them by clicking on the `Edit` button next to the branches.

Down near the bottom of the page is the `Merge pull request` button. When you click on this button, GitHub will merge the changes from the compare branch into the base branch. That's it! You have merged the changes remotely. 🎉

But wait there's more! There is one more action we need to take after we merge remotely. We need to pull the changes down to our local machine. If we were working with our own repository it would be as simple as running the following command in the terminal:

```bash
git pull origin main
```

However we are working with a forked repository. This means that we need to pull the changes from the original repository. To do this we need to add the original repository as a remote repository. Navigate to your partner's repository on GitHub and copy the HTTPS key from the drop down `Code` button. Then run the following command in the terminal:

```bash
git remote add upstream <HTTPS key>
```

This action will add another remote location we can pull changes from. Now we can pull the changes from the original repository. Run the following command in the terminal:

```bash
git pull upstream main
```

Remember we have to do this because when we created the pull request we we merged the changes into the original repository. While we made and pushed the changes to our our forked repository through a feature branch, the changes were merged into the `main` branch of the original repository.

**When to Merge Remotely**

Merging remotely is typically done when you are working on a team. This is because it is easier to review code and discuss changes when they are done through a pull request. This is also a good way to keep the main codebase clean and free of bugs. Merge conflicts can still happen when merging remotely, but they are less likely to happen because you are working on a feature branch and not the main codebase.

### Resolving Merge Conflicts Remotely

So what is a merge conflict? A merge conflict happens when Git cannot automatically merge the changes from one branch into another. This can happen when two branches have made changes to the same line of code. When this happens, Git will mark the file with conflict markers. These conflict markers will show you the changes that are in conflict.

When a merge conflict happens remotely, GitHub will let you know. You will see a message that says `This pull request has merge conflicts`. When you see this message, you will need to resolve the merge conflict before you can merge the changes. To resolve the merge conflict, click on the `Resolve conflicts` button. This will take you to the merge conflict page.

On the merge conflict page, you will see the files that have a merge conflict. You will also see the changes that are in conflict. To resolve the conflict, you will need to edit the file and remove the conflict markers. Once you have resolved the conflict, you can click on the `Mark as resolved` button. This will mark the conflict as resolved and you can now merge the changes.

Let's take a look at an example of a merge conflict:

```js
<<<<<<< HEAD
// Current Changes
=======
// Incoming Changes
>>>>>>> compare-branch
```

A merge conflict will always be broken down into the following parts:

- **Incoming Changes** - This is the changes that are coming in from the compare branch.
- **Current Changes** - This is the changes that are currently in the base branch.

The incoming changes will always be between the `<<<<<<< HEAD` and `=======` conflict markers. 

The current changes will always be between the `=======` and `>>>>>>> compare-branch` conflict markers.

To resolve any conflicts, take a look at the contents of the file and decide which changes you want to keep. In some cases, you may want to keep both changes. Once you have decided on the changes, remove the conflict markers you:

- Click on the `Mark as resolved` button.
- Then click the `Commit merge` button.

Once you have commited the changes on GitHub, you will be taken back to the pull request page. You can now merge the changes as you normally would.

> Remember to pull the changes down to your local machine after you have resolved the merge conflict. This will ensure that your local machine is up to date with the remote repository.

## Merging Locally

Merging branches locally is done through the terminal. We want to always follow the same steps when merging branches locally:

- Checkout to the that you want to merge into.
- Merge the branch you want to merge into the you are checkout on.

Let's do this together. First checkout to the `main` branch:

```bash
git checkout main
```

Since we merged our feature branch remotely let's create a new branch to work with locally. Run the following command in your terminal:

```bash
git checkout -b feature/new-feature-two
```

Create and make changes to a new file. Once you have made the change, add and commit the changes. Check back out to the `main` branch:

```bash
git checkout main
```

**Let's Merge**

Now that we have made a change on the `feature/new-feature-two` branch, let's merge the changes into the `main` branch. Run the following command in your terminal:

```bash
git merge feature/new-feature-two
```

You did it! You have merged the changes from the `feature/new-feature-two` branch into the `main` branch. 🎉

> If you have a remote repository connected to your local repository, you will need to push the changes to the remote repository.

**When to Merge Locally**

Merging locally is typically done when you are working on a feature or bug fix. This is because it is easier to test the changes and make sure they work before merging them into the main codebase. Merging locally is also a good way to resolve merge conflicts. If a merge conflict happens, you can resolve the conflict locally before pushing the changes to the remote repository.

> Typically companies will require you to resolve merge conflicts locally before accepting any finished work.

### Resolving Merge Conflicts Locally

Resolving merge conflicts locally is done much like it is done remotely. When a merge conflict happens, Git will mark the file with conflict markers. These conflict markers will show you the changes that are in conflict. A couple of good practices to follow when resolving merge conflicts are:

- **Take your time** - Merge conflicts can be tricky to resolve. Take your time and make sure you understand the changes that are in conflict.
- **Run `git status`** - Running `git status` will show you the files that have a merge conflict. This will help you keep track of the files you need to resolve.
- **Use `crtl + shift + f`** - This will allow you to search for the conflict markers in the entire repository. This will help you find the changes that are in conflict.

Take your time with the code and once you have decided on the changes you want to keep, remove the conflict markers. After you have completed the changes:

- **Add the changes** - `git add .`
- **Commit the changes** - `git commit -m "Resolved merge conflict"`

Then push the changes to the remote repository if you have one connected to your local repository.
