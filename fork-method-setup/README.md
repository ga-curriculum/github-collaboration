# ![GitHub Collaboration - Fork Method - Setup](./assets/hero.png)

## Setup

In this lecture, your instructor and a partner they've chosen will demo the GitHub collaboration workflow, and then you'll get the chance to do it all again yourself with a small team.

Before you begin collaborating, you will want to determine who will fill the following roles on your team:

- Programmer
- GitHub manager

Programmers will not manage the GitHub repo for the project but will contribute code to the repo.

GitHub managers will manage the project's GitHub repo while also contributing their own code to the repo.

For this activity, you should designate a single GitHub manager. This will help maintain a clear division of labor and avoid confusion about who is responsible for what task. Any other collaborators will fill the programmer role.

### Create a GitHub repository (***GitHub managers***)

> ⚠️ Only ***GitHub managers*** should complete this task.

Create a new ***public*** repository on [GitHub](https://github.com/) named `github-collaboration`. ***Important***: as you create it, initialize the repository by adding a README file.

Through the rest of this lecture, we'll refer to this as the ***GitHub manager's remote repo***.

Copy the URL to the ***GitHub manager's remote repo*** and distribute it to the programmers on your team.

## Clone the repo (***GitHub managers***)

> ⚠️ Only ***GitHub managers*** should complete this task.

Open your Terminal application and navigate to your `~/code/ga/lectures` directory:

```bash
cd ~/code/ga/lectures
```

Clone the `github-collaboration` repo you just created to your device. Your GitHub username should be present in the URL used in the `git clone` command, like this:

```bash
git clone https://github.com/<your-username>/github-collaboration.git
```

Replacing `<your-username>` (including the `<` and `>`) with your GitHub username.

> 🚨 As always, don't clone into a directory already initialized as a git repository as this will create a nested repo.

Enter the new `github-collaboration` directory. We'll refer to this as the ***GitHub manager's local repo***.

```bash
cd github-collaboration
```

Finally, open it in VS Code:

```bash
code .
```
