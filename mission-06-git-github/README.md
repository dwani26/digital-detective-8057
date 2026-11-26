
# Mission 6 — Git and GitHub

## 1. Task / Objective

The main aim of this mission was to learn how Git and GitHub work. I learned how to track changes, stage and commit files, create branches and make a Pull Request. I also understood how Git helps when multiple people are working on the same project.

## 2. Work Completed

- Checked the Git repository status and learned how to stage and commit changes.
- Created a new branch named `update-about`.
- Added a **My Learning** section to the main `README.md` file.
- Pushed my branch to GitHub and created a Pull Request from `update-about` to `main`.
- Checked the changes in the Pull Request.
- Wrote down some important Git commands with their meanings.
- Saved my mission notes in `mission-06-task.md`.

**Pull Request status:** Open (not merged).

## 3. Commands / Tools Used

| Git command | Purpose |
|---|---|
| `git status` | Checks the current status of the repository. |
| `git switch -c update-about` | Creates a new branch and switches to it. |
| `git branch` | Shows all the branches in the repository. |
| `git add README.md` | Adds the README file to staging. |
| `git commit -m` | Saves the changes with a commit message. |
| `git log --oneline` | Shows the commit history in a short format. |
| `git log --oneline main..update-about` | Shows the commits available in update-about but not in main. |
| `git push` | Pushes my changes to GitHub. |
| `git push -u origin update-about` | Pushes the new branch to GitHub. |
| `git switch main` | Switches back to the main branch. |

**Tools used:** VS Code, Terminal and GitHub.

## 4. My Understanding

### Task 6.1 — Basic Git Workflow

| Git operation | My understanding |
|---|---|
| Check repository status | It shows which files have been changed and which files are ready to be committed. |
| Stage selected changes | It allows me to select the files that I want to include in my next commit. |
| Create a commit | It saves my changes in Git history along with a message. |
| View commit history | It helps me see my previous commits and understand what changes I made. |

**Difference between staging and committing:**

Staging means selecting the files or changes that I want to save. Committing means actually saving those staged changes in Git history. So, I can choose only the files I want and commit them instead of committing everything together.

### Task 6.2 — Working with Branches

In this task, I created a new branch called `update-about`. I made changes to the root `README.md` file by adding a **My Learning** section.

After making the changes, I checked the repository status, added the README file using `git add README.md` and committed it with the message:

`Add My Learning section to root README`

Finally, I pushed the branch to GitHub.

### Task 6.3 — Creating a Pull Request

After pushing my branch to GitHub, I created a Pull Request from `update-about` to `main`.

I also added a small description explaining the changes I made and checked the modified file in the **Files changed** section.

The Pull Request is still open and has not been merged because the task only required me to create it.

**What is a branch?**

A branch is like a separate working area inside a Git repository. It allows me to make changes without directly affecting the main branch.

**What is a Pull Request?**

A Pull Request is used to request that changes made in one branch should be added to another branch. It also allows other team members to review the changes before merging them.

**Why are branches and Pull Requests useful for teamwork?**

When many people work on the same project, everyone can create their own branch and work separately. Once the work is completed, they can create a Pull Request so that others can check the changes before they are added to the main project.

### Task 6.4 — Git Command Glossary

| Operation | Command | My understanding |
|---|---|---|
| Initialise a repository | `git init` | Creates a Git repository in the current folder. |
| Check status | `git status` | Shows the current changes in the repository. |
| Stage changes | `git add` | Selects the changes that I want to commit. |
| Commit changes | `git commit -m "message"` | Saves the staged changes with a message. |
| View history | `git log --oneline` | Shows the previous commits. |
| Create a branch | `git switch -c name` | Creates a new branch and switches to it. |
| List branches | `git branch` | Shows all the available branches. |
| Switch branches | `git switch name` | Changes from one branch to another. |
| Push changes | `git push` | Uploads my local commits to GitHub. |
| Pull changes | `git pull` | Gets the latest changes from GitHub into my local branch. |

## 5. Difficulties Faced

At first, when I tried to create the Pull Request, GitHub showed the message:

"There isn't anything to compare. main and update-about are identical."

I was confused because I had already created and pushed the `update-about` branch. Later, I understood that I had not made any new changes or commits in that branch. So, both branches were still pointing to the same commit.

## 6. How I Resolved Them

To understand the problem, I used the following commands:

- `git branch` to check the available branches.
- `git log --oneline` to check the commit history.
- `git log --oneline main..update-about` to check whether there were any new commits in my branch.

I found that both branches had the same commit and there were no new commits to compare.

Then I edited the root `README.md` file and added the **My Learning** section. I staged the file, committed the changes and pushed them to GitHub.

After doing this, GitHub was able to show the differences between the two branches, and I successfully created the Pull Request.

## 7. Evidence / Files

- GitHub repository: https://github.com/akash-iyer-27/digital-detective-8028
- Branch created: `update-about`
- Pull Request from `update-about` to `main`.
- Root `README.md` containing the My Learning section.
- `mission-06-git-github/mission-06-task.md` containing my mission notes.
- `mission-06-git-github/README.md` containing this report.

## 8. Commit Details

**Commit messages:**

1. `Add My Learning section to root README` — committed in the `update-about` branch.
2. `Complete Git and GitHub collaboration mission` — committed in the `main` branch.

**Final Status:**

- All the required changes were pushed to GitHub.
- The new branch `update-about` is available on GitHub.
- The Pull Request was successfully created.
- The Pull Request is open and not merged.

**Verification:** I checked my GitHub repository and confirmed that the branch, Pull Request and commits are visible.
