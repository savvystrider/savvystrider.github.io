# What is cloning in Git?

A **clone** is a copy of a remote repository that exists on your computer instead of on a website server. **Cloning** is the act of making the copy.

After you [initialize Git](how-to-initialize-git-repository.md) in your local project folder, you can use this basic command to clone an existing repository from GitHub:

`git clone https://github.com/YOUR-USERNAME/YOUR-REPOSITORY`

!!! info

    You can find the URL by navigating to the GitHub repository online and clicking on the green **Code** button. You can clone with the `HTTPS` or `SSH` options.

The `git clone` command creates a copy on your computer of the latest version of the respoitory and its full history. Cloning creates a new branch for you to make your own changes/edits without having to be online. When your changes are ready, you will have to merge the changes from your local branch to the main repository.

***

##### Sources
- [GitHub Docs](https://docs.github.com/en)
- [GitHub Glossary](https://docs.github.com/en/get-started/quickstart/github-glossary)