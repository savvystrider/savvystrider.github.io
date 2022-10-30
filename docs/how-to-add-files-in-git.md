# How do I add files in Git?

Let's say that you have Git installed *and* you've [initialized the repository](docs/how-to-initialize-git-repository.md). Is Git tracking any new files that you create?

Not until you **add** them.

Let's say you have created a new file called `newpost.txt`. You can run the following command to have Git start tracking it:

`git add newpost.txt`

!!! info

    You can add multiple files at once with this command:

    `git add .`

    The period at the end indicates that *everything* in the current directory should be added. 

Adding a file means that you are adding the file to the **staging index** with the intenion of **committing** your changes. No, you can't commit your changes before adding. That's not how Git works.

After you have added the file, you can use the following command to get a summary of which files have changes that are staged for the next commit:

`git status`

***

##### Sources
- Skoglund, K. (2019). Git Essential Training: The Basics [Video]. LinkedIn Learning. https://www.linkedin.com/learning/git-essential-training-the-basics
- [Pro Git](hhttps://git-scm.com/book/en/v2)