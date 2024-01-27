# **CHAPTER 3: GIT BASICS FOR GITHUB**

# **3(a) Installing and Configuring Git**

**Introduction**

Git is an essential tool for managing projects on GitHub. It is a version control system that allows multiple people to work together on a project and tracks changes to the code over time. This section will guide you through the installation and basic configuration of Git.

**Installing Git**

1. Download Git

a. Visit the official Git website: Git Downloads.

b. Select the version compatible with your operating system (Windows, macOS, or Linux/Unix).

2. Installation Process

a. Windows: Run the downloaded .exe file and follow the installation wizard. Accept the default settings or customize as per your preference.

b. macOS: Open the downloaded .dmg file and follow the instructions. You can also install Git via Homebrew by running brew install git in the terminal.
Linux/Unix: Often Git is pre-installed. If not, you can install it via your distribution's package manager (for example, sudo apt-get install git for Debian/Ubuntu).

**Configuring Git**

1. Setting Your Username

a. Open your terminal (Command Prompt or Git Bash on Windows, Terminal app on macOS, or the shell in Linux/Unix).

b. Set your username by running:

command : git config --global user.name "Your Name"

2. Setting Your Email Address

a. Similarly, set your email address (the one associated with your GitHub account):

command : git config --global user.email "your_email@example.com"

3. Checking Your Configuration

a. Verify your settings by running:

command : git config --list

**Conclusion**

With Git installed and configured, you're now ready to start using Git for version control. Remember, these initial steps are a one-time setup; once done, you're all set to explore Git's powerful features.


# **3(b) Basic Git Operations: Clone, Init, Add, Commit, Pull, Push**

**Introduction**

Understanding Git operations is crucial for effectively managing your projects on GitHub. This section will explain the basic commands: clone, init, add, commit, pull, and push, using simple examples for better comprehension.

**Git Operations**

1. Clone

a. Purpose: To create a copy of an existing repository on your local machine.

b. Command: git clone [URL of the repository]

c. Example: To clone a repository, navigate to the desired repository on GitHub, copy its URL, and use git clone https://github.com/username/repository.git in your terminal.

2. Init

a. Purpose: To initialize a new Git repository in your project directory.

b. Command: git init

c. Example: Navigate to your project folder in the terminal and run git init. This command creates a new subdirectory named .git that houses all necessary repository files.

3. Add

a. Purpose: To stage changes for a commit.

b. Command: git add [file] or git add . to add all changes.

c. Example: After editing a file, use git add filename.txt to stage it.

4. Commit

a. Purpose: To save your changes to the local repository.

b. Command: git commit -m "[commit message]"

c. Example: git commit -m "Initial commit" will commit the staged changes with a descriptive message.

5. Pull

a. Purpose: To fetch and integrate changes from the remote repository to your local repository.

b. Command: git pull [remote] [branch]

c. Example: git pull origin main will pull changes from the main branch of the remote repository.

6. Push

a. Purpose: To send your committed changes to a remote repository.

b. Command: git push [remote] [branch]

c. Example: git push origin main will push your commits to the main branch of the remote repository.

**Conclusion**

These basic Git operations form the foundation of project management and collaboration on GitHub. Familiarity with these commands will enable you to contribute to projects and manage your own repositories effectively.


# **3(c) Setting Up a Local Git Repository**

**Introduction**

A local Git repository allows you to work on your project and track changes on your own machine before pushing them to GitHub. This section will guide you through the process of setting up a local repository.

**Steps to Set Up a Local Repository**

1. Create a Project Directory

a. If you don't already have a project directory, create one in your preferred location on your computer.

b. Use your file explorer to create a new folder, or use the mkdir command in the terminal.

2. Initialize the Repository

a. Open your terminal or Git Bash (for Windows users).

b. Navigate to your project directory using the cd command.

c. Run git init. This command creates a new subdirectory named .git that houses all your repository's version control information.

3. Add Project Files

a. Place the files you want to track into your project directory.

b. You can create new files or copy existing files into this directory.

4. Stage Your Files

a. Run git add . to stage all files in the project directory, preparing them for a commit.

b. For specific files, use git add [file-name].

5. Commit the Files

a. Once your files are staged, commit them to the repository with a message describing the changes.

b. Use git commit -m "Initial commit" or replace the message with something more descriptive of the changes made.

6. Link to a Remote Repository (Optional)

a. If you wish to push your local repository to GitHub, first create a remote repository on GitHub.

b. Then, link your local repository to the remote one using git remote add origin [URL of the GitHub repository].

c. Verify the remote repository is linked by using git remote -v.

**Working with Your Local Repository**

a. Check Status: Use git status to see which files are staged, uncommitted, or untracked.

b. View Commit History: git log shows the commit history.

c. Push to GitHub: Once you're ready to share your work or back it up on GitHub, use git push origin [branch-name] to push your commits to the remote repository.

**Conclusion** 

Setting up and maintaining a local Git repository is an integral part of using Git and GitHub. It allows for version control of your projects and facilitates collaboration with others. With these steps, you're now ready to manage your projects using Git.

