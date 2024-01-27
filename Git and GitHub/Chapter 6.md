# **CHAPTER 6: GITHUB CLI AND ADVANCED GIT TECHNIQUES**

# **6(a) Introduction to GitHub CLI**

**Overview**

GitHub CLI is a powerful tool that brings GitHub functionality to your terminal, allowing you to handle a variety of GitHub actions without leaving the command line. This section introduces the GitHub CLI, its installation, and basic usage.

**What is GitHub CLI?**

a. Definition: GitHub CLI is a command-line tool that enables you to interact with GitHub features directly from your terminal.

b. Benefits:
i.   Streamlines GitHub workflows.
ii.  Allows for scripting and automation of GitHub tasks.
iii. Provides a direct and efficient way to manage issues, pull requests, and other GitHub features.

**Installation**

1. Windows: Download and run the installer from the GitHub CLI release page.

2. macOS: Install using Homebrew with the command: brew install gh.

3. Linux: Choose a package based on your distribution from the installation instructions.

**Setting Up**

a. Run gh auth login and follow the prompts to authenticate your GitHub account.

b. Choose whether to authenticate via a web browser or by pasting a token.

**Conclusion**

The GitHub CLI is an indispensable tool for developers looking to streamline their GitHub workflows. With basic installation and setup, you're ready to start exploring its capabilities.


# **6(b) Basic Commands and Operations with GitHub CLI**

**Introduction**

After setting up GitHub CLI, you can leverage a variety of commands to manage your GitHub activities directly from the command line. This section will cover some fundamental GitHub CLI commands and their uses.

**GitHub CLI Basic Commands**

1. Repository Management

a. Create a New Repository: gh repo create [name]

b. Clone a Repository: gh repo clone [repository]

c. List Repositories: gh repo list [username]

2. Issues and Pull Requests

a. Create an Issue: gh issue create

b. List Issues: gh issue list

c. View an Issue: gh issue view [issue_number]

d. Create a Pull Request: gh pr create

e. List Pull Requests: gh pr list

f. Checkout a Pull Request Locally: gh pr checkout [pr_number]

3. GitHub Actions

a. List Workflow Runs: gh workflow list

b. View a Specific Workflow Run: gh workflow view [workflow_id]

c. View the Log of a Workflow Run: gh run view --log

**Example Workflow with GitHub CLI**

1. Scenario: Managing an Issue and Creating a Pull Request.

2. Steps:
a. Check existing issues: gh issue list

b. Create a new issue: gh issue create and fill in details.

c. Work on the issue in your code editor.

d. Create a new branch: git checkout -b fix-issue

e. Make changes and commit: git commit -am "Fix issue"

f. Push the branch: git push origin fix-issue

g. Create a pull request: gh pr create and follow prompts.

**Conclusion**

GitHub CLI simplifies many routine tasks, making it a valuable tool for developers. Familiarizing yourself with these basic commands can significantly enhance your efficiency in managing GitHub projects.


# **6(c) Advanced Git Techniques for Efficient Workflows**

**Introduction**

Advanced Git techniques can significantly enhance your efficiency and ability to manage complex projects. This section will introduce some powerful Git strategies and best practices for sophisticated project management.

**Advanced Git Techniques**

1. Branching Strategies

a. Feature Branching: Create branches for each new feature to keep changes isolated.

b. Git Flow: A robust branching model designed for release management, including branches like develop, feature, release, and hotfix.

2. Rebasing and Merging

a. Rebase: Use git rebase for a cleaner, linear project history. It integrates changes from one branch into another by applying the changes onto the base branch.

b. Merge Squashing: When merging a feature branch back into the main branch, use git merge --squash to condense all changes into a single commit, keeping the history tidy.

3. Cherry Picking

a. Use git cherry-pick [commit-hash] to apply changes from specific commits to your current branch. This is useful when you need only specific changes from a branch without merging all of them.

4. Stashing Changes

a. Use git stash to temporarily store modified, tracked files when you need to switch contexts. Retrieve the stashed changes with git stash pop.

5. Using Tags for Releases

a. Use git tag to mark specific points in your repository's history, typically used for release versions. E.g., git tag v1.0.0.

**Example Workflow Using Advanced Techniques**

1. Scenario: Implementing a new feature in a separate branch and integrating it into the main branch.

2. Steps:

a. Create a new feature branch: git checkout -b new-feature.

b. Make changes and commit them in the feature branch.

c. Regularly pull changes from the main branch: git pull origin main.

d. Use git rebase main on the feature branch for a linear history.

e. Once the feature is complete, merge it into the main branch using git checkout main and git merge --squash new-feature.

**Conclusion** 

Mastering these advanced Git techniques can dramatically improve your project management, making your workflow more efficient and your repository history cleaner and more understandable.

