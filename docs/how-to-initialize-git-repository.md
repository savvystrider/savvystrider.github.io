# How do I initialize a Git repository?
A **repository** is a directory identified by Git for tracking changes. In order for Git to track changes to documents, it must be **initialized** within the project directory. You can do that with this command:

`git init`

If you run this command in an empty folder, it will create a new, empty repository. The folder will remain empty until files are added.

!!! note

    Actually, the folder will only *appear* to be empty. Executing `git init` creates a `.git` subdirectory with metadata and template files.

If you run this command in an existing project folder, it will re-initialize Git tracking.

!!! note

    `git init` will likely be the first command you run in a new project. Other Git commands will not work until the repository is initialized.

## What happens after I initialize a repository?
You would assume that running the `git init` command will let Git know we would like it to start keeping track of any files in that folder. Unfortunately, Git will not keep track of anything unless you instruct it to. More on that later!


***

##### Sources
- Skoglund, K. (2019). Git Essential Training: The Basics [Video]. LinkedIn Learning. https://www.linkedin.com/learning/git-essential-training-the-basics
- [Pro Git](https://git-scm.com/book/en/v2)
- [Atlassian Git Tutorial](https://www.atlassian.com/git/tutorials/learn-git-with-bitbucket-cloud)