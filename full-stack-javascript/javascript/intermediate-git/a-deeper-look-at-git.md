# A Deeper Look at Git

### How can you amend your last commit?

Using the `git commit --amend` command

### What are some different ways to rewrite history?

- `git commit --ammend`
- `git rebase`
- `git reset`
- `git revert`

### What is a safe way to push history changes to a remote repository?

Updating the local history using fetch, merge, and then attempting to push again.

### What are the dangers of history-changing operations

It can destroy files other people are working on, it can cause conflicts in the history

### What are best practices of history-changing operations

1.  If working on a team project, make sure rewriting history is safe to do and others know you’re doing it.

2.  Ideally, stick to using these commands only on branches that you’re working with by yourself.

3.  Using the -f flag to force something should scare you, and you better have a really good reason for using it.

4.  Don’t push after every single commit, changing published history should be avoided when possible.

5.  Regarding the specific commands we’ve covered:

    - For git amend never amend commits that have been pushed to remote repositories.
    - For git rebase never rebase a repository that others may work off of.
    - For git reset never reset commits that have been pushed to remote repositories.
    - For git push --force only use it when appropriate, use it with caution, and preferably default to using git push --force-with-lease.

### Explain what it means for branches to be pointers

Branches points to a single commit which is the latest commit this, but how does the branch knows about all the commit inside it? Even though the branch only points to the latest commit, every commit is a pointer to the commit before it so it can be thought of like this

Branch points to Z
Z points to X which is the previous commit before it
X points to Y which is again the previous commit for it
Y doesn't point to anything that means it's the first commit
