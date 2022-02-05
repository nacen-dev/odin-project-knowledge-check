# Git Basics

## Knowledge Check

- How do you create a new repository on GitHub?
  - You can create a new repository on Github by navigating to the upper right corner of the site and clicking on the + icon then click new repository. 
- How do you copy a repository onto your local machine from GitHub?
  - To copy a repository onto your local machine from Github it needs to be cloned, cloning can be done in three different ways one is cloning through https, second is cloning through ssh, lastly the new way is to use the Github CLI 
- What is the default name of your remote connection?
  - The default name is origin
- Explain what origin is in git push origin main.
  - origin is the default name of the remote connection of your local repository to github
- Explain what main is in git push origin main.
  - main is the default name of the default branch of your git repository you are pushing into
- Explain the two-stage system that Git uses to save files.
  - The staging area where the changes are now being tracked but not yet saved into the repository and commits where changes have been saved into the repository.
- How do you check the status of your current repository?
  - Using the `$git status` command to check the status of the current repository.
- How do you add files to the staging area in git?
  - Using the `$git add` command you can add files to the staging area.
- How do you commit the files in the staging area and add a descriptive message?
  - Using the `$git commit -m message` command will allow you to commit and add a descriptive message.
- How do you push your changes to your repository on GitHub?
  - Using the `$git push` command then referencing the remote connection by default it is origin $git push origin.
- How do you look at the history of your previous commits?
  - Using the `$git log` command you can check the history of your previous commits.