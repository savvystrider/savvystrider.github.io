# How do I commit my changes in Git?
Let's say you have [added a file](how-to-add-files-in-git.md) to the staging index called `newpost.txt`. To get the file into the repository, you must **commit** your changes *and* include a message.

To commit the changes to our file, you can use the following command:

`git commit`

This command commits the file but does not include the required message. Without including a message, your text editor will automatically open and demand a message. You can also use this command to commit *all* changes in the working directory:

`git commit -a`

You can commit and add a message at the same time with this command:

`git commit -m "Initial commit"`

!!! note

    `-m` means you want to add a message. "Initial commit" is the message. Notice that it's wrapped in double-quotes and it's very short. In fact, "Initial commit" is a standard first commit message.

And, yes, if you're wondering, you can add and commit changes at the same time with this command:

`git commit -am "commit message`

This command combines the `-a` and `-m` options above.

***

##### Sources
- Skoglund, K. (2019). Git Essential Training: The Basics [Video]. LinkedIn Learning. https://www.linkedin.com/learning/git-essential-training-the-basics
- [Pro Git](https://git-scm.com/book/en/v2)
- [Atlassian Git Tutorial](https://www.atlassian.com/git/tutorials/learn-git-with-bitbucket-cloud)